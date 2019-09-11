---
title: Schnellere Downloads von Markenportalen
seo-title: Schnellere Downloads von Markenportalen
description: Verkürzen Sie die Download-Zeiten von Brand Portal und freigegebenen Links.
seo-description: Verkürzen Sie die Download-Zeiten von Brand Portal und freigegebenen Links.
uuid: 2871137 e -6471-49 a 7-872 a -841 bd 92543 d 1
contentOwner: mgulati
topic-tags: download-install
content-type: Referenz
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 301 f 7 a 0 b -5527-4 aac-b 731-bfc 145 fed 0 c 0
translation-type: tm+mt
source-git-commit: fb8243ea896d39b324a69ea534271ee3015c076f

---


# Schnellere Downloads von Markenportalen {#guide-to-accelerate-downloads-from-brand-portal}

Mit dem Markenportal können Sie die Download-Leistung großer Asset-Dateien verbessern, indem Sie die Integration mit IBM Aspera Connect durchführen, was eine Installationsanwendung ist. Die Anwendung verwendet proprietäre Technologie, um TCP-Overhead zu entfernen und die Übertragungsgeschwindigkeit der Asset-Dateien zu verbessern. Diese Integration gewährleistet eine verbesserte Download-Erfahrung.

>[!NOTE]
>
>Die Downloadgeschwindigkeit variiert für Benutzer je nach Faktoren wie Netzwerkbandbreite, Serverlatenz und geografischer Standort der Kunden.

Ist diese Option aktiviert, können Brand Portal-Benutzer die zum Herunterladen der gewünschten Asset-Dateien von Brand Portal oder über freigegebene Links benötigte Zeit durch die Installation des Aspera Connect-Clients erheblich verkürzen.

![](assets/enable-fast-file-download.png)

## Voraussetzungen für die Beschleunigung des Datei-Downloads {#prerequisites-to-accelerate-file-download}

Um die Dateien schneller herunterzuladen, stellen Sie Folgendes sicher:

