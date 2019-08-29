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
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Arbeiten mit Berichten {#work-with-reports}

The reporting capability is instrumental in assessing [!DNL Brand Portal] usage, and knowing how internal and external users interact with approved assets. Administrators can view [!DNL Brand Portal] Usage report, which is always available on Asset Reports page. Auch Berichte über Benutzeranmeldungen und heruntergeladene, abgelaufene, veröffentlichte und über Links freigegebene Assets können erzeugt und auf der Seite „Asset-Berichte“ angezeigt werden. Diese Berichte sind bei der Analyse der Asset-Bereitstellung hilfreich, wodurch Sie wichtige Erfolgsmetriken ableiten können, um die Akzeptanz genehmigter Assets innerhalb und außerhalb Ihres Unternehmens zu messen.

Die Berichtverwaltungsoberfläche ist intuitiv und enthält detaillierte Optionen und Steuerungen, mit denen Sie auf gespeicherte Berichte zugreifen können. Über die Seite „Asset-Berichte“, auf der alle bisher erstellten Berichte aufgelistet werden, können Sie Berichte anzeigen, herunterladen oder löschen.

## Anzeigen von Berichten {#view-reports}

Gehen Sie wie folgt vor, um einen Bericht anzuzeigen:

1. From the toolbar at the top, tap/click the [!DNL AEM] logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Create/Manage Reports** to open **Asset Reports **page.

   ![](assets/access-asset-reports.png)

3. Access **Usage** report and other generated reports from Asset Reports page.

   >[!NOTE]
   >
   >Usage report is present by default in [!DNL Brand Portal]. Er kann nicht erstellt oder gelöscht werden. Sie können jedoch die Berichte "Download" ," Ablaufdatum" , "Veröffentlichen" ," Link-Freigabe" und "Benutzeranmeldungen" erstellen, herunterladen und löschen.

   Um einen Bericht anzuzeigen, tippen/klicken Sie auf den Link zum Bericht. Wählen Sie alternativ den Bericht aus und tippen/klicken Sie in der Symbolleiste auf das Symbol Ansicht.

   **Der Nutzungsbericht** zeigt Informationen über die Anzahl der aktuellen [!DNL Brand Portal] Benutzer, den von allen Assets belegten Speicherplatz und die Gesamtzahl der Assets in an [!DNL Brand Portal]. Der Bericht zeigt außerdem die zulässige Kapazität für jede dieser Informationsmetriken an.

   ![](assets/usage-report.png)

   **Der** Bericht zu Benutzeranmeldungen enthält Informationen über die Benutzer, die sich angemeldet [!DNL Brand Portal]haben. The report shows display names, email IDs, personas (admin, viewer, editor, guest), groups, last login, activity status, and login count of each user from [!DNL Brand Portal] 6.4.2 deployment until the time of report generation.

   ![](assets/user-logins.png)

   Der Bericht **Download** listet alle Assets auf und zeigt Details zu allen Assets an, die in einem bestimmten Zeitraum heruntergeladen wurden.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >The assets** Download** report displays only the assets that were individually selected and downloaded from [!DNL Brand Portal]. Wenn ein Benutzer einen Ordner heruntergeladen hat, der Assets enthält, zeigt der Bericht den Ordner oder die Assets im Ordner nicht an.

   Der Bericht **Ablauf** zeigt alle Assets (inklusive Details) an, die in einem bestimmten Zeitraum abgelaufen sind.

   ![](assets/expiration-report.png)

   Der Bericht **Veröffentlichen**[!DNL AEM] zeigt Informationen zu allen Assets an, die in einem bestimmten Zeitraum von in veröffentlicht wurden.[!DNL Brand Portal]

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Publish Report does not display information about content fragments, as the content fragments cannot be published to the [!DNL Brand Portal].

   **Link-Freigabebericht** listet alle Assets auf, die über Links aus der [!DNL Brand Portal] Schnittstelle in einem bestimmten Zeitraum freigegeben wurden. Der Bericht informiert darüber hinaus, wann das Asset über einen Link geteilt wurde, vom Benutzer, wann der Link abläuft, und die Anzahl der freigegebenen Links für den Mandanten (und Benutzer, für die der Asset-Link freigegeben wurde). Die Spalten im Bericht zur Linkfreigabe können nicht angepasst werden.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Der Bericht zur Linkfreigabe zeigt keine Benutzer an, die Zugriff auf das über den Link freigegebene Asset haben oder die das Asset über den Link heruntergeladen haben.
   >
   >
   >Zum Nachverfolgen von Downloads über den freigegebenen Link müssen Sie den Bericht „Download“ nach der Auswahl der Option **Nur Downloads über Link-Freigabe** auf der Seite **Bericht erstellen** erstellen. In diesem Fall ist der Benutzer (Heruntergeladen von) in diesem Fall anonym.

## Erstellen von Berichten {#generate-reports}

Administrators can generate and manage the following standard reports, once generated, they are saved to be [accessed](../using/brand-portal-reports.md#main-pars-header) later:

* Benutzeranmeldungen
* Download
* Ablauf
* Veröffentlichen
* Linkfreigabe

Die Spalten in den Berichten „Download“, „Ablauf“ und „Veröffentlichen“ können für die Anzeige angepasst werden. Gehen Sie wie folgt vor, um einen Bericht zu generieren:

1. From toolbar at the top, tap/click the [!DNL AEM] logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, tap/click **Create/Manage Reports** to open **Asset Reports **page.

   ![](assets/asset-reports.png)

3. Tippen/klicken Sie auf der Seite Asset-Berichte auf **Erstellen**.
4. From the **Create Report** page, select a report to create, and tap/click **Next**.

   ![](assets/crete-report.png)

5. Konfigurieren Sie die Berichtdetails. Geben Sie den Titel, die Beschreibung, die Ordnerstruktur (wo soll der Bericht ausgeführt und welche Statistiken sollen generiert werden) und den Datumsbereich für die Berichte **Download**, **Ablauf** und **Veröffentlichen** an.

   ![](assets/create-report-page.png)

   Whereas, **Link Share Report** only needs the title, description, and date range parameters.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Sonderzeichen # und % im Berichttitel werden durch einen Bindestrich (-) in der Berichtgenerierung ersetzt.

6. Tap/click **Next**, to configure the columns of Download, Expiration, and Publish reports.
7. Aktivieren oder deaktivieren Sie dazu die entsprechenden Kontrollkästchen. For example, to view names of users (who downloaded assets) in **Download** report, select **Downloaded By**. Die folgende Abbildung veranschaulicht die Auswahl von Standardspalten im Bericht „Download“.

   ![](assets/createdownloadreport.png)

   Sie können einem Bericht auch benutzerdefinierte Spalten hinzufügen, um weitere Daten für Ihre individuellen Anforderungen anzuzeigen.

   Gehen Sie wie folgt vor, um benutzerdefinierte Spalten in den Berichten „Download“, „Veröffentlichen“ oder „Ablauf“ hinzuzufügen :

   1. To display a custom column, tap/click **Add** within **Custom Columns**.
   2. Specify name of the column in **Column Name** field.
   3. Wählen Sie die Eigenschaftsauswahl, um auszuwählen, welche Eigenschaft der Spalte zugewiesen werden soll.

      ![](assets/property-picker.png)
Alternativ können Sie den Pfad im Feld „Eigenschaftspfad“ eingeben.

      ![](assets/property-path.png)

      Tippen/klicken Sie auf **Hinzufügen** und wiederholen Sie die Schritte 2 und 3, um weitere benutzerdefinierte Spalten hinzuzufügen.

8. Tippen/klicken Sie auf **Erstellen**. Eine Meldung benachrichtigt Sie darüber, dass die Berichtserstellung startet.

## Herunterladen von Berichten {#download-reports}

Führen Sie einen der folgenden Schritte aus, um einen Bericht zu speichern und als CSV-Datei herunterzuladen:

* Select a report on Asset Reports page, and tap/click **Download** from the toolbar at the top.

![](assets/download-asset-report.png)

* Öffnen Sie auf der Seite „Asset-Berichte“ einen Bericht. Select **Download** option from the top of the report page.

![](assets/download-report-fromwithin.png)

## Löschen von Berichten {#delete-reports}

Zum Löschen eines vorhandenen Berichts müssen Sie den Bericht auf der Seite **Asset-Berichte** auswählen und dann in der Symbolleiste am oberen Rand auf **Löschen** tippen bzw. klicken.

>[!NOTE]
>
>Der **Verwendungsbericht** kann nicht gelöscht werden.
