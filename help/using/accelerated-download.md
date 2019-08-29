---
title: Anleitung zum Beschleunigen von Downloads von Brand Portal
seo-title: Anleitung zum Beschleunigen von Downloads von Brand Portal
description: Verkürzen Sie die Download-Zeiten von Brand Portal und freigegebenen Links.
seo-description: Verkürzen Sie die Download-Zeiten von Brand Portal und freigegebenen Links.
uuid: 2871137 e -6471-49 a 7-872 a -841 bd 92543 d 1
contentOwner: mgulati
topic-tags: download-install
content-type: Referenz
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 301 f 7 a 0 b -5527-4 aac-b 731-bfc 145 fed 0 c 0
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Anleitung zum Beschleunigen von Downloads von Brand Portal {#guide-to-accelerate-downloads-from-brand-portal}

Markenportal unterstützt den beschleunigten Download großer Asset-Dateien durch Integration mit IBM Aspera Connect, einer Installationsanwendung. Die Anwendung nutzt proprietäre Technologie, um TCP-Overheads zu verhindern und Übertragungsgeschwindigkeiten für Dateien zu verbessern und so den Download zu optimieren. Benutzer an unterschiedlichsten geografischen Standorten mit Problemen mit hoher Latenz können auch von dieser Funktion profitieren.

>[!NOTE]
>
>IBM Aspera Connect ermöglicht schnelle Downloads von großen Asset-Dateien von Brand Portal und freigegebenen Links. Die jeweilige Download-Geschwindigkeit variiert jedoch abhängig von Faktoren wie der Netzwerkbandbreite, der Serverlatenz und dem geografischen Standort der Clients.

To configure specific tenants for accelerated file download, administrators **[!UICONTROL Enable Download Acceleration]** (which is disabled by default)from **General Settings** in the administrative tools panel.

Ist diese Option aktiviert, können Brand Portal-Benutzer die zum Herunterladen der gewünschten Asset-Dateien von Brand Portal oder über freigegebene Links benötigte Zeit durch die Installation des Aspera Connect-Clients erheblich verkürzen.

![](assets/enable-fast-file-download.png)

## Voraussetzungen für die Beschleunigung des Datei-Downloads {#prerequisites-to-accelerate-file-download}

Um die schnellere Dateidownload-Funktion zu verwenden, stellen Sie Folgendes sicher:

* Administratoren haben die Ports 33001 (TCP und UDP) in der Firewall geöffnet. For more information on the prerequisites to using IBM Aspera Connect, see [Aspera Connect Client documentation](https://downloads.asperasoft.com/en/documentation/8).

   Nachfolgend sind die Download-Domänen für verschiedene geografische Standorte aufgeführt:

   | Region | Domäne |
   |---|---|
   | NA OR1 | downloads-na1.brand-portal.adobe.com |
   | NA VA5 | downloads-na2.brand-portal.adobe.com |
   | EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
   | APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

* Zum Herunterladen des IBM Aspera Connect-Installationspakets sind Administratorrechte erforderlich, da Sie Aspera Connect nicht unter einem Gastkonto installieren können.

### System- und Browseranforderungen {#system-and-browser-requirements}

Die System- und Browseranforderungen für Aspera Connect 3.8.0 sind wie folgt:

| ﻿BS | BS-Version | Browser |  | Erforderliche Bibliotheken |
|----------------|----------------------------------------|-------------------|-------|--------------------------|
| Windows | Windows 7, 8, 10 | Chrome | 64–66 |  |
|  | Windows Server 2008, R2, 2012 R2, 2016 | Firefox | 57–60 |  |
|  |  | Firefox ESR | 52 |  |
|  |  | Internet Explorer | 11 |  |
|  |  | Microsoft Edge | 39-42 |  |
| MacOS | 10.11–10.13 | Chrome | 64–66 |  |
|  |  | Firefox | 57–60 |  |
|  |  | Firefox ESR | 52 |  |
|  |  | Safari | 11 |  |
| Linux (64 Bit) | RHEL 6–7 | Chrome | 64–66 | OpenSSL 1.0.2g oder höher |
|  | CentOS 6–7 |  |  | Mesa EGL |
|  | Debian 7–9 |  |  | glib2 2.28 oder höher |
|  | SLES 11–12 |  |  |  |
|  | Fedora 26–27 |  |  |  |
|  | OpenSUSE 42.3 | Firefox | 57–60 |  |
|  | Ubuntu 14–17 | Firefox ESR | 52 |  |

Plattformunterstützungsmatrizen von verschiedenen Versionen des Aspera-Übertragungsclients finden Sie unter [Aspera Connect-Plattformunterstützungsmatrix](https://www.asperasoft.com/company/support/transfer-clients/).

## Erwartete Download-Zeiten mit dem Dateibeschleuniger {#expected-download-performance-using-file-accelerator}

Die erwartete Download-Leistung für 2 GB-Datei mit dem Aspera Connect-Dateidownload-Beschleuniger an verschiedenen Client-Speicherorten lautet wie folgt, wobei unter Oregon in den USA unter Oregon ein Brand Portal-Server angezeigt wird:

| Client-Standort | Latenzzeit zwischen Client und Server | Geschwindigkeit mit dem Aspera-Dateiübertragungsbeschleuniger | Zeit zum Herunterladen der 2 GB-Datei mit Aspera File Transfer Accelerator |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| USA, Westen (Nordkalifornien) | 18 ms | 36 MB/s | 57 Sekunden |
| USA, Westen (Oregon) | 42 ms | 36 MB/s | 57 Sekunden |
| USA, Osten (Nordvirginia) | 85 ms | 35 MB/s | 58 Sekunden |
| APAC (Tokio) | 124 ms | 36 MB/s | 57 Sekunden |
| Noida | 275 ms | 13,36 MB/s | 153 Sekunden |
| Sydney | 175 ms | 29 MB/s | 70 Sekunden |
| London | 179 ms | 35 MB/s | 58 Sekunden |
| Singapur | 196 ms | 34 MB/s | 60 Sekunden |

>[!NOTE]
>
>Die genannten Daten sind gemäß den in lab ausgeführten Tests vorhanden und werden nur angeblendet. Die festgestellten Ergebnisse variieren je nach Faktoren wie Netzwerkbandbreite, Serverlatenz und Kundenstandort.

## Download-Workflow mit dem Dateibeschleuniger {#download-workflow-using-file-accelerator}

So laden Sie Assets schneller von Brand Portal herunter:

1. Melden Sie sich über Ihren bevorzugten Browser bei Brand Portal an.
2. Suchen Sie nach der gewünschten Asset-Datei oder Sammlung bzw. dem gewünschten Ordner, die bzw. der heruntergeladen werden soll, und wählen Sie diese bzw. diesen aus. Tippen bzw. klicken Sie auf die Option „Herunterladen“.
Download dialog appears with [Enable download acceleration] option selected.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >Die Funktion zum Senden von E-Mail-Benachrichtigungen mit dem Link zum Herunterladen von Assets wird derzeit nicht unterstützt, während schnellere Downloads aktiviert sind.

   ![](assets/fast-download-emailchk.png)

3. Tap/ click **Download**.
Um die Download-Zeiten für Ihr Brand Portal-Mandantenkonto zu verkürzen, müssen Sie die Aspera Connect-Clientanwendung auf Ihrem System installiert haben.

4. **Herunterladen des Aspera Connect-Clients**
Falls der Aspera Connect-Client nicht auf Ihrem System installiert oder der vorhandene installierte Aspera Connect-Client veraltet ist, wird eine Eingabeaufforderung auf der Browser-Seite angezeigt, über die Sie den systemspezifischen Aspera Connect-Client herunterladen können. Wählen Sie dazu die Option **Neueste Version herunterladen** aus.

   ![](assets/aspera-not-launched.png)

   To download the latest version of Aspera Connect from [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), select **Download Now** and follow the instructions.

5. **Installieren Sie den Aspera Connect Client**,
um IBM Aspera Connect-Client-Setup zu installieren, führen Sie die Setup aus der MSI-Datei der IBM Aspera Connect-Client-Anwendung aus und folgen Sie dem Installationsassistenten.

6. Sobald der Client erfolgreich installiert ist, aktualisieren Sie die Browser-Seite und führen Sie die Download-Schritte erneut aus oder wählen Sie die Option **Neu starten** im Dialogfeld **Download** des Assets (Schritt 2).
When using Aspera Connect for the first time, the browser prompts to open the link using **IBM Aspera Connect**. To skip this dialog in future, enable **Remember my choice for FASP links**.

   >[!NOTE]
   >
   >Diese Meldung unterscheidet sich von Browser zu Browser.

7. Ein Dialogfeld wird bestätigt, ob die Übertragung fortgesetzt werden soll oder nicht. Select **Allow** to begin.
To skip this dialog in future, enable **Use my choice for all connections with this host**.
Der Download beginnt. In einem Dialogfeld wird der Fortschritt des Downloads angezeigt. Use the dialog box to **pause**, **resume**, or **cancel** the download.
Die Aspera Connect-Anwendung bietet im System ein Aktivitätsfenster, über das Benutzer alle Übertragungssitzungen anzeigen und verwalten können. Weitere Informationen finden Sie in der [Dokumentation zum Aspera Connect-Client](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

Nach erfolgreichem Abschluss des Downloads wird in einem Dialogfeld der Speicherort angezeigt, an dem Assets auf das System des Benutzers heruntergeladen werden. Wenn der Download scheitert, wird ein Fehler angezeigt.

>[!NOTE]
>
>There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **Always ask me where to save downloaded files** is enabled under the tab **Transfers **within **Preferences**. Before any download begins, provide the location in the text box **Save downloaded files to**.

## Verwenden des Dateibeschleunigers im Browser Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge wird im erweiterten geschützten Modus (EPM, Enhanced Protected Mode) ausgeführt, der eine Kommunikation mit dem Aspera Connect-Server im selben privaten Netzwerk oder mit einer vertrauenswürdigen Website verhindert. Daher wird jedes Mal, wenn eine Verbindung zum Server hergestellt wird, eine Popup-Meldung angezeigt.

![](assets/switchapps-msedge.png)

Um eine beschleunigte Download-Funktion auf Microsoft Edge zu verwenden, entfernen Sie die Markenportal-Site aus der Liste der vertrauenswürdigen Sites.

1. Open the Control Panel (press **Window key + X**, then select **Control Panel**).
2. Navigieren Sie zu **Netzwerk und Internet &gt; Internetoptionen**. Klicken Sie auf die Registerkarte **Sicherheit**.
3. Klicken Sie auf **Zone vertrauenswürdiger Sites** und dann auf **Sites**.
4. Entfernen Sie die Brand Portal-Website aus der Liste.

## Voreinstellungen für den Aspera Connect-Client {#aspera-connect-client-preferences}

Es gibt einige nützliche Voreinstellungen, die in den Voreinstellungen des IBM Aspera Connect-Clients festgelegt werden können. Klicken Sie dazu mit der rechten Maustaste auf das Symbol und wählen Sie **Voreinstellungen** aus.

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
