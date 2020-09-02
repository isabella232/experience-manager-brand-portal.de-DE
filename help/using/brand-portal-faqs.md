---
title: Häufig gestellte Fragen
seo-title: null
description: Hier erhalten Sie Antworten auf häufig gestellte Fragen, die in Adobe Experience Manager Assets Brand Portal veröffentlicht wurden.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: a32eed22ebfbc683fca96950fc2e08bf5cfaccb3
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 99%

---


# Häufig gestellte Fragen {#frequently-asked-questions}

Die häufig gestellten Fragen zu Brand Portal betreffen die Fragen und Probleme von Endbenutzern, die bei der Arbeit mit der neuesten Version 6.4.6 von AEM Assets Brand Portal oder mit früheren Versionen auftreten können.


## Häufig gestellte Fragen zu Brand Portal 6.4.6 {#faqs-bp646}

**Frage. Der vorhandene alte OAuth-Endpunkt (`https://legacy-oauth.cloud.adobe.io/login`) funktioniert nicht. Was könnte der Grund sein?**

**Antwort.** Die alte OAuth-Konfiguration wird nicht mehr unterstützt. Sie müssen die Autoreninstanzen von AEM Assets auf das neueste Service Pack aktualisieren und es mithilfe von Adobe Developer Console konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren von AEM Assets mit Brand Portal](configure-aem-assets-with-brand-portal.md). Um die alte OAuth-Konfiguration jedoch bis zum Upgrade verwenden zu können, ändern Sie den alten OAuth-Endpunkt in `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Frage. Nach der Aktualisierung auf Adobe Developer Console kann ich die Assets des Beitragsordners von Brand Portal nicht in AEM Assets veröffentlichen. Meine Autoreninstanz befindet sich unter AEM 6.5.4. Was könnte der Grund sein?**

**Antwort.** Ja, es gibt ein bekanntes Problem bei der Veröffentlichung von Assets des Beitragsordners in AEM Assets unter AEM 6.5.4 über Adobe Developer Console.

Das Problem wurde in AEM 6.5.5 behoben. Sie können Ihre AEM Assets-Instanz auf das neueste Service Pack AEM 6.5.5 aktualisieren und Ihre Konfigurationen in Adobe Developer Console [aktualisieren](https://docs.adobe.com/content/help/de-DE/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.translate.html#upgrade-integration-65).

Zur sofortigen Fehlerbehebung unter AEM 6.5.4 wird empfohlen, [den Hotfix herunterzuladen](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) und auf der AEM-Autoreninstanz zu installieren.

**Frage. Der Inhalt des Beitragsordners wird nicht aus Brand Portal in AEM Assets veröffentlicht. Was könnte der Grund sein?**

**Antwort.** Wenden Sie sich an Ihren AEM Assets-Administrator, damit er die Konfigurationen überprüft, und stellen Sie sicher, dass für den Brand Portal-Mandanten nur eine Autoreninstanz konfiguriert ist.

Dieses Problem tritt möglicherweise auf, wenn Sie einen Brand Portal-Mandanten auf mehreren AEM Assets-Autoreninstanzen konfiguriert haben. Wenn z. B. der Administrator denselben Brand Portal-Mandanten auf der AEM Assets-Autoreninstanz der Staging- und Proudktionsumgebung konfiguriert, wird die Asset-Veröffentlichung in Brand Portal zwar ausgelöst, die AEM Assets-Autoreninstanz kann das Asset jedoch nicht importieren, da der Replikationsagent das Anfrage-Token nicht erhält.


**Frage. Ich kann keine Assets aus AEM Assets in Brand Portal veröffentlichen. Im Replikationsprotokoll wird angegeben, dass bei der Verbindung eine Zeitüberschreitung aufgetreten ist. Gibt es eine schnelle Lösung?**

**Antwort.** Normalerweise schlägt die Veröffentlichung mit einem Zeitüberschreitungsfehler fehl, wenn die Replikationswarteschlange mehrere ausstehende Anforderungen enthält. Um das Problem zu beheben, konfigurieren Sie die Replikationsagenten so, dass keine Zeitüberschreitung erfolgt.

Gehen Sie wie folgt vor, um den Replikationsagenten zu konfigurieren:
1. Melden Sie sich bei der AEM Assets-Autorenistanz an.
1. Navigieren Sie im Bedienfeld **Tools** zu **[!UICONTROL Bereitstellung]** > **[!UICONTROL Replikation]**.
1. Klicken Sie auf der Seite „Replikation“ auf **[!UICONTROL Agenten für Autor]**. Sie sehen die vier Replikationsagenten für Ihren Brand Portal-Mandanten.
1. Klicken Sie auf die Replikationsagenten-URL, um die Agentendetails zu öffnen.
1. Klicken Sie auf **[!UICONTROL Bearbeiten]**, um die Einstellungen des Replikationsagenten zu ändern.
1. Klicken Sie in den Agenteneinstellungen auf die Registerkarte **[!UICONTROL Erweitert]**.
1. Aktivieren Sie das Kontrollkästchen Verbindung **[!UICONTROL schließen]** .
1. Wiederholen Sie die Schritte 4 bis 7, um alle vier Replikationsagenten zu konfigurieren.
1. Starten Sie den Server neu und überprüfen Sie die Verbindung.


## Häufig gestellte Fragen zu Brand Portal 6.4.5 {#faqs-bp645}

**Frage. Was ist die wichtigste Änderung in Version 6.4.5 von Brand Portal?**

**Antwort.** In AEM Assets Brand Portal 6.4.5 haben Benutzer von Brand Portal die Möglichkeit, Inhalte aus der Brand Portal-Instanz hochzuladen und den Beitragsordner ohne Administratorrechte wieder in AEM Assets zu veröffentlichen.
Weitere Informationen finden Sie in [Asset-Beschaffung in Brand Portal](brand-portal-asset-sourcing.md).



**Frage. Verliere ich den Zugriff auf vorhandene Assets, Funktionen oder Konfigurationen, die ich erstellt habe?**

**Antwort.** Alle bestehenden Funktionen und Konfigurationen stehen weiterhin zur Verfügung. Es gibt keine Auswirkungen auf Ihre Endbenutzer und Ihre Inhalte bleiben unverändert.



**Frage. Wann findet der Wechsel zur neuen Brand Portal-Version statt?**

**Antwort.** Brand Portal 6.4.5 wurde im Oktober 2019 für die Produktion freigegeben. Die nächste Brand Portal-Version wird voraussichtlich im 3. Quartal 2020 veröffentlicht.
Bezüglich Updates und Versionsänderungen wird empfohlen, die [Versionshinweise](brand-portal-release-notes.md) und [Neuigkeiten in Brand Portal](whats-new.md) zu verfolgen.



**Frage. Wie sind die Auswirkungen auf meine Benutzer?**

**Antwort.** Die Brand Portal-Version 6.4.5 ist ausschließlich in Brand Portal verfügbar, sodass keine Auswirkungen auf Ihre Endbenutzer auftreten.



**Frage. Muss ich als Benutzer von Brand Portal irgendwelche Aufgaben durchführen?**

**Antwort.** Brand Portal-Version 6.4.5 enthält eine neue Funktion namens &quot;Asset-Beschaffung&quot;. Der AEM-Administrator muss die Asset-Beschaffung in AEM Assets konfigurieren, um diese Funktion für die Brand Portal-Benutzer zu aktivieren. Weitere Informationen finden Sie unter [Aktivieren der Asset-Beschaffung](brand-portal-configure-asset-sourcing.md).



**Frage. Wer kann einen Beitragsordner erstellen?**

**Antwort.** Jeder AEM-Benutzer, der berechtigt ist, einen neuen Ordner in AEM Assets zu erstellen, kann einen **Beitragsordner** erstellen. Erstellen Sie zum Erstellen eines **Beitragsordners** einen neuen Ordner des Typs **Asset-Beitrag**.
Dieser Ordner ist für die aktiven Brand Portal-Benutzer freigegeben, die daraufhin Beiträge beisteuern können.



**Frage. Was enthält ein Beitragsordner?**

**Antwort.** Der **Beitragsordner** enthält die beiden Unterordner **NEU** und **FREIGEGEBEN**. Zunächst ist der Ordner NEU leer, und der Ordner SHARED enthält den Referenzinhalt (wiederverwendbare Assets) für die Brand Portal-Benutzer.
Die Brand Portal-Benutzer greifen auf den **Beitragsordner** zu und laden Inhalte in den Ordner **NEU** hoch.



**Frage.  Kann ich den Namen eines bestehenden Beitragsordners ändern?**

**Antwort.** **Nein**, Sie können den Namen eines bestehenden **Beitragsordners** nicht ändern.



**Frage. Wie hoch sind die Anforderungen an Asset-Beiträge?**

**Antwort.** Das **kurze** Dokument, das dem **Beitragsordner** beigefügt ist, sowie der im Ordner **FREIGEGEBEN** hochgeladene Referenzinhalt (wiederverwendbare Assets) verdeutlichen den Brand Portal-Benutzern die Notwendigkeit von Beiträgen und Erwartungen an Beitragende. Sie werden kollektiv als Asset-Anforderungen bezeichnet.



**Frage. Kann ich Assets in einen beliebigen zulässigen Ordner hochladen?**

**Antwort.** Nicht in alle zulässigen Ordner. Ein Brand Portal-Benutzer kann Inhalte nur in den **Beitragsordner** hochladen, der vom AEM- oder Brand Portal-Administrator freigegeben wird.



**Frage. Wie erhalte ich Zugriff auf einen Beitragsordner?**

**Antwort.** Sie können nur dann auf einen **Beitragsordner** zugreifen, wenn dieser für Sie freigegeben wurde. Sie erhalten eine E-Mail-/Pulsbenachrichtigung, sobald ein Beitragsordner für Sie freigegeben wurde. Sie können entweder über den Link in der E-Mail auf den Beitragsordner zugreifen oder sich bei Ihrer Brand Portal-Instanz anmelden und zum Glockensymbol für die Benachrichtigung navigieren, um auf den Beitragsordner zuzugreifen.

>[!NOTE]
>
>Wenn Sie kein bestehender Brand Portal-Benutzer sind, bitten Sie den AEM-Administrator, ein Benutzerkonto in AEM Admin Console zu erstellen und Ihr Profil zur Benutzerkonfigurationsdatei in der Brand Portal-Benutzerliste hinzuzufügen. Weitere Informationen finden Sie unter [Hinzufügen von Brand Portal-Benutzern](brand-portal-configure-asset-sourcing.md).

**Frage. Welches Format hat die CSV-Datei für den Benutzerimport?**

**Antwort.** Das Format entspricht dem von Admin Console für den Massenimport von Benutzern unterstützten Format. E-Mail-Adresse, Vorname und Nachname sind obligatorisch.



**Frage. Wie wird die Liste der Benutzer (Brand Portal-Beitragende) in der Dropdown-Liste &quot;Asset-Beitrag-Benutzer&quot; gefüllt?**

**Antwort.** Die Benutzer in der Dropdown-Liste werden aus der in AEM hochgeladenen Datei für die Brand Portal-Benutzerkonfiguration (.CSV) gefüllt.



**Frage. Wo kann ich den Status von Import- und Veröffentlichungsaufträgen sehen?**

**Antwort.** In AEM können Sie den Status eines Imports auf einer **asynchronen** Auftragsseite sehen. In Brand Portal können Sie den Status eines Veröffentlichungsauftrags unter **[!UICONTROL Tools > Asset-Beitragsstatus]** anzeigen.



**Frage. Wie häufig wird ein Importauftrag ausgeführt, der regelmäßig in AEM ausgeführt wird?**

**Antwort.** In AEM wird die Abfrage alle fünf Minuten ausgeführt.



**Frage. Gibt es einen Schwellenwert dafür, wie oft ein Ordner von Brand Portal in AEM Assets veröffentlicht werden kann?**

**Antwort.** Nein, alle Assets im Ordner **NEU** werden unabhängig davon, ob sie zuvor veröffentlicht wurden, in AEM Assets veröffentlicht. Jedes Mal, wenn ein **Beitragsordner** von Brand Portal in AEM Assets veröffentlicht wird, überschreibt er den Inhalt des Ordners **NEU**.



**Frage. Wie werden neue Assets in einen Beitragsordner hochgeladen?**

**Antwort.** Lesen Sie die detaillierte Dokumentation zum [Hochladen von Assets in den Beitragsordner](brand-portal-upload-assets-to-contribution-folder.md).



**Frage. Warum sehe ich keine Miniaturansichten/Vorschauen zu den Assets, die von einem Brand Portal-Benutzer in den Ordner NEU hochgeladen wurden?**

**Antwort.** Das ist normal, da auf der Brand Portal-Seite kein Workflow ausgeführt wird.



**Frage. Was passiert, wenn ein Ordner von AEM Assets an Brand Portal veröffentlicht wird, das sich im Fluss befindet?**

**Antwort.** In AEM werden Protokolle für jedes Mal aufgezeichnet, wenn ein Ordner in Brand Portal veröffentlicht wird. Zum Zeitpunkt der Veröffentlichung werden alle Assets, die nicht in Brand Portal veröffentlicht werden, in eine Replikationswarteschlange gestellt. Assets, die nach dem Auslösen des Veröffentlichungsauftrags zum Ordner hinzugefügt wurden, werden nicht in Brand Portal veröffentlicht. Wenn der AEM-Benutzer den Ordner erneut veröffentlicht, werden nur die zuvor noch nicht veröffentlichten (und in der Replikationswarteschlange vorhandenen) Assets in Brand Portal veröffentlicht.
Dies gilt für alle Ordner, die von AEM Assets in Brand Portal veröffentlicht werden, und für den Ordner FREIGEGEBEN in einem Beitragsordner.



**Frage. An wen kann ich mich bei Fragen wenden?**

**Antwort.** Kontaktieren Sie Ihren Adobe-Kundenbetreuer oder den Kundensupport.


>[!NOTE]
>
>Der Veröffentlichungszeitplan ist vorläufig und kann jederzeit geändert werden. Wenden Sie sich an Ihren Adobe-Kundenbetreuer oder den Kundensupport, um aktuelle Informationen zum Veröffentlichungszeitplan zu erhalten.





## Produktzugriff und Support (Websites mit Zugriffsbeschränkung) {#product-access-and-support-restricted-sites}

Diese Sites sind nur für Kunden verfügbar. Wenn Sie Kunde sind und Zugriff benötigen, wenden Sie sich an Ihren Adobe-Kundenbetreuer.

* [](https://daycare.day.com) [Produktzugriff](https://login.marketing.adobe.com)

* [Adobe-Kundenunterstützung](https://helpx.adobe.com/de/contact.html)
