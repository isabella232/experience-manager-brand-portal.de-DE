---
title: Beheben von Problemen beim parallelen Veröffentlichen in Brand Portal
seo-title: Troubleshoot issues in parallel publishing to Brand Portal
description: Erfahren Sie, wie Sie Probleme beim parallelen Veröffentlichen beheben können.
seo-description: Troubleshoot parallel publishing.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: e95dbff93ec4d207fe32a1752f9ccf59ee7c4e90
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 54%

---

# Beheben von Problemen beim parallelen Veröffentlichen in Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal ist mit Experience Manager Assets so konfiguriert, dass genehmigte Marken-Assets nahtlos aus der Experience Manager Assets-Autoreninstanz aufgenommen (oder veröffentlicht) werden. Sobald [konfiguriert](../using/configure-aem-assets-with-brand-portal.md), verwendet die Experience Manager-Autoreninstanz einen Replikationsagenten, um die ausgewählten Assets im Brand Portal-Cloud-Service zu replizieren, damit Brand Portal-Benutzer genehmigte Assets verwenden. Mehrere Replikationsagenten werden in Experience Manager 6.2 SP1-CFP5, Experience Manager CFP 6.3.0.2 und höher verwendet, um eine schnelle parallele Veröffentlichung zu ermöglichen.

>[!NOTE]
>
>Adobe empfiehlt ein Upgrade auf Experience Manager 6.4.1.0, um sicherzustellen, dass Experience Manager Assets Brand Portal erfolgreich mit Experience Manager Assets konfiguriert ist. Aufgrund der Einschränkungen in Experience Manager 6.4 tritt beim Konfigurieren von Experience Manager Assets mit Brand Portal ein Fehler auf, und die Replikation schlägt fehl.

Beim Konfigurieren des Cloud-Service für Brand Portal unter **[!UICONTROL /etc/cloudservice]** werden alle erforderlichen Benutzer und Token automatisch generiert und im Repository gespeichert. Die Cloud-Service-Konfiguration wird erstellt, Servicebenutzer, die für Replikation und Replikationsagenten erforderlich sind, um Inhalte zu replizieren, werden ebenfalls erstellt. Es werden vier Replikationsagenten erstellt. Wenn Sie also zahlreiche Assets aus Experience Manager in Brand Portal veröffentlichen, werden die Assets in die Warteschlange gestellt und über Round Robin unter den Replikationsagenten verteilt.

Jedoch kann das Veröffentlichen zwischenzeitlich aufgrund zu großer Sling-Aufträge, erhöhter Netzwerk- und **[!UICONTROL Datenträger-E/A]**-Vorgänge in der Experience Manager-Autoreninstanz oder geringer Leistung der Experience Manager-Autoreninstanz scheitern. Es wird daher empfohlen, die Verbindung mit den Replikationsagenten zu testen, bevor Sie mit der Veröffentlichung beginnen.

![](assets/test-connection.png)

## Beheben von Problemen bei der ersten Veröffentlichung: Validieren der Veröffentlichungskonfiguration {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

So validieren Sie Ihre Veröffentlichungskonfigurationen:

1. Überprüfen Sie die Fehlerprotokolle.
1. Überprüfen Sie, ob der Replikationsagent erstellt wurde.
1. Testen Sie die Verbindung.

**Prüfen der Protokollfragmente beim Erstellen des Cloud Service**

Prüfen Sie die Protokollfragmente. Überprüfen Sie, ob der Replikationsagent erstellt wurde oder nicht. Wenn die Erstellung des Replikationsagenten scheitert, bearbeiten Sie den Cloud-Service, indem Sie geringfügige Änderungen am Cloud-Service vornehmen. Validieren und überprüfen Sie erneut, ob der Replikationsagent erstellt wurde oder nicht. Falls nicht, bearbeiten Sie den Service erneut.

Wenn der Cloud-Service selbst nach mehrmaligem Bearbeiten nicht richtig konfiguriert ist, senden Sie ein Daycare-Ticket.

**Testen der Verbindung zu Replikationsagenten**

Sehen Sie sich das Protokoll an. Wenn im Replikationsprotokoll Fehler gemeldet werden:

1. Wenden Sie sich an den Support.

