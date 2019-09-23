---
title: Beheben von Problemen beim parallelen Veröffentlichen in Brand Portal
seo-title: Beheben von Problemen beim parallelen Veröffentlichen in Brand Portal
description: Erfahren Sie, wie Sie Probleme beim parallelen Veröffentlichen beheben können.
seo-description: Erfahren Sie, wie Sie Probleme beim parallelen Veröffentlichen beheben können.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: Referenz
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Beheben von Problemen beim parallelen Veröffentlichen in Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal unterstützt die Integration mit AEM Assets, damit genehmigte Markenelemente nahtlos aus der Autoreninstanz von AEM Assets erfasst (oder veröffentlicht) werden können. Once [integrated](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html), AEM Author uses a replication agent to replicate the selected asset(s) to Brand Portal cloud service for approved usage by Brand Portal users. Mehrere Replizierungsagenten werden für die schnelle parallele Veröffentlichung mit AEM 6.2 SP1-CFP5], AEM CFP 6.3.0.2 und höher verwendet.

>[!NOTE]
>
>Adobe empfiehlt ein Upgrade auf AEM 6.4.1.0, um sicherzustellen, dass AEM Assets Brand Portal erfolgreich mit AEM Assets integriert ist. A limitation in AEM 6.4 gives an error while configuring integration with Brand Portal and replication fails.

Beim Konfigurieren des Cloud-Service für Brand Portal unter [!UICONTROL /etc/cloudservice] werden alle erforderlichen Benutzer und Token automatisch generiert und im Repository gespeichert. Die Cloud-Service-Konfiguration wird erstellt, Servicebenutzer, die für Replikation und Replikationsagenten erforderlich sind, um Inhalte zu replizieren, werden ebenfalls erstellt. Hierbei werden vier Replikationsagenten erstellt. So when you publish numerous assets from AEM to Brand Portal, these are queued and distributed among these replication agents through Round Robin.

However, publishing can fail intermittently due to- large sling jobs, increased Network and [!UICONTROL Disk I/O] on AEM Author instance, or slowed performance of AEM Author instance. Daher wird empfohlen, die Verbindung zu den Replikationsagenten zu testen, bevor mit dem Veröffentlichen begonnen wird.

![](assets/test-connection.png)

## Troubleshoot failures in first time publishing: validating your publish configuration {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

So validieren Sie Ihre Veröffentlichungskonfigurationen:

1. Überprüfen Sie die Fehlerprotokolle.
2. Überprüfen Sie, ob der Replikationsagent erstellt wurde.
3. Testen Sie die Verbindung.

**Protokolle beim Erstellen des Cloud-Dienstes nachverfolgen**

Prüfen Sie die Protokollfragmente. Überprüfen Sie, ob der Replikationsagent erstellt wurde oder nicht. Wenn die Erstellung des Replikationsagenten scheitert, bearbeiten Sie den Cloud-Service, indem Sie geringfügige Änderungen am Cloud-Service vornehmen. Validieren und überprüfen Sie erneut, ob der Replikationsagent erstellt wurde oder nicht. Falls nicht, bearbeiten Sie den Service erneut.

Wenn der Cloud-Service selbst nach mehrmaligem Bearbeiten nicht richtig konfiguriert ist, senden Sie ein Daycare-Ticket.

**Testen der Verbindung zu Replikationsagenten**

Sehen Sie sich das Protokoll an. Wenn im Replikationsprotokoll Fehler gemeldet werden:

1. Wenden Sie sich an den Adobe Support.

2. Wiederholen Sie die [Bereinigung](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) und erstellen Sie die Veröffentlichungskonfiguration erneut.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Vorhandene Veröffentlichungskonfigurationen in Brand Portal bereinigen {#clean-up-existing-config}

Most of the times when publishing is not working, the reason can be that the user who is publishing (for example: [!UICONTROL mac-&lt;tenantid&gt;-replication]) doesn't have the latest private key, and hence publish fails with "401 unauthorized" error and no other error is reported in replication agent logs. Um die Problembehebung zu vermeiden, können Sie stattdessen eine neue Konfiguration erstellen. Damit die neue Konfiguration ordnungsgemäß funktioniert, müssen Sie Folgendes aus dem AEM-Autor-Setup bereinigen:

1. go to [!UICONTROL localhost:4502/crx/de] (considering you are running author instance on [!UICONTROL localhost:4502]):\
   i. delete /etc/replication/agents.author/mp_Replication*\
   ii. delete /etc/cloudservices/mediaportal/&lt;config_name&gt;

2. Gehen Sie zu [!UICONTROL localhost:4502/useradmin]:\
   i search for user [!UICONTROL mac-&lt;tenantid&gt;-replication
ii delete this user

Jetzt wird das gesamte System bereinigt. Jetzt können Sie versuchen, eine neue  cloudservice  config and still use the already existing JWT application in [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/). Es ist nicht notwendig, eine neue Anwendung zu erstellen. Stattdessen muss einfach nur der öffentliche Schlüssel in der neu erstellten Cloud-Konfiguration aktualisiert werden.

## Problem mit der Sichtbarkeit der Developer Connection-JWT-Anwendung {#developer-connection-jwt-application-tenant-visibility-issue}

If on [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/), all the  orgs  (tenants) for which the current users hold system administrator are listed. Wenn Sie den Organisationsnamen hier nicht finden oder Sie eine Anwendung für einen erforderlichen Mandanten hier nicht erstellen können, überprüfen Sie, ob Sie über ausreichende (Systemadministrator-)Rechte hierfür verfügen.

Auf dieser Benutzeroberfläche gibt es das bekannte Problem, dass nur die Top-10-Anwendungen für einen Mandanten sichtbar sind. Wenn Sie die Anwendung erstellen, bleiben Sie auf dieser Seite und erstellen Sie ein Lesezeichen für die URL. Sie müssen nicht zur Auflistungsseite der Anwendung wechseln und die von Ihnen erstellte Anwendung suchen. Sie können diese als Lesezeichen gespeicherte URL direkt aufrufen und die Anwendung bei Bedarf aktualisieren/löschen.

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

Wenn ein Replikationsagent, mit dem das Veröffentlichen in Brand Portal bisher korrekt funktionierte, keine Veröffentlichungsaufträge mehr verarbeitet, prüfen Sie die Replikationsprotokolle. In AEM ist eine Funktion zur automatischen Wiederholung integriert. Wenn das Veröffentlichen eines bestimmten Assets scheitert, wird automatisch ein Wiederholungsversuch gestartet. Wenn ein temporäres Problem aufgetreten ist, z. B. ein Netzwerkfehler, kann eine Wiederholung erfolgreich sein.

If there are continuous publish failures and queue is blocked, then you should check **[!UICONTROL test connection]** and try to solve the errors that are being reported.

Basierend auf den Fehlern kann es empfehlenswert sein, ein Support-Ticket zu öffnen, damit das Brand Portal-Technikerteam Ihnen beim Beheben der Probleme helfen kann.
