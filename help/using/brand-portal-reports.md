---
title: Arbeiten mit Berichten
seo-title: Arbeiten mit Berichten
description: AEM Assets Brand Portal-Administratoren können Berichte zur Brand Portal-Nutzung anzeigen und Berichte erstellen, verwalten und anzeigen, die Informationen zu heruntergeladenen, abgelaufenen und veröffentlichten Assets sowie über Brand Portal freigegebene Links enthalten.
seo-description: AEM Assets Brand Portal-Administratoren können Berichte zur Brand Portal-Nutzung anzeigen und Berichte erstellen, verwalten und anzeigen, die Informationen zu heruntergeladenen, abgelaufenen und veröffentlichten Assets sowie über Brand Portal freigegebene Links enthalten.
uuid: dc 4 e 5275-a 614-4 b 95-8 c 70-2 b 7 e 470 c 50 a 7
content-type: Referenz
topic-tags: Administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 7683074 f-b 6 ea -42 e 0-a 411-3 b 13 eb 88 d 1 f 2
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Arbeiten mit Berichten {#work-with-reports}

Die Berichterstellungsfunktion ist hilfreich, um die Markenportal-Nutzung zu bewerten und zu wissen, wie interne und externe Benutzer mit genehmigten Assets interagieren. Administratoren können den Brand Portal-Verwendungsbericht anzeigen, der immer auf der Seite „Asset-Berichte“ verfügbar ist. Auch Berichte über Benutzeranmeldungen und heruntergeladene, abgelaufene, veröffentlichte und über Links freigegebene Assets können erzeugt und auf der Seite „Asset-Berichte“ angezeigt werden. Diese Berichte sind bei der Analyse der Asset-Bereitstellung hilfreich, wodurch Sie wichtige Erfolgsmetriken ableiten können, um die Akzeptanz genehmigter Assets innerhalb und außerhalb Ihres Unternehmens zu messen.

Die Berichtverwaltungsoberfläche ist intuitiv und enthält detaillierte Optionen und Steuerungen, mit denen Sie auf gespeicherte Berichte zugreifen können. Über die Seite „Asset-Berichte“, auf der alle bisher erstellten Berichte aufgelistet werden, können Sie Berichte anzeigen, herunterladen oder löschen.

## Anzeigen von Berichten {#view-reports}

Gehen Sie wie folgt vor, um einen Bericht anzuzeigen:

1. Tippen bzw. klicken Sie oben in der Symbolleiste auf das AEM-Logo, um auf die Admin Tools zuzugreifen.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **[!UICONTROL Create/Manage Reports]** to open **[!UICONTROL Asset Reports]** page.

   ![](assets/access-asset-reports.png)

3. Access **[!UICONTROL Usage]** report and other generated reports from Asset Reports page.

   >[!NOTE]
   >
   >Der Verwendungsbericht ist in Brand Portal standardmäßig vorhanden. Er kann nicht erstellt oder gelöscht werden. Sie können jedoch die Berichte "Download" ," Ablaufdatum" , "Veröffentlichen" ," Link-Freigabe" und "Benutzeranmeldungen" erstellen, herunterladen und löschen.

   Um einen Bericht anzuzeigen, tippen/klicken Sie auf den Link zum Bericht. Wählen Sie alternativ den Bericht aus und tippen/klicken Sie in der Symbolleiste auf das Symbol Ansicht.

   Der [!UICONTROL Verwendungsbericht] zeigt Informationen zur Anzahl der aktuellen Brand Portal-Benutzer, den von allen Assets belegten Speicherplatz sowie die Gesamtzahl der Assets in Brand Portal an. Der Bericht zeigt außerdem die zulässige Kapazität für jede dieser Informationsmetriken an.

   ![](assets/usage-report.png)

   Der Bericht [!UICONTROL Benutzeranmeldungen] bietet Informationen zu Benutzern, die sich beim Portal angemeldet haben. Der Bericht zeigt Anzeigenamen, E-Email-IDs, Mitarbeiter (Admin, Viewer, Editor, Gast), Gruppen, letzte Anmeldung, Aktivitätsstatus und Anmeldungsanzahl der einzelnen Benutzer aus der Markenoberfläche von Brand Portal 6.4.2 bis zum Zeitpunkt der Berichterstellung an.

   ![](assets/user-logins.png)

   Der Bericht [!UICONTROL Download] listet alle Assets auf und zeigt Details zu allen Assets an, die in einem bestimmten Zeitraum heruntergeladen wurden.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >The assets [!UICONTROL Download] report displays only the assets that were individually selected and downloaded from Brand Portal. Wenn ein Benutzer einen Ordner heruntergeladen hat, der Assets enthält, zeigt der Bericht den Ordner oder die Assets im Ordner nicht an.

   Der Bericht [!UICONTROL Ablauf] zeigt alle Assets (inklusive Details) an, die in einem bestimmten Zeitraum abgelaufen sind.

   ![](assets/expiration-report.png)

   Der Bericht [!UICONTROL Veröffentlichen] zeigt Informationen zu allen Assets an, die in einem bestimmten Zeitraum von AEM in Brand Portal veröffentlicht wurden.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Der Bericht „Veröffentlichen“ zeigt keine Informationen zu Inhaltsfragmenten an, da diese nicht in Brand Portal veröffentlicht werden können.

   Der Bericht zur [!UICONTROL Linkfreigabe listet alle Assets auf, die über Links von der Brand Portal-Benutzeroberfläche aus in einem bestimmten Zeitrahmen freigegeben wurden. ] Der Bericht informiert darüber hinaus, wann das Asset über einen Link geteilt wurde, vom Benutzer, wann der Link abläuft, und die Anzahl der freigegebenen Links für den Mandanten (und Benutzer, für die der Asset-Link freigegeben wurde). Die Spalten im Bericht zur Linkfreigabe können nicht angepasst werden.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Der Bericht zur Linkfreigabe zeigt keine Benutzer an, die Zugriff auf das über den Link freigegebene Asset haben oder die das Asset über den Link heruntergeladen haben.
   >
   >
   >Zum Nachverfolgen von Downloads über den freigegebenen Link müssen Sie den Bericht „Download“ nach der Auswahl der Option **[!UICONTROL Nur Downloads über Link-Freigabe]** auf der Seite **Bericht erstellen]erstellen.[!UICONTROL ** In diesem Fall ist der Benutzer (Heruntergeladen von) in diesem Fall anonym.

## Erstellen von Berichten {#generate-reports}

Administrators can generate and manage the following standard reports, once generated, they are saved to be [accessed](../using/brand-portal-reports.md#main-pars-header) later:

* Benutzeranmeldungen
* Download
* Ablauf
* Veröffentlichen
* Linkfreigabe

Die Spalten in den Berichten „Download“, „Ablauf“ und „Veröffentlichen“ können für die Anzeige angepasst werden. Gehen Sie wie folgt vor, um einen Bericht zu generieren:

1. Tippen/klicken Sie oben in der Symbolleiste auf das AEM-Logo, um auf die Admin Tools zuzugreifen.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, tap/click **[!UICONTROL Create/Manage Reports]** to open **Asset Reports **page.

   ![](assets/asset-reports.png)

3. Tippen/klicken Sie auf der Seite Asset-Berichte auf **[!UICONTROL Erstellen]**.
4. From the **[!UICONTROL Create Report]** page, select a report to create, and tap/click **[!UICONTROL Next]**.

   ![](assets/crete-report.png)

5. Konfigurieren Sie die Berichtdetails. Geben Sie den Titel, die Beschreibung, die Ordnerstruktur (wo soll der Bericht ausgeführt und welche Statistiken sollen generiert werden) und den Datumsbereich für die Berichte [!UICONTROL Download], [!UICONTROL Ablauf] und [!UICONTROL Veröffentlichen] an.

   ![](assets/create-report-page.png)

   Whereas, [!UICONTROL Link Share Report] only needs the title, description, and date range parameters.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Sonderzeichen # und % im Berichttitel werden durch einen Bindestrich (-) in der Berichtgenerierung ersetzt.

6. Tap/click **[!UICONTROL Next]**, to configure the columns of Download, Expiration, and Publish reports.
7. Aktivieren oder deaktivieren Sie dazu die entsprechenden Kontrollkästchen. For example, to view names of users (who downloaded assets) in [!UICONTROL Download] report, select **[!UICONTROL Downloaded By]**. Die folgende Abbildung veranschaulicht die Auswahl von Standardspalten im Bericht „Download“.

   ![](assets/createdownloadreport.png)

   Sie können einem Bericht auch benutzerdefinierte Spalten hinzufügen, um weitere Daten für Ihre individuellen Anforderungen anzuzeigen.

   Gehen Sie wie folgt vor, um benutzerdefinierte Spalten in den Berichten „Download“, „Veröffentlichen“ oder „Ablauf“ hinzuzufügen :

   1. To display a custom column, tap/click **[!UICONTROL Add]** within [!UICONTROL Custom Columns].
   2. Specify name of the column in **[!UICONTROL Column Name]** field.
   3. Wählen Sie die Eigenschaftsauswahl, um auszuwählen, welche Eigenschaft der Spalte zugewiesen werden soll.

      ![](assets/property-picker.png)
Alternativ können Sie den Pfad im Feld „Eigenschaftspfad“ eingeben.

      ![](assets/property-path.png)

      Tippen/klicken Sie auf **Hinzufügen** und wiederholen Sie die Schritte 2 und 3, um weitere benutzerdefinierte Spalten hinzuzufügen.

8. Tippen/klicken Sie auf **[!UICONTROL Erstellen]**. Eine Meldung benachrichtigt Sie darüber, dass die Berichtserstellung startet.

## Herunterladen von Berichten {#download-reports}

Führen Sie einen der folgenden Schritte aus, um einen Bericht zu speichern und als CSV-Datei herunterzuladen:

* Select a report on Asset Reports page, and tap/click **[!UICONTROL Download]** from the toolbar at the top.

![](assets/download-asset-report.png)

* Öffnen Sie auf der Seite „Asset-Berichte“ einen Bericht. Select **[!UICONTROL Download]** option from the top of the report page.

![](assets/download-report-fromwithin.png)

## Löschen von Berichten {#delete-reports}

Zum Löschen eines vorhandenen Berichts müssen Sie den Bericht auf der Seite **[!UICONTROL Asset-Berichte]** auswählen und dann in der Symbolleiste am oberen Rand auf **Löschen[!UICONTROL tippen bzw. klicken.]**

>[!NOTE]
>
>Der [!UICONTROL Verwendungsbericht] kann nicht gelöscht werden.
