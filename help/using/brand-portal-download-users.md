---
title: Herunterladen von Assets
seo-title: Herunterladen von Assets
description: Alle Benutzer können gleichzeitig mehrere Assets oder Ordner herunterladen, auf die sie zugreifen können. Auf diese Weise können bestätigte Marken-Assets sicher für die Offline-Nutzung verteilt werden.
seo-description: Alle Benutzer können gleichzeitig mehrere Assets oder Ordner herunterladen, auf die sie zugreifen können. Auf diese Weise können bestätigte Marken-Assets sicher für die Offline-Nutzung verteilt werden.
uuid: 4 b 77118 e-a 76 e -4 d 8 a -992 a-cb 3 c 3097 bc 03
content-type: Referenz
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: download-install
discoiquuid: f 90 c 2214-beea -4695-9102-8 b 952 bc 9 fd 17
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Herunterladen von Assets {#download-assets}

All users can simultaneously download multiple assets and folders accessible to them from [!DNL Brand Portal]. Auf diese Weise können bestätigte Marken-Assets sicher für die Offline-Nutzung verteilt werden. Read on to know how to download approved assets from [!DNL Brand Portal], and what to expect from the [download performance](../using/brand-portal-download-users.md#main-pars-header).

>[!NOTE]
>
>Nur Administratoren können abgelaufenen Assets herunterladen. Weitere Informationen zu abgelaufenen Assets finden Sie unter [Digital Rights Management für Assets](../using/manage-digital-rights-of-assets.md).

## Schritte zum Herunterladen von Assets {#steps-to-download-assets}

To download assets or folders containing assets for [!DNL Brand Portal], follow these steps:

1. From the [!DNL Brand Portal] interface, do one of the following:

   * Wählen Sie die Ordner oder Assets aus, die Sie herunterladen möchten. From the toolbar at the top, click the **Download** icon.
   ![](assets/downloadassets-1.png)

   * Um einen bestimmten Ordner oder ein Asset herunterzuladen, führen Sie den Mauszeiger über den Ordner bzw. das Asset. From the quick action thumbnails available, click the **Download** icon.
   ![](assets/downloadsingleasset-1.png)

   >[!NOTE]
   >
   >Wenn die Assets, die Sie herunterladen, auch lizenzierte Assets enthalten, werden Sie zur Seite **Copyright-Management** weitergeleitet. Wählen Sie auf dieser Seite die Assets aus, klicken Sie auf **Zustimmen** und klicken Sie dann auf **Herunterladen**. Wenn Sie ablehnen, werden die lizenzierten Assets nicht heruntergeladen.\
   >License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in [!DNL AEM] Assets.

   ![](assets/licensed-asset-download-1.png)

   The **Download** dialog box appears with the **Asset(s)** option selected by default.

   ![](assets/donload-assets-dialog-1.png)

   >[!NOTE]
   >
   >If the assets you are downloading are image files, and you select only the **Asset(s)** option in Download dialog but are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) then no image files are downloaded and a Notice prompts, stating that you have been restricted by administrator to access original renditions.

   ![](assets/restrictaccess-note.png)

2. To download the renditions of assets in addition to the assets, select **Rendition(s)**. However, to allow auto-generated renditions to download along with custom renditions, deselect **Exclude Auto Generated Renditions**, which is selected by default.

   ![](assets/exclude-auto-renditions.png)

   To download only the renditions, deselect **Asset(s)**.

   >[!NOTE]
   >
   >Standardmäßig werden nur die Assets heruntergeladen. However, original renditions of image files are not downloaded if you are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   * To speed up the download of asset files from [!DNL Brand Portal], select **Enable download acceleration** option and [follow the wizard](../using/accelerated-download.md#main-pars-header-405749062). To know more about faster download of assets refer [Guide to accelerate downloads from [!DNL Brand Portal]](../using/accelerated-download.md).

   * Um eine [benutzerdefinierte Bildvorgabe zum Asset und seinen Ausgabeformaten](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages) zuzuweisen, wählen Sie **Dynamische Ausgabe(n)** aus. Legen Sie die benutzerdefinierten Eigenschaften für die Bildvorgabe fest (Größe, Format, Farbraum, Auflösung und Bild-Modifikator), um die benutzerdefinierte Bildvorgabe zuzuweisen, die beim Herunterladen des Assets und seiner Ausgabeformate verwendet wird. Um nur die dynamischen Ausgabeformate herunterzuladen, deaktivieren Sie die Option **Asset(s)**.
   ![](assets/dynamic-renditions.png)

   >[!NOTE]
   >
   >To preview (or download) dynamic renditions of any asset, ensure that the dynamic media is enabled and the asset's [!UICONTROL Pyramid tiff] rendition exists at the [!DNL AEM] author instance, from where the assets have been published. When an asset is published to [!DNL Brand Portal], its [!UICONTROL Pyramid tiff] rendition is also published. Es gibt keine Möglichkeit, die [!UICONTROL Pyramid TIFF] -Darstellung zu [!DNL Brand Portal]generieren.

   * To preserve the [!DNL Brand Portal] folder hierarchy while downloading assets, select **Create separate folder for each asset**. By default, [!DNL Brand Portal] folder hierarchy is ignored and all assets are downloaded in one folder in your local system.

   * To send an email notification to users with a link for downloading the assets, select **Email**.
   ![](assets/download-link.png)

   >[!NOTE]
   >
   >Der Downloadlink in der E-Mail-Benachrichtigung läuft nach 45 Tagen ab.
   >
   >Administrators can customize email messages, that is, logo, description, and footer, using the [Branding](../using/brand-portal-branding.md) feature.

3. Klicken Sie auf **Herunterladen**.

   Die Assets (und Ausgabeformate, sofern ausgewählt) werden als ZIP-Datei in Ihren lokalen Ordner heruntergeladen. Es wird jedoch keine ZIP-Datei erstellt, wenn ein einzelnes Asset ohne eines der Ausgabeformate heruntergeladen wird. Dies gewährleistet einen schnellen Download.

   Die Original-Ausgabeformate der ausgewählten Assets werden nicht heruntergeladen, wenn Sie [vom Administrator nicht die Berechtigung für den Zugriff auf die Original-Ausgabeformate erhalten haben](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   >[!NOTE]
   >
   >Einzeln ausgewählte und heruntergeladene Assets sind im Bericht zu heruntergeladenen Assets sichtbar. Wenn jedoch ein Ordner, der Assets enthält, heruntergeladen wird, werden weder der Ordner noch die Assets im heruntergeladenen Bericht angezeigt.

   To know how to download assets from shared links, refer [downloading assets from shared links](../using/brand-portal-link-share.md#main-pars-header-1703469193).

## Erwartete Download-Zeiten {#expected-download-performance}

Das Dateidownloaderlebnis kann je nach Faktoren, wie z. B. lokale Internetverbindung und Serverlatenz, für Benutzer unterschiedlicher Kundenstandorte unterschiedlich sein. The expected download performance for 2 GB file observed at different client locations is as follows, with [!DNL Brand Portal] server at Oregon in United States:

| Client-Standort | Latenzzeit zwischen Client und Server | Erwartete Download-Geschwindigkeit | Zeit zum Herunterladen einer 2 GB-Datei |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| USA, Westen (Nordkalifornien) | 18 ms | 7,68 MB/s | 4 Minuten |
| USA, Westen (Oregon) | 42 ms | 3,84 MB/s | 9 Minuten |
| USA, Osten (Nordvirginia) | 85 ms | 1,61 MB/s | 21 Minuten |
| APAC (Tokio) | 124 ms | 1,13 MB/s | 30 Minuten |
| Noida | 275 ms | 0,5 MB/s | 68 Minuten |
| Sydney | 175 ms | 0,49 MB/s | 69 Minuten |
| London | 179 ms | 0,32 MB/s | 106 Minuten |
| Singapur | 196 ms | 0,5 MB/s | 68 Minuten |

**Hinweis**: Die genannten Daten werden unter Testbedingungen betrachtet, was für Benutzer an unterschiedlichen Orten unterschiedlich sein kann, wenn unterschiedliche Latenz und Bandbreite erkannt werden.
