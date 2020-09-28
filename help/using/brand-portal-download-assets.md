---
title: Herunterladen von Assets
seo-title: Herunterladen von Assets
description: Alle Benutzer können gleichzeitig mehrere Assets oder Ordner herunterladen, auf die sie zugreifen können. Auf diese Weise können genehmigte Marken-Assets sicher für die Offline-Nutzung verteilt werden.
seo-description: Alle Benutzer können gleichzeitig mehrere Assets oder Ordner herunterladen, auf die sie zugreifen können. Auf diese Weise können genehmigte Marken-Assets sicher für die Offline-Nutzung verteilt werden.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: e497fb791030d74d9e5672b68387661ca7140d8a
workflow-type: tm+mt
source-wordcount: '1294'
ht-degree: 100%

---


# Herunterladen von Assets {#download-assets}

<!-- Before update in Download experience - 26th Aug 2020 by Vishabh.
 All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](../using/brand-portal-download-assets.md#main-pars-header).
-->

Adobe Experience Manager Assets Brand Portal verbessert das Download-Erlebnis, indem es den Benutzern ermöglicht, mehrere Assets und Ordner aus Brand Portal gleichzeitig herunterzuladen. Auf diese Weise können genehmigte Marken-Assets sicher für die Offline-Nutzung verteilt werden. Hier erfahren Sie, wie Sie genehmigte Assets von Brand Portal herunterladen und welche [Download-Zeiten](../using/brand-portal-download-assets.md#expected-download-performance) dabei zu erwarten sind.

>[!NOTE]
>
>Installieren Sie IBM Aspera Connect 3.9.9 als Browser-Erweiterung, bevor Sie die Assets aus Brand Portal herunterladen.


<!--
**Types of renditions in Brand Portal:**

* Original asset rendition

  It is the original binary of the asset uploaded in AEM Assets. 
  
  
* System renditions

  These are the thumbnail renditions which are automatically generated in AEM Assets based on the "DAM update asset" workflow. 
  
* Custom renditions

  These are the additional renditions that an asset might have and its dynamic renditions. Any user can create additional custom renditions, whereas, only the AEM administrator can create dynamic renditions of an image in AEM Assets. To know more, see [how to apply image presets or dynamic renditions](../using/brand-portal-image-presets.md).     
-->

## Konfigurieren des Asset-Downloads {#configure-download}

Die Download-Konfiguration ermöglicht es Brand Portal-Administratoren, die Ausgabeformate zu definieren, die den Benutzern von Brand Portal zum Herunterladen der Assets zur Verfügung stehen. Der Administrator kann die Einstellungen für den Asset-**[!UICONTROL Download]** über die Benutzeroberfläche von Brand Portal konfigurieren.

Die folgenden Konfigurationen sind verfügbar:

* **[!UICONTROL Schneller Download]**

   Ermöglicht Hochgeschwindigkeits-Downloads von Assets. Weitere Informationen finden Sie unter [Anleitung zur Beschleunigung von Downloads aus Brand Portal](../using/accelerated-download.md).

* **[!UICONTROL Benutzerdefinierte Ausgabeformate]**

   Laden Sie benutzerdefinierte und (oder) dynamische Ausgabeformate der Assets herunter.
Alle Asset-Ausgabeformate außer dem ursprünglichen Asset und den systemgenerierten Ausgaben werden als benutzerdefinierte Ausgaben aufgerufen. Dies schließt sowohl statische als auch dynamische Ausgaben ein, die für das Asset verfügbar sind. Jeder Benutzer kann eine benutzerdefinierte statische Ausgabe in AEM Assets erstellen. Allerdings kann nur der AEM-Administrator benutzerdefinierte dynamische Ausgaben erstellen. Weitere Informationen finden Sie unter [Anwenden von Bildvorgaben oder dynamischen Ausgabeformaten](../using/brand-portal-image-presets.md)

* **[!UICONTROL Systemausgaben]**

   Laden Sie systemgenerierte Ausgabeformate der Assets herunter. Dies sind die Miniaturansichten, die in AEM Assets auf der Grundlage des Workflows „DAM-Update-Asset“ automatisch generiert werden.

Melden Sie sich bei Ihrem Brand Portal-Mandanten als Administrator an und navigieren Sie zu **[!UICONTROL Tools]** > **[!UICONTROL Download]**. Standardmäßig ist die Konfiguration **[!UICONTROL Schneller Download]** in den **[!UICONTROL Download-Einstellungen]** aktiviert.

Administratoren können jede beliebige Kombination aktivieren, um den Asset-Download-Prozess zu konfigurieren.

![](assets/download-configuration.png)


Je nach Konfiguration bleibt der Download-Workflow für eigenständige Assets, mehrere Assets, Ordner mit Assets, lizenzierte oder nicht lizenzierte Assets und den Download von Assets über einen Freigabe-Link konstant.


* Wenn die Konfigurationen für **[!UICONTROL benutzerdefinierte Ausgaben]** und **[!UICONTROL Systemausgaben]** deaktiviert sind, werden die Original-Ausgabeformate der Assets heruntergeladen, ohne dass den Benutzern ein zusätzliches Dialogfeld angezeigt wird.

<!--
If all the three download configurations are turned-off, or only the **[!UICONTROL Fast Download]** configuration is enabled, the original assets are directly downloaded on your local system with no additional step required.
Test.. 
-->

* Wenn eine der Konfigurationen für **[!UICONTROL benutzerdefinierte Ausgaben]** oder **[!UICONTROL Systemausgaben]** aktiviert ist, wird ein zusätzliches Dialogfeld für den **[!UICONTROL Download]** angezeigt, in dem Sie auswählen können, ob das Original-Asset zusammen mit seinen Ausgabeformaten heruntergeladen werden soll oder ob nur bestimmte Ausgabeformate heruntergeladen werden sollen.

>[!NOTE]
>
>Nur die Administratoren können die abgelaufenen Assets herunterladen. Weitere Informationen zu abgelaufenen Assets finden Sie unter [Verwalten der digitalen Rechte von Assets](../using/manage-digital-rights-of-assets.md).


## Schritte zum Herunterladen von Assets        {#steps-to-download-assets}

Im Folgenden werden die Schritte zum Herunterladen von Assets oder Ordnern mit Assets aus Brand Portal beschrieben:

1. Führen Sie in der Brand Portal-Benutzeroberfläche einen der folgenden Schritte aus:

   * Wählen Sie die Ordner oder Assets aus, die Sie herunterladen möchten. Klicken Sie oben in der Symbolleiste auf das Symbol **[!UICONTROL Download]**.

      ![](assets/downloadassets-1.png)

   * Um ein bestimmtes Asset oder einen bestimmten Ordner herunterzuladen, halten Sie den Mauszeiger über das Asset oder den Ordner und klicken Sie in den Schnellzugriff-Miniaturansichten auf das Symbol **[!UICONTROL Download]**.

      ![](assets/downloadsingleasset-1.png)


      >[!NOTE]
      >
      >Wenn Sie die Assets zum ersten Mal herunterladen und IBM Aspera Connect nicht in Ihrem Browser installiert haben, werden Sie aufgefordert, Aspera Download Accelerator zu installieren.

      >[!NOTE]
      >
      >Wenn die Assets, die Sie herunterladen, auch lizenzierte Assets enthalten, werden Sie zur Seite **[!UICONTROL Copyright-Management]** weitergeleitet. Wählen Sie auf dieser Seite die Assets aus, klicken Sie auf **[!UICONTROL Zustimmen]** und klicken Sie dann auf **[!UICONTROL Herunterladen]**. Wenn Sie ablehnen, werden die lizenzierten Assets nicht heruntergeladen.
      > 
      >An lizenzgeschützte Assets wird eine [Lizenzvereinbarung angehängt](https://helpx.adobe.com/de/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets). Dazu muss die [Metadateneigenschaft](https://helpx.adobe.com/de/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) der Assets in Experience Manager Assets entsprechend eingestellt werden.

      ![](assets/licensed-asset-download-1.png)

      <!--
     >>[!NOTE]
     >
     >Ensure to select all the required asset renditions while downloading them from the asset details page, and click **[!UICONTROL Download]**. The selected renditions are downloaded to your local machine.
     > 
     >Once you download, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the downloaded renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.
     >
     -->

      Wenn eine der Konfigurationen für **[!UICONTROL benutzerdefinierte Ausgaben]** oder **[!UICONTROL Systemausgaben]** in den **[!UICONTROL Download-Einstellungen]** aktiviert ist, wird das Dialogfeld **[!UICONTROL Download]** angezeigt, wobei das Kontrollkästchen **[!UICONTROL Assets]** standardmäßig ausgewählt ist. Wenn die Konfiguration **[!UICONTROL Schneller Download]** aktiviert ist, ist das Kontrollkästchen **[!UICONTROL Download-Beschleunigung aktivieren]** standardmäßig aktiviert.

      ![](assets/download-dialog.png)

      >[!NOTE]
      >
      >Wenn es sich bei den Assets, die Sie herunterladen, um Bilddateien handelt und Sie nur das Kontrollkästchen **[!UICONTROL Asset(s)]** im Dialogfeld **[!UICONTROL Download]** aktivieren, aber nicht [von einem Administrator berechtigt wurden, auf die Original-Ausgabeformate der Bilddateien zuzugreifen](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), werden keine Bilddateien heruntergeladen. Dann erscheint der Hinweis, dass der Administrator Ihnen keine Berechtigung für den Zugriff auf Original-Ausgabeformate erteilt hat.

      ![](assets/restrictaccess-note.png)

1. Um die Ausgabeformate zusätzlich zu den Original-Assets herunterzuladen, aktivieren Sie das Kontrollkästchen **[!UICONTROL Ausgabeformat(e)]**. Wenn Sie jedoch die systemgenerierten Ausgabeformate zusammen mit den benutzerdefinierten Ausgabeformaten herunterladen möchten, deaktivieren Sie das Kontrollkästchen **[!UICONTROL Systemausgaben ausschließen]**.

   ![](assets/download-system-rendition.png)

   * Wenn Sie nur die Ausgabeformate herunterladen möchten, deaktivieren Sie das Kontrollkästchen **[!UICONTROL Asset(s)]**.

      >[!NOTE]
      >
      >Standardmäßig werden nur die Assets heruntergeladen. Die Original-Ausgabeformate der Bilddateien werden jedoch nicht heruntergeladen, wenn Sie[ vom Administrator nicht die Berechtigung für den Zugriff auf die Original-Ausgabeformate der Bilddateien erhalten haben](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   * Um die ausgewählten Assets über einen Link für andere Benutzer freizugeben, aktivieren Sie das Kontrollkästchen **[!UICONTROL E-Mail]**. Den Benutzern wird eine E-Mail-Benachrichtigung mit dem Link zum Herunterladen gesendet. Informationen zum Herunterladen von Assets über freigegebene Links finden Sie unter [Herunterladen von Assets über freigegebene Links](../using/brand-portal-link-share.md#main-pars-header-1703469193).

      ![](assets/download-link.png)

      >[!NOTE]
      >
      >Der Downloadlink in der E-Mail-Benachrichtigung läuft nach 45 Tagen ab.
      >
      >Administratoren können mit der Funktion [Branding](../using/brand-portal-branding.md) das Logo, die Beschreibung und die Fußzeile der E-Mail-Nachrichten anpassen.

   * Sie können eine vordefinierte Bildvorgabe auswählen oder eine benutzerdefinierte dynamische Ausgabe im Dialogfeld **[!UICONTROL Download]** erstellen.

      Um eine [benutzerdefinierte Bildvorgabe auf das Asset und seine Ausgaben](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages) anzuwenden, aktivieren Sie das Kontrollkästchen **[!UICONTROL Dynamische Ausgabe(n)]**. Legen Sie die Eigenschaften für die Bildvorgabe fest (Größe, Format, Farbraum, Auflösung und Bild-Modifikator), um während des Downloads des Assets und seiner Ausgabeformate die benutzerdefinierte Bildvorgabe anzuwenden. Wenn Sie nur die dynamischen Ausgaben herunterladen möchten, deaktivieren Sie das Kontrollkästchen **[!UICONTROL Asset(s)]**.

      ![](assets/dynamic-rendition.png)

      >[!NOTE]
      >
      >Brand Portal unterstützt die Konfiguration von Dynamic Media sowohl im Hybird- als auch im Scene7-Modus.
      >
      >(*Bei Ausführung der AEM-Autoreninstanz im **Dynamic Media-Hybrid-Modus***)      >Um dynamische Ausgaben eines Assets als Vorschau anzeigen (oder herunterladen) zu können, stellen Sie sicher, dass Dynamic Media aktiviert ist und die Pyramid TIFF-Ausgabe in der AEM Assets-Autoreninstanz, von der aus die Assets veröffentlicht wurden, vorhanden ist. Wenn ein Asset in Brand Portal veröffentlicht wird, wird auch sein PTIFF-Ausgabeformat veröffentlicht.

   * Damit die Brand Portal-Ordnerhierarchie beim Herunterladen von Assets erhalten bleibt, aktivieren Sie das Kontrollkästchen **[!UICONTROL Separaten Ordner für jedes Asset erstellen]**. Die Brand Portal-Ordnerhierarchie wird standardmäßig ignoriert und alle Assets werden in einen Ordner auf Ihrem lokalen System heruntergeladen.

1. Klicken Sie auf **[!UICONTROL Download]**.

   Die Assets (und Ausgaben, sofern ausgewählt) werden als ZIP-Datei in Ihren lokalen Ordner heruntergeladen. Es wird jedoch keine ZIP-Datei erstellt, wenn ein einzelnes Asset ohne eine der Ausgaben heruntergeladen wird.

   Wenn Sie nicht [vom Administrator für Zugriff auf die Originalausgaben autorisiert wurden](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), werden die Originalausgaben der ausgewählten Assets nicht heruntergeladen.

   >[!NOTE]
   >
   >Einzeln ausgewählte und heruntergeladene Assets sind im Bericht zu heruntergeladenen Assets sichtbar. Wenn jedoch ein Ordner mit Assets heruntergeladen wird, werden weder der Ordner noch die Assets im Bericht zu heruntergeladenen Assets angezeigt.


## Erwartete Download-Zeiten {#expected-download-performance}

Die Zeiten von Datei-Downloads variieren unter Umständen für Benutzer an verschiedenen Client-Standorten. Dies ist abhängig von Faktoren wie der lokalen Internet-Verbindung und der Server-Latenz. Die erwartete Download-Zeit für eine 2 GB große Datei an verschiedenen Client-Standorten ist wie folgt, wenn sich der Brand Portal-Server in Oregon in den USA befindet:

| Client-Standort | Latenz zwischen Client und Server | Erwartete Download-Geschwindigkeit | Erforderliche Zeit für den Download einer 2 GB großen Datei |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| USA, Westen (Nordkalifornien) | 18 ms | 7,68 MB/s | 4 Minuten |
| USA, Westen (Oregon) | 42 ms | 3,84 MB/s | 9 Minuten |
| USA, Osten (Nordvirginia) | 85 ms | 1,61 MB/s | 21 Minuten |
| Asien-Pazifik-Raum (Tokio) | 124 ms | 1,13 MB/s | 30 Minuten |
| Noida | 275 ms | 0,5 MB/s | 68 Minuten |
| Sydney | 175 ms | 0,49 MB/s | 69 Minuten |
| London | 179 ms | 0,32 MB/s | 106 Minuten |
| Singapur | 196 ms | 0,5 MB/s | 68 Minuten |

>[!NOTE]
>
>Hinweis: Die angegebenen Daten wurden unter Testbedingungen gemessen und können daher für Benutzer an verschiedenen Standorten mit unterschiedlicher Latenz und Bandbreite abweichen.