* **[!UICONTROL Aktivieren Sie die Option Download-Beschleunigung]** (standardmäßig deaktiviert) aus [!UICONTROL allgemeinen Einstellungen] im Verwaltungswerkzeug-Bedienfeld.
* Port 33001 (TCP und UDP) ist auf der Firewall geöffnet. Weitere Informationen zu den Voraussetzungen finden Sie in der [Dokumentation zu Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8).
* Installieren Sie Aspera Connect mit Administratorrechten.
* For platform support of Aspera transfer client, see [Aspera Connect platform support matrix](https://www.asperasoft.com/company/support/transfer-clients/).

## Download-Domänen {#download-domains}

Nachfolgend sind die Download-Domänen für verschiedene geografische Standorte aufgeführt:

| Regionscodes | Domäne |
|---|---|
| NA OR1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## Sample download performance using file accelerator {#expected-download-performance-using-file-accelerator}

Die folgende Tabelle zeigt die Downloadleistung für 2 GB-Datei mit dem Aspera Connect-Dateidownload-Beschleuniger:

**Die beobachteten Ergebnisse variieren je nach Faktoren wie Netzwerkbandbreite, Serverlatenz und Kundenstandort, wobei sich der Markenportal-Server unter Oregon (USA) befindet.*

| Client-Standort | Latenzzeit zwischen Client und Server (Millisekunden) | Geschwindigkeit mit Aspera Connect File Transfer Accelerator (mbps) | Zeit zum Herunterladen von 2 GB Datei mit Aspera File Transfer Accelerator (Sekunden) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| USA, Westen (Nordkalifornien) | 18 | 36 | 57 |
| USA, Westen (Oregon) | 42 | 36 | 57 |
| USA, Osten (Nordvirginia) | 85 | 35 | 58 |
| APAC (Tokio) | 124 | 36 | 57 |
| Noida (Indien) | 275 | 13.36 | 153 |
| Sydney | 175 | 29 | 70 |
| London | 179 | 35 | 58 |
| Singapur | 196 | 34 | 60 |

## Download-Workflow mit dem Dateibeschleuniger {#download-workflow-using-file-accelerator}

So laden Sie Assets schneller von Brand Portal herunter:

1. Melden Sie sich mit einem unterstützten Browser bei Brand Portal an.
2. Suchen Sie nach der gewünschten Asset-Datei oder Sammlung bzw. dem gewünschten Ordner, die bzw. der heruntergeladen werden soll, und wählen Sie diese bzw. diesen aus. Tippen bzw. klicken Sie auf die Option „Herunterladen“.
Download dialog appears with [Enable download acceleration] option selected.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >Die Funktion zum Senden von E-Mail-Benachrichtigungen mit dem Link zum Herunterladen von Assets wird derzeit nicht unterstützt, während schnellere Downloads aktiviert sind.

   ![](assets/fast-download-emailchk.png)

3. Tap/click the **[!UICONTROL Download]** option.
Um die Download-Zeiten für Ihr Brand Portal-Mandantenkonto zu verkürzen, müssen Sie die Aspera Connect-Clientanwendung auf Ihrem System installiert haben.

4. **Herunterladen des Aspera Connect-Clients**
Falls der Aspera Connect-Client nicht auf Ihrem System installiert oder der vorhandene installierte Aspera Connect-Client veraltet ist, wird eine Eingabeaufforderung auf der Browser-Seite angezeigt, über die Sie den systemspezifischen Aspera Connect-Client herunterladen können. Wählen Sie dazu die Option **[!UICONTROL Neueste Version herunterladen aus]**.

   ![](assets/aspera-not-launched.png)

   To download the latest version of Aspera Connect from [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), select **[!UICONTROL Download Now]** and follow the instructions.

5. **Installieren Sie den Aspera Connect Client**,
um IBM Aspera Connect-Client-Setup zu installieren, führen Sie die Setup aus der MSI-Datei der IBM Aspera Connect-Client-Anwendung aus und folgen Sie dem Installationsassistenten.

6. Sobald der Client erfolgreich installiert ist, aktualisieren Sie die Browser-Seite und führen Sie die Download-Schritte erneut aus oder wählen Sie die Option **[!UICONTROL Neu starten]** im Dialogfeld **Download]des Assets (Schritt 2).[!UICONTROL **
When using Aspera Connect for the first time, the browser prompts to open the link using **[!UICONTROL IBM Aspera Connect]**. To skip this dialog in future, enable **[!UICONTROL Remember my choice for FASP links]**.

   >[!NOTE]
   >
   >Diese Meldung unterscheidet sich von Browser zu Browser.

7. Ein Dialogfeld wird bestätigt, ob die Übertragung fortgesetzt werden soll oder nicht. Select **[!UICONTROL Allow]** to begin.
To skip this dialog in future, enable **[!UICONTROL Use my choice for all connections with this host]**.
Der Download beginnt. In einem Dialogfeld wird der Fortschritt des Downloads angezeigt. Use the dialog box to **[!UICONTROL pause]**, **[!UICONTROL resume]**, or **[!UICONTROL cancel]** the download.
Die Aspera Connect-Anwendung bietet im System ein Aktivitätsfenster, über das Benutzer alle Übertragungssitzungen anzeigen und verwalten können. Weitere Informationen finden Sie in der [Dokumentation zum Aspera Connect-Client](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

Nach erfolgreichem Abschluss des Downloads wird in einem Dialogfeld der Speicherort angezeigt, an dem Assets auf das System des Benutzers heruntergeladen werden. Wenn der Download scheitert, wird ein Fehler angezeigt.

>[!NOTE]
>
>There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab [!UICONTROL Transfers] within [!UICONTROL Preferences]. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.

## Verwenden des Dateibeschleunigers im Browser Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge wird im erweiterten geschützten Modus (EPM, Enhanced Protected Mode) ausgeführt, der eine Kommunikation mit dem Aspera Connect-Server im selben privaten Netzwerk oder mit einer vertrauenswürdigen Website verhindert. Daher wird jedes Mal, wenn eine Verbindung zum Server hergestellt wird, eine Popup-Meldung angezeigt.

![](assets/switchapps-msedge.png)

Um eine beschleunigte Download-Funktion auf Microsoft Edge zu verwenden, entfernen Sie die Markenportal-Site aus der Liste der vertrauenswürdigen Sites.

1. Open the Control Panel (press **[!UICONTROL Window key + X]**, then select **[!UICONTROL Control Panel]**).
2. Navigieren Sie zu **[!UICONTROL Netzwerk und Internet &gt; Internetoptionen]**. Klicken Sie auf die Registerkarte **[!UICONTROL Sicherheit].**
3. Klicken Sie auf **[!UICONTROL Zone vertrauenswürdiger Sites]** und dann auf **[!UICONTROL Sites]**.
4. Entfernen Sie die Brand Portal-Website aus der Liste.

## Voreinstellungen für den Aspera Connect-Client {#aspera-connect-client-preferences}

Es gibt einige nützliche Voreinstellungen, die in den Voreinstellungen des IBM Aspera Connect-Clients festgelegt werden können. Klicken Sie dazu mit der rechten Maustaste auf das Symbol und wählen Sie **[!UICONTROL Voreinstellungen aus]**.

![](assets/download_assets_frombrandportalimg19.png)

Sie können das Standard-Downloadverzeichnis festlegen.

![](assets/aspera-preferences.png)

Außerdem kann der Aspera Connect-Client so konfiguriert werden, dass er automatisch bei Systemstart gestartet und ausgeführt wird und so schneller für Downloads verfügbar ist.

![](assets/aspera-automaticallylaunch.png)

## Beheben von Problemen mit der Downloadbeschleunigung {#troubleshoot-issues-with-download-acceleration}

Wenn die Downloadbeschleunigung für Sie nicht funktioniert, führen Sie folgende Schritte aus, um zu beheben:

1. Check that ports are not blocked, by visiting [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) from your machine.

   Wenn die Ports nicht in Ordnung sind, kontaktieren Sie Ihr Netzwerkteam, um sicherzustellen, dass die Ports 33001 (TCP und UDP) nicht in der Firewall blockiert werden.

2. If the ports are OK then check if your network is not slow, by measuring the available bandwidth using [https://www.speedtest.net/](https://www.speedtest.net/).

   Ist die Brandbreite gering (1–10 MBit/s oder nur KBit/s), rufen Sie die Aspera-Voreinstellungen auf und versuchen Sie, die Bandbreite auf die verfügbare Bandbreite zu beschränken.

3. To confirm whether the downloads from Aspera demo server are working, use [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).\
   (Anmeldung: asperaweb, password: demoaspera)

4. Wenn keiner der zuvor genannten Schritte den Fehler beheben kann, heben Sie die Auswahl der Option „Downloadbeschleunigung aktivieren“ auf und verwenden Sie die normale Download-Funktion.
