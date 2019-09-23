---
title: Arbeiten mit Berichten
seo-title: Arbeiten mit Berichten
description: AEM Assets Brand Portal-Administratoren können Berichte zur Brand Portal-Nutzung anzeigen und Berichte erstellen, verwalten und anzeigen, die Informationen zu heruntergeladenen, abgelaufenen und veröffentlichten Assets sowie über Brand Portal freigegebene Links enthalten.
seo-description: AEM Assets Brand Portal-Administratoren können Berichte zur Brand Portal-Nutzung anzeigen und Berichte erstellen, verwalten und anzeigen, die Informationen zu heruntergeladenen, abgelaufenen und veröffentlichten Assets sowie über Brand Portal freigegebene Links enthalten.
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: Referenz
topic-tags: Administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Arbeiten mit Berichten {#work-with-reports}

The reporting capability is instrumental in assessing Brand Portal usage, and knowing how internal and external users interact with approved assets. Administratoren können den Brand Portal-Verwendungsbericht anzeigen, der immer auf der Seite „Asset-Berichte“ verfügbar ist. Auch Berichte über Benutzeranmeldungen und heruntergeladene, abgelaufene, veröffentlichte und über Links freigegebene Assets können erzeugt und auf der Seite „Asset-Berichte“ angezeigt werden. Diese Berichte sind hilfreich bei der Analyse der Ressourcenbereitstellung, mit deren Hilfe Sie wichtige Erfolgsmetriken ableiten können, um die Akzeptanz genehmigter Ressourcen innerhalb und außerhalb Ihrer Organisation zu messen.

Die Berichtverwaltungsoberfläche ist intuitiv und enthält detaillierte Optionen und Steuerungen, mit denen Sie auf gespeicherte Berichte zugreifen können. Über die Seite „Asset-Berichte“, auf der alle bisher erstellten Berichte aufgelistet werden, können Sie Berichte anzeigen, herunterladen oder löschen.

## Anzeigen von Berichten {#view-reports}

Gehen Sie wie folgt vor, um einen Bericht anzuzeigen:

1. Tippen bzw. klicken Sie oben in der Symbolleiste auf das AEM-Logo, um auf die Admin Tools zuzugreifen.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **[!UICONTROL Create/Manage Reports]** to open **[!UICONTROL Asset Reports]** page.

   ![](assets/access-asset-reports.png)

3. Greifen Sie auf den **[!UICONTROL Nutzungsbericht]und andere generierte Berichte von der Seite „Asset-Berichte“ aus zu.**

   >[!NOTE]
   >
   >Der Verwendungsbericht ist in Brand Portal standardmäßig vorhanden. Er kann nicht erstellt oder gelöscht werden. Sie können jedoch Berichte zu Downloads, Ablaufdaten, Veröffentlichungen, Linkfreigaben und Benutzeranmeldungen erstellen, herunterladen und löschen.

   Um einen Bericht anzuzeigen, tippen/klicken Sie auf den Link zum Bericht. Alternativ wählen Sie den Bericht aus und tippen/klicken Sie in der Symbolleiste auf das Symbol „Anzeigen“.

   Der [!UICONTROL Verwendungsbericht] zeigt Informationen zur Anzahl der aktuellen Brand Portal-Benutzer, den von allen Assets belegten Speicherplatz sowie die Gesamtzahl der Assets in Brand Portal an. Der Bericht zeigt außerdem die zulässige Kapazität für jede dieser Informationsmetriken an.

   ![](assets/usage-report.png)

   Der Bericht [!UICONTROL Benutzeranmeldungen] bietet Informationen zu Benutzern, die sich beim Portal angemeldet haben. Der Bericht zeigt Anzeigenamen, E-Mail-IDs, Personas (Admin, Viewer, Editor, Gast), Gruppen, die letzte Anmeldung, den Aktivitätsstatus und die Anzahl der Anmeldungen der einzelnen Benutzer von der Bereitstellung des Markenportals 6.4.2 bis zum Zeitpunkt der Berichterstellung an.

   ![](assets/user-logins.png)

   Der Bericht [!UICONTROL Download] listet alle Assets auf und zeigt Details zu allen Assets an, die in einem bestimmten Zeitraum heruntergeladen wurden.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >The assets [!UICONTROL Download] report displays only the assets that were individually selected and downloaded from Brand Portal. Wenn ein Benutzer einen Ordner mit Assets heruntergeladen hat, werden der Ordner bzw. die Assets im Ordner nicht im Bericht angezeigt.

   Der Bericht [!UICONTROL Ablauf] zeigt alle Assets (inklusive Details) an, die in einem bestimmten Zeitraum abgelaufen sind.

   ![](assets/expiration-report.png)

   Der Bericht [!UICONTROL Veröffentlichen] zeigt Informationen zu allen Assets an, die in einem bestimmten Zeitraum von AEM in Brand Portal veröffentlicht wurden.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Der Bericht „Veröffentlichen“ zeigt keine Informationen zu Inhaltsfragmenten an, da diese nicht in Brand Portal veröffentlicht werden können.

   Der Bericht zur [!UICONTROL Linkfreigabe listet alle Assets auf, die über Links von der Brand Portal-Benutzeroberfläche aus in einem bestimmten Zeitrahmen freigegeben wurden. ] Der Bericht beinhaltet auch Informationen, wann und von welchem Benutzer das Asset über den Link freigegeben wurde und wann der Link abläuft, sowie Angaben zur Anzahl freigegebener Links für den Mandanten (und Benutzer, für die der Asset-Link freigegeben wurde). Die Spalten im Bericht zur Linkfreigabe können nicht angepasst werden.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Der Bericht zur Linkfreigabe zeigt keine Benutzer an, die Zugriff auf das über den Link freigegebene Asset haben oder die das Asset über den Link heruntergeladen haben.
   >
   >
   >Zum Nachverfolgen von Downloads über den freigegebenen Link müssen Sie den Bericht „Download“ nach der Auswahl der Option **[!UICONTROL Nur Downloads über Link-Freigabe]** auf der Seite **Bericht erstellen]erstellen.[!UICONTROL ** Der Benutzer (heruntergeladen von) ist in diesem Fall jedoch anonym.

## Erstellen von Berichten {#generate-reports}

Administratoren können die folgenden Standardberichte generieren und verwalten. Sobald sie generiert wurden, werden sie zur späteren Verwendung [zugänglich](../using/brand-portal-reports.md#main-pars-header) gespeichert:

* Benutzeranmeldungen
* Download
* Ablauf
* Veröffentlichen
* Linkfreigabe

Die Spalten in den Berichten „Download“, „Ablauf“ und „Veröffentlichen“ können für die Anzeige angepasst werden. Gehen Sie wie folgt vor, um einen Bericht zu generieren:

1. Tippen/klicken Sie oben in der Symbolleiste auf das AEM-Logo, um auf die Admin Tools zuzugreifen.

   ![](assets/aemlogo.png)

2. Tippen/klicken Sie im Admin Tools-Bereich auf **[!UICONTROL Berichte erstellen/verwalten], um die Seite „Asset-Berichte“ zu öffnen.**

   ![](assets/asset-reports.png)

3. Tippen/klicken Sie auf der Seite „Asset-Berichte“ auf **[!UICONTROL Erstellen]**.
4. Wählen Sie auf der Seite **[!UICONTROL Bericht erstellen]** den Bericht aus, den Sie erstellen möchten, und tippen/klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/crete-report.png)

5. Konfigurieren Sie die Berichtdetails. Geben Sie den Titel, die Beschreibung, die Ordnerstruktur (wo soll der Bericht ausgeführt und welche Statistiken sollen generiert werden) und den Datumsbereich für die Berichte [!UICONTROL Download], [!UICONTROL Ablauf] und [!UICONTROL Veröffentlichen] an.

   ![](assets/create-report-page.png)

   Für den [!UICONTROL Bericht zur Linkfreigabe] müssen nur die Parameter für den Titel, die Beschreibung und den Datumsbereich festgelegt werden.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Die Sonderzeichen # und % im Berichtstitel werden bei der Berichtserstellung durch einen Bindestrich (-) ersetzt.

6. Tap/click **[!UICONTROL Next]**, to configure the columns of Download, Expiration, and Publish reports.
7. Aktivieren oder deaktivieren Sie dazu die entsprechenden Kontrollkästchen. For example, to view names of users (who downloaded assets) in [!UICONTROL Download] report, select **[!UICONTROL Downloaded By]**. Die folgende Abbildung veranschaulicht die Auswahl von Standardspalten im Bericht „Download“.

   ![](assets/createdownloadreport.png)

   Sie können einem Bericht auch benutzerdefinierte Spalten hinzufügen, um weitere Daten für Ihre individuellen Anforderungen anzuzeigen.

   Gehen Sie wie folgt vor, um benutzerdefinierte Spalten in den Berichten „Download“, „Veröffentlichen“ oder „Ablauf“ hinzuzufügen :

   1. Um eine benutzerdefinierte Spalte anzuzeigen, tippen/klicken Sie auf **[!UICONTROL Hinzufügen]** innerhalb von [!UICONTROL Benutzerdefinierte Spalten].
   2. Geben Sie im Feld **[!UICONTROL Spaltenname]den Namen der Spalte ein.**
   3. Wählen Sie die Eigenschaftsauswahl, um auszuwählen, welche Eigenschaft der Spalte zugewiesen werden soll.

      ![](assets/property-picker.png)
Alternativ können Sie den Pfad im Feld „Eigenschaftspfad“ eingeben.

      ![](assets/property-path.png)

      Tippen/klicken Sie auf **Hinzufügen** und wiederholen Sie die Schritte 2 und 3, um weitere benutzerdefinierte Spalten hinzuzufügen.

8. Tippen/klicken Sie auf **[!UICONTROL Erstellen]**. Eine Meldung benachrichtigt Sie darüber, dass die Berichtserstellung startet.

## Herunterladen von Berichten {#download-reports}

Führen Sie einen der folgenden Schritte aus, um einen Bericht zu speichern und als CSV-Datei herunterzuladen:

* Wählen Sie auf der Seite „Asset-Berichte“ einen Bericht aus und tippen/klicken Sie oben in der Symbolleiste auf **[!UICONTROL Download].**

![](assets/download-asset-report.png)

* Öffnen Sie auf der Seite „Asset-Berichte“ einen Bericht. Wählen Sie oben auf der Berichtseite die Option **[!UICONTROL Download].**

![](assets/download-report-fromwithin.png)

## Löschen von Berichten {#delete-reports}

Zum Löschen eines vorhandenen Berichts müssen Sie den Bericht auf der Seite **[!UICONTROL Asset-Berichte]** auswählen und dann in der Symbolleiste am oberen Rand auf **Löschen]tippen bzw. klicken.[!UICONTROL **

>[!NOTE]
>
>Der Bericht [!UICONTROL Verwendung] kann nicht gelöscht werden.