1. Wiederholen Sie die [Bereinigung](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) und erstellen Sie die Veröffentlichungskonfiguration erneut.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Vorhandene Veröffentlichungskonfigurationen in Brand Portal bereinigen {#clean-up-existing-config}

Wenn eine Veröffentlichung nicht funktioniert, liegt das meistens daran, dass der Benutzer, der die Veröffentlichung durchführt (z. B. `mac-<tenantid>-replication`) nicht den neuesten privaten Schlüssel hat. Daher scheitert die Veröffentlichung mit dem Fehler „401 unauthorized“ und in den Replikationsagenten-Protokollen wird kein anderer Fehler gemeldet. Möglicherweise sollten Sie die Fehlerbehebung vermeiden und stattdessen eine Konfiguration erstellen. Damit die neue Konfiguration ordnungsgemäß funktioniert, bereinigen Sie Folgendes in der Einrichtung des Experience Manager-Autors:

1. Gehen Sie zu `localhost:4502/crx/de/` (unter Berücksichtigung der Tatsache, dass Sie die Autoreninstanz auf localhost::4502: ausführen)\
   i. Löschen Sie `/etc/replication/agents.author/mp_replication`
ii. Löschen Sie 
`/etc/cloudservices/mediaportal/<config_name>`

1. Gehen Sie zu localhost:4502/useradmin:\
   i. Suchen Sie den Benutzer `mac-<tenantid>replication`
ii. Löschen Sie diesen Benutzer

Jetzt wird das gesamte System bereinigt. Jetzt können Sie versuchen, eine Cloud Service-Konfiguration zu erstellen und weiterhin die vorhandene JWT-Anwendung zu verwenden. Es ist nicht erforderlich, eine Anwendung zu erstellen, sondern den öffentlichen Schlüssel aus der neu erstellten Cloud-Konfiguration zu aktualisieren.

>[!NOTE]
>
>Ändern Sie keine automatisch generierten Einstellungen.


## Problem mit der Sichtbarkeit der Developer Connection-JWT-Anwendung {#developer-connection-jwt-application-tenant-visibility-issue}

In `https://legacy-oauth.cloud.adobe.io/` sind alle Organisationen (Mandanten) aufgelistet, für die die aktuellen Benutzer Systemadministrator sind. Wenn Sie den Organisationsnamen hier nicht finden oder Sie hier keine Anwendung für einen erforderlichen Mandanten erstellen können, überprüfen Sie bitte, ob Sie über ausreichende (Systemadministrator-) Rechte verfügen.

Auf dieser Benutzeroberfläche gibt es ein bekanntes Problem, dass für jeden Mandanten nur die Top-10-Anwendungen sichtbar sind. Wenn Sie die Anwendung erstellen, bleiben Sie auf dieser Seite und erstellen Sie ein Lesezeichen für die URL. Sie müssen nicht zur Auflistungsseite der Anwendung wechseln und die von Ihnen erstellte Anwendung suchen. Sie können diese als Lesezeichen gespeicherte URL direkt aufrufen und die Anwendung bei Bedarf aktualisieren/löschen.

Die JWT-Anwendung wird unter Umständen nicht korrekt aufgelistet. Daher wird empfohlen, beim Erstellen der JWT-Anwendung ein Lesezeichen für die URL zu setzen oder sie sich zu notieren.

## Laufende Konfiguration funktioniert nicht mehr {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

Wenn ein Replikationsagent, der gerade in Brand Portal veröffentlicht wurde, die Verarbeitung von Veröffentlichungsaufträgen stoppt, überprüfen Sie die Replikationsprotokolle. In Experience Manager ist die Funktion zum automatischen Wiederholen integriert. Wenn die Veröffentlichung eines bestimmten Assets scheitert, wird der Versuch daher automatisch wiederholt. Wenn es ein zeitweiliges Problem gibt, z. B. einen Netzwerkfehler, kann es bei einem erneuten Versuch erfolgreich sein.

Wenn jedoch kontinuierliche Fehler beim Veröffentlichen auftreten und die Warteschlange blockiert ist, sollten Sie **[!UICONTROL Verbindung testen]** auswählen und versuchen, die dort gemeldeten Fehler zu beheben.

Basierend auf den Fehlern kann es empfehlenswert sein, ein Support-Ticket zu öffnen, damit das Brand Portal-Technikerteam Ihnen beim Beheben der Probleme helfen kann.


## Konfigurieren von Replikationsagenten, um Verbindungsabbrüche wegen Zeitüberschreitung zu verhindern {#connection-timeout}

Normalerweise schlägt der Veröffentlichungsauftrag mit einem Zeitüberschreitungsfehler fehl, wenn die Replikationswarteschlange mehrere ausstehende Anforderungen enthält. Um das Problem zu beheben, konfigurieren Sie die Replikationsagenten so, dass keine Zeitüberschreitung erfolgt.

So konfigurieren Sie die Replikationsagenten:

1. Melden Sie sich bei der AEM Assets-Autorenistanz an.
1. Navigieren Sie im Bedienfeld **Tools** zu **[!UICONTROL Bereitstellung]** > **[!UICONTROL Replikation]**.
1. Klicken Sie auf der Seite „Replikation“ auf **[!UICONTROL Agenten für Autor]**. Sie sehen die vier Replikationsagenten Ihres Brand Portal-Mandanten.
1. Klicken Sie auf die Replikationsagenten-URL und klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. Klicken Sie in den Agenteneinstellungen auf die Registerkarte **[!UICONTROL Erweitert]**.
1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Verbindung schließen]**.
1. Wiederholen Sie die Schritte 4 bis 7, um alle vier Replikationsagenten zu konfigurieren.
1. Starten Sie den Server neu.
