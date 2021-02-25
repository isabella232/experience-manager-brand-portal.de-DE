---
title: Herunterladen von Assets
seo-title: Herunterladen von Assets
description: Alle Benutzer können gleichzeitig mehrere Assets oder Ordner herunterladen, auf die sie zugreifen können. Auf diese Weise können genehmigte Marken-Assets sicher für die Offline-Nutzung verteilt werden.
seo-description: Alle Benutzer können gleichzeitig mehrere Assets oder Ordner herunterladen, auf die sie zugreifen können. Auf diese Weise können genehmigte Marken-Assets sicher für die Offline-Nutzung verteilt werden.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
contentOwner: Vishabh Gupta
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: fab0855e8d30e7b6ddf9b4ae5b2ce1fb627c81ce
workflow-type: tm+mt
source-wordcount: '1935'
ht-degree: 36%

---


# Herunterladen von Assets aus dem Markenportal {#download-assets-from-bp}

<!-- Before update in Download experience - 26th Aug 2020 comment by Vishabh.
 All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](../using/brand-portal-download-assets.md#main-pars-header).
-->

Adobe Experience Manager Assets Brand Portal verbessert das Download-Erlebnis, indem es den Benutzern ermöglicht, mehrere Assets und Ordner aus Brand Portal gleichzeitig herunterzuladen. Auf diese Weise können genehmigte Marken-Assets sicher für die Offline-Nutzung verteilt werden. Hier erfahren Sie, wie Sie genehmigte Assets von Brand Portal herunterladen und welche [Download-Zeiten](../using/brand-portal-download-assets.md#expected-download-performance) dabei zu erwarten sind.


>[!NOTE]
>
>In Brand Portal 2020.10.0 (und höher) ist die Einstellung **[!UICONTROL Fast Download]** standardmäßig aktiviert, die IBM Aspera Connect zum beschleunigten Herunterladen der Assets verwendet. [Installieren Sie IBM Aspera Connect 3.9.9 als Browser-Erweiterung, bevor Sie die Assets aus Brand Portal herunterladen. ](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) Weitere Informationen finden Sie unter [Anleitung zum Beschleunigen von Downloads aus dem Markenportal](../using/accelerated-download.md).
>
>Wenn Sie IBM Aspera Connect nicht verwenden und den normalen Download-Prozess fortsetzen möchten, wenden Sie sich an den Markenportal-Administrator, um die Einstellung **[!UICONTROL Schneller Download]** zu deaktivieren.

## Konfigurieren des Asset-Downloads {#configure-download}

Markenportal-Administratoren können die Einstellungen für den Asset-Download und die Benutzergruppe für die Markenportal-Benutzer konfigurieren, damit sie über die Oberfläche des Markenportals auf Asset-Darstellungen zugreifen und diese herunterladen können.

>[!NOTE]
>
>Die auf der Benutzeroberfläche angewendeten Download-Einstellungen erleichtern den Benutzern des Markenportals eine Selbstbedienung, um die Asset-Darstellungen einfach zu konfigurieren und herunterzuladen. Das Herunterladen von Assets auf der Anwendungsebene wird dadurch nicht eingeschränkt. Die Benutzer können beispielsweise weiterhin auf die Asset-Darstellungen zugreifen und sie mit dem vollständigen URL-Pfad herunterladen.

Der Zugriff auf und das Herunterladen der Asset-Darstellungen über die Oberfläche des Markenportals sind durch die folgenden Konfigurationen definiert:

* Download-Einstellungen aktivieren
* Konfigurieren von Benutzergruppeneinstellungen

### Download-Einstellungen {#enable-download-settings} aktivieren

Die Administratoren können das Asset **[!UICONTROL Download-Einstellungen]** aktivieren, um die Darstellungen zu definieren, auf die die Benutzer des Markenportals zum Herunterladen zugreifen können.

Die verfügbaren Einstellungen sind:

* **[!UICONTROL Schneller Download]**

   Es bietet einen beschleunigten Download der Assets mit IBM Aspera Connect. Standardmäßig ist die Einstellung **[!UICONTROL Schneller Download]** unter **[!UICONTROL Download-Einstellungen]** aktiviert.

* **[!UICONTROL Benutzerdefinierte Ausgabeformate]**

   Ermöglicht das Herunterladen benutzerdefinierter und (oder) dynamischer Darstellungen der Assets.

   Alle Asset-Darstellungen außer dem ursprünglichen Asset und den systemgenerierten Darstellungen werden als benutzerdefinierte Darstellungen bezeichnet. Dies schließt sowohl statische als auch dynamische Ausgaben ein, die für das Asset verfügbar sind. Jeder Benutzer kann eine benutzerdefinierte statische Ausgabe in AEM Assets erstellen. Allerdings kann nur der AEM-Administrator benutzerdefinierte dynamische Ausgaben erstellen. Weitere Informationen finden Sie unter [Anwenden von Bildvorgaben oder dynamischen Darstellungen](../using/brand-portal-image-presets.md).

* **[!UICONTROL Systemausgaben]**

   Aktiviert das Herunterladen systemgenerierter Darstellungen der Assets.

   Dies sind die Miniaturansichten, die in AEM Assets auf der Grundlage des Workflows „DAM-Update-Asset“ automatisch generiert werden.

* **[!UICONTROL Asset-Download]**

   Ermöglicht das Herunterladen der Darstellungen in einem separaten Ordner für jedes Asset. Die Einstellung gilt für Ordner, Sammlungen und den Massendownload von Assets (über 20 Assets).


Melden Sie sich bei Ihrem Brand Portal-Mandanten als Administrator an und navigieren Sie zu **[!UICONTROL Tools]** > **[!UICONTROL Download]**.

Die Administratoren können eine beliebige Kombination von Einstellungen für die Benutzer des Markenportals aktivieren, um auf Darstellungen zuzugreifen und sie herunterzuladen.

![](assets/download-settings-new.png)


>[!NOTE]
>
>Nur die Administratoren können die abgelaufenen Assets herunterladen. Weitere Informationen zu abgelaufenen Assets finden Sie unter [Verwalten der digitalen Rechte von Assets](../using/manage-digital-rights-of-assets.md).

### Konfigurieren von Benutzergruppeneinstellungen {#configure-user-group-settings}

Zusätzlich zu den **[!UICONTROL Download-Einstellungen]** können die Markenportal-Administratoren die Einstellungen für verschiedene Benutzergruppen zur Ansicht konfigurieren und (oder) die Originalelemente und deren Darstellungen herunterladen.

Melden Sie sich bei Ihrem Markenportal-Mandanten als Administrator an und navigieren Sie zu **[!UICONTROL Tools]** > **[!UICONTROL Benutzer]**. Navigieren Sie auf der Seite **[!UICONTROL Benutzerrollen]** zur Registerkarte **[!UICONTROL Gruppen]**, um die Ansichten- und (oder) Downloadeinstellungen für die Benutzergruppen zu konfigurieren.

![view-download-permission](assets/download-permissions.png)

>[!NOTE]
>
>Wenn ein Benutzer mehreren Gruppen hinzugefügt wurde und eine dieser Gruppen über Einschränkungen verfügt, gelten die Einschränkungen für diesen Benutzer.

Je nach Konfiguration bleibt der Download-Workflow für eigenständige Assets, mehrere Assets, Ordner mit Assets, lizenzierte oder nicht lizenzierte Assets und den Download von Assets über einen Freigabe-Link konstant.

Die folgende Matrix definiert, ob ein Benutzer je nach den [Downloadkonfigurationen](#configure-download) Zugriff auf die Darstellungen hat:

| **Download-Einstellungen: Benutzerdefinierte Darstellungen** | **Download-Einstellungen: Systemdarstellungen** | **Benutzergruppeneinstellungen: Original herunterladen** | **Benutzergruppeneinstellungen: Darstellungen herunterladen** | **Ergebnis** |
|---|---|---|---|---|
| EIN | EIN | EIN | EIN | Ansicht und Herunterladen aller Darstellungen |
| EIN | EIN | OFF | OFF | Original-Asset der Ansicht |
| OFF | OFF | EIN | EIN | Ansicht und Herunterladen des Originalassets |
| EIN | OFF | EIN | EIN | Ansicht und Herunterladen von Original-Assets und benutzerdefinierten Darstellungen |
| OFF | EIN | EIN | EIN | Ansicht und Herunterladen der Original-Asset- und Systemdarstellungen |
| EIN | OFF | OFF | OFF | Original-Asset der Ansicht |
| OFF | EIN | OFF | OFF | Original-Asset der Ansicht |
| OFF | OFF | OFF | EIN | Original-Asset der Ansicht |
| OFF | OFF | EIN | OFF | Ansicht und Herunterladen des Originalassets |
| OFF | OFF | OFF | OFF | Original-Asset der Ansicht |



## Herunterladen von Assets {#download-assets}

Benutzer von Brand Portal können mehrere Assets, Ordner mit Assets und Sammlungen von der Oberfläche des Markenportals herunterladen.

>[!NOTE]
>
>Wenden Sie sich an den Markenportal-Administrator, wenn Sie nicht berechtigt sind, auf die Asset-Darstellungen zuzugreifen oder sie herunterzuladen.

Wenn der Benutzer Zugriff auf Darstellungen hat, wird dem Benutzer das erweiterte Dialogfeld **[!UICONTROL Herunterladen]** mit den folgenden Funktionen bereitgestellt:
* Anzeigen aller verfügbarer Ausgabedarstellungen eines Assets in der Download-Liste.
* Ausschließen von Ausgabedarstellungen der Assets, die nicht heruntergeladen werden müssen.
* Wenden Sie denselben Darstellungssatz auf alle ähnlichen Asset-Typen mit einem Klick an.
* Anwenden eines anderen Darstellungssatzes für verschiedene Asset-Typen.
* Erstellen Sie für jedes Asset einen eigenen Ordner.
* Herunterladen ausgewählter Assets und ihrer Ausgabedarstellungen.

![download-dialog](assets/download-dialog-box.png)

>[!NOTE]
>
>Das Dialogfeld **[!UICONTROL Download]** wird nur angezeigt, wenn **[!UICONTROL Benutzerspezifische Darstellungen]** und (oder) **[!UICONTROL Systemwiedergaben]** unter **[!UICONTROL Download-Einstellungen]** aktiviert ist.


### Schritte zum Herunterladen von Assets {#bulk-download}

Im Folgenden finden Sie die Schritte zum Herunterladen von Assets oder Ordnern, die Assets enthalten, aus der Benutzeroberfläche des Markenportals:

1. Melden Sie sich bei Ihrem Markenportal-Mandanten an. Standardmäßig wird die Ansicht **[!UICONTROL Files]** geöffnet, die alle veröffentlichten Assets und Ordner enthält.

   Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie die Assets oder Ordner aus, die Sie herunterladen möchten. Klicken Sie oben in der Symbolleiste auf das Symbol **[!UICONTROL Download]**.

      ![select-multiple-assets](assets/select-assets-new.png)

   * Um bestimmte Asset-Darstellungen eines Assets herunterzuladen, halten Sie den Mauszeiger über das Asset und klicken Sie auf das Symbol **[!UICONTROL Herunterladen]**, das in den Miniaturbildern der Schnellaktion verfügbar ist.

      ![select-asset](assets/select-asset.png)


      >[!NOTE]
      >
      >Wenn Sie die Assets zum ersten Mal herunterladen und IBM Aspera Connect nicht in Ihrem Browser installiert haben, werden Sie aufgefordert, [den Aspera Download Accelerator](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) zu installieren.


      >[!NOTE]
      >
      >Wenn die Assets, die Sie herunterladen, auch lizenzierte Assets enthalten, werden Sie zur Seite **[!UICONTROL Copyright-Management]** weitergeleitet. Wählen Sie auf dieser Seite die Assets aus, klicken Sie auf **[!UICONTROL Zustimmen]** und klicken Sie dann auf **[!UICONTROL Herunterladen]**. Wenn Sie ablehnen, werden die lizenzierten Assets nicht heruntergeladen.
      > 
      >An lizenzgeschützte Assets wird eine [Lizenzvereinbarung angehängt](https://helpx.adobe.com/de/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets). Dazu muss die [Metadateneigenschaft](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) der Assets in Experience Manager Assets entsprechend eingestellt werden.


      ![lizenziertes Asset](assets/licensed-asset-new.png)

1. Das Dialogfeld **[!UICONTROL Download]**, in dem alle ausgewählten Assets aufgelistet sind, wird geöffnet.

   Klicken Sie auf ein beliebiges Asset, um die verfügbaren Darstellungen Ansicht, und aktivieren Sie die Kontrollkästchen der Darstellungen, die Sie herunterladen möchten.

   Sie können die Darstellungen für einzelne Assets manuell auswählen oder ausschließen oder auf das Symbol **Anwenden** klicken, um denselben Darstellungssatz auszuwählen, der für ähnliche Asset-Typen heruntergeladen werden soll (alle Bilddateien in diesem Beispiel). Klicken Sie im Dialogfeld **[!UICONTROL Alle anwenden]** auf **[!UICONTROL Fertig]**, um die Regel auf alle ähnlichen Assets anzuwenden.

   ![apply-all](assets/apply.png)

   Sie können ein Asset auch aus der Download-Liste entfernen (falls erforderlich), indem Sie auf das Symbol **Entfernen** klicken.

   ![Entfernen](assets/remove.png)

   Damit die Brand Portal-Ordnerhierarchie beim Herunterladen von Assets erhalten bleibt, aktivieren Sie das Kontrollkästchen **[!UICONTROL Separaten Ordner für jedes Asset erstellen.]**

   Die Downloadschaltfläche gibt die Anzahl der ausgewählten Elemente wieder. Nachdem Sie die Regeln angewendet haben, klicken Sie auf **[!UICONTROL Elemente herunterladen]**.

   ![download-dialog](assets/download-dialog-box-new.png)

1. Standardmäßig ist die Einstellung **[!UICONTROL Schneller Download]** in **[!UICONTROL Download-Einstellungen]** aktiviert. Daher wird ein Bestätigungsfeld angezeigt, um einen beschleunigten Download mit IBM Aspera Connect zu ermöglichen.

   Um weiterhin **[!UICONTROL Schnelles Herunterladen]** zu verwenden, klicken Sie auf **[!UICONTROL Zulassen]**. Alle ausgewählten Darstellungen werden mit IBM Aspera Connect in einen ZIP-Ordner heruntergeladen.

   Wenn Sie IBM Aspera Connect nicht verwenden möchten, klicken Sie auf **[!UICONTROL Ablehnen]**. Wenn **[!UICONTROL Fast Download]** verweigert wird oder fehlschlägt, füllt das System eine Fehlermeldung aus. Klicken Sie auf die Schaltfläche **[!UICONTROL Normaler Download]**, um mit dem Herunterladen der Assets fortzufahren.

>[!NOTE]
>
>Wenn die Einstellung **[!UICONTROL Schneller Download]** vom Administrator deaktiviert wird, werden die ausgewählten Darstellungen direkt in einen ZIP-Ordner heruntergeladen, ohne IBM Aspera Connect zu verwenden.


>[!NOTE]
>
>Wenn ein Ordner, eine Sammlung oder mehr als 20 Assets zum Herunterladen ausgewählt sind, wird das Dialogfeld **[!UICONTROL Herunterladen]** übersprungen und alle für den Benutzer verfügbaren Asset-Darstellungen mit Ausnahme der dynamischen Darstellungen werden in einen ZIP-Ordner heruntergeladen.
>
>Wenn die Einstellung **[!UICONTROL Asset-Download]** in **[!UICONTROL Download-Einstellungen]** aktiviert ist, werden die Asset-Darstellungen für jedes Asset im ZIP-Ordner in einen separaten Ordner heruntergeladen.


>[!NOTE]
>
>Brand Portal unterstützt die Konfiguration von Dynamic Media sowohl im Hybrid- als auch im Scene7-Modus.
>
>(*Bei Ausführung der AEM-Autoreninstanz im **Dynamic Media-Hybrid-Modus***)
>
>Um dynamische Ausgaben eines Assets als Vorschau anzeigen (oder herunterladen) zu können, stellen Sie sicher, dass Dynamic Media aktiviert ist und die Pyramid TIFF-Ausgabe in der AEM Assets-Autoreninstanz, von der aus die Assets veröffentlicht wurden, vorhanden ist. Wenn ein Asset vom AEM zum Markenportal veröffentlicht wird, wird auch seine Pyramid-TIFF-Darstellung veröffentlicht.



Wenn Sie nicht [vom Administrator für Zugriff auf die Originalausgaben autorisiert wurden](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), werden die Originalausgaben der ausgewählten Assets nicht heruntergeladen.

![no-access-message](assets/no-access-message.png)

<!-- This issue has been resolved, check with engineering.
>[!NOTE]
>
>Once you have downloaded the asset renditions, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.
-->

### Herunterladen von Assets von der Seite mit den Asset-Details {#download-assets-from-asset-details-page}

Neben dem Arbeitsablauf zum Herunterladen gibt es eine andere Methode, die Darstellungen für einzelne Assets direkt von der Seite mit den Asset-Details herunterzuladen.

Die Benutzer können verschiedene Darstellungen Vorschau, bestimmte Darstellungen auswählen und diese direkt aus dem Bedienfeld **[!UICONTROL Darstellungen]** auf der Seite mit den Asset-Details herunterladen, ohne das Dialogfeld **[!UICONTROL Herunterladen]** öffnen zu müssen.


Führen Sie die folgenden Schritte aus, um Asset-Darstellungen von der Seite mit den Asset-Details herunterzuladen:

1. Melden Sie sich bei Ihrem Markenportal-Mandanten an und klicken Sie auf das Asset, um die Seite mit den Asset-Details zu öffnen.
1. Klicken Sie auf das Symbol für die Überlagerung auf der linken Seite und dann auf **[!UICONTROL Darstellungen]**.

   ![rendition-navigation](assets/rendition-navigation.png)

1. Im Bedienfeld **[!UICONTROL Darstellungen]** werden alle verfügbaren Asset-Darstellungen basierend auf den Asset [Downloadkonfigurationen](#configure-download) Liste.

   Wählen Sie die gewünschten Darstellungen aus und klicken Sie auf **[!UICONTROL Elemente herunterladen]**.

   ![renditions-panel](assets/renditions-panel.png)

1. Standardmäßig ist die Einstellung **[!UICONTROL Schneller Download]** in **[!UICONTROL Download-Einstellungen]** aktiviert. Daher wird ein Bestätigungsfeld angezeigt, um einen beschleunigten Download mit IBM Aspera Connect zu ermöglichen.

   Um weiterhin **[!UICONTROL Schnelles Herunterladen]** zu verwenden, klicken Sie auf **[!UICONTROL Zulassen]**. Alle ausgewählten Darstellungen werden mit IBM Aspera Connect in einen ZIP-Ordner heruntergeladen.

   Wenn Sie die Verwendung von **[!UICONTROL Fast Download]** ablehnen, füllt das System eine Fehlermeldung aus. Klicken Sie auf die Schaltfläche **[!UICONTROL Normaler Download]**, um mit dem Herunterladen der Assets fortzufahren.

>[!NOTE]
>
>Wenn die Einstellung **[!UICONTROL Schneller Download]** vom Administrator deaktiviert wird, werden die ausgewählten Darstellungen direkt in einen ZIP-Ordner heruntergeladen, ohne IBM Aspera Connect zu verwenden.


>[!NOTE]
>
>Einzeln ausgewählte und heruntergeladene Assets sind im Bericht zu heruntergeladenen Assets sichtbar. Wenn jedoch ein Ordner mit Assets heruntergeladen wird, werden weder der Ordner noch die Assets im Bericht zu heruntergeladenen Assets angezeigt.

<!--
>[!NOTE]
>
>Assets that are individually downloaded are visible in the assets download report. However, if a folder containing assets is downloaded, the folder and assets are not displayed in the assets download report.
-->

<!-- Backup of content before updating the new feature docs.
## Configure asset download {#configure-download}

The download configuration allows the Brand Portal administrators to define the set of renditions available to the Brand Portal users for downloading the assets. The administrator can configure the asset **[!UICONTROL Download]** settings from the Brand Portal interface. 

The available configurations are:

* **[!UICONTROL Fast Download]** 

  Enables high-speed download of the assets. To know more, see [guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).

* **[!UICONTROL Custom Renditions]** 
  
  Download custom and (or) dynamic renditions of the assets. 
  All the asset renditions other than the original asset and system-generated renditions are called as custom renditions. It includes static as well as dynamic renditions available for the asset. Any user can create a custom static rendition in AEM Assets, whereas, only the AEM administrator can create custom dynamic renditions. To know more, see [how to apply image presets or dynamic renditions](../using/brand-portal-image-presets.md)

* **[!UICONTROL System Renditions]** 

  Download system-generated renditions of the assets. These are the thumbnails which are automatically generated in AEM Assets based on the "DAM update asset" workflow. 

Log in to your Brand Portal tenant as an administrator and navigate to **[!UICONTROL Tools]** > **[!UICONTROL Download]**. By default, the **[!UICONTROL Fast Download]** configuration is enabled in the **[!UICONTROL Download Settings]**. 

The administrators can enable any combination to configure the asset download process.

![](assets/download-configuration.png)


Based on the configuration, the download workflow remains constant for stand-alone assets, multiple assets, folders containing assets, licensed or unlicensed assets, and downloading assets using share link. 


* If both **[!UICONTROL Custom Renditions]** and **[!UICONTROL System Renditions]** configurations are turned-off, the original renditions of the assets are downloaded without any additional dialog being presented to the users.    


* If any of the **[!UICONTROL Custom Renditions]** or **[!UICONTROL System Renditions]** configuration is enabled, an additional **[!UICONTROL Download]** dialog box appears wherein you can choose whether to download the original asset along with its renditions, or download only specific renditions. 

>[!NOTE]
>
>Only the administrators can download the expired assets. For more information about expired assets, see [manage digital rights of assets](../using/manage-digital-rights-of-assets.md).

## Steps to download assets {#steps-to-download-assets}

Following are the steps to download assets or folders containing assets from Brand Portal:

1. From the Brand Portal interface, do one of the following:

   * Select the folders or assets you want to download. From the toolbar at the top, click the **[!UICONTROL Download]** icon.

     ![](assets/downloadassets-1.png)

   * To download a specific asset or folder, hover the pointer over the asset or folder and click the **[!UICONTROL Download]** icon available in the quick action thumbnails.

     ![](assets/downloadsingleasset-1.png)


     >[!NOTE]
     >
     >If you are downloading the assets for the first time and do not have IBM Aspera Connect installed in your browser, it will prompt you to install the Aspera download accelerator. 


     >[!NOTE]
     >
     >If the assets you are downloading also include licensed assets, you are redirected to the **[!UICONTROL Copyright Management]** page. In this page, select the assets, click **[!UICONTROL Agree]**, and then click **[!UICONTROL Download]**. If you choose to disagree, licensed assets are not downloaded. 
     > 
     >License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in Experience Manager Assets.


     ![](assets/licensed-asset-download-1.png)

     
     >[!NOTE]
     >
     >Ensure to select all the required asset renditions while downloading them from the asset details page, and click **[!UICONTROL Download]**. The selected renditions are downloaded to your local machine.
     > 
     >Once you download, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the downloaded renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.

     If any of the **[!UICONTROL Custom Renditions]** or **[!UICONTROL System Renditions]** configuration is enabled in the **[!UICONTROL Download Settings]**, the **[!UICONTROL Download]** dialog appears with the **[!UICONTROL Asset(s)]** check box selected by default. If the **[!UICONTROL Fast Download]** configuration is enabled, the **[!UICONTROL Enable download acceleration]** check box is selected by default.

     ![](assets/download-dialog.png)

     >[!NOTE]
     >
     >If the downloading assets are image files, and you select only the **[!UICONTROL Asset(s)]** check box in the **[!UICONTROL Download]** dialog but are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) then no image files are downloaded and a notification appears, stating that you have been restricted by the administrator to access original renditions.

     ![](assets/restrictaccess-note.png)

1. To download the renditions in addition to the original assets, select the **[!UICONTROL Rendition(s)]** check box. However, if you want to download the system-generated renditions along with the custom renditions, clear the **[!UICONTROL Exclude System Renditions]** check box.

   ![](assets/download-system-rendition.png)

   * To download only the renditions, clear the **[!UICONTROL Asset(s)]** check box.

     >[!NOTE]
     >
     >By default, only the assets are downloaded. However, original renditions of image files are not downloaded if you are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

    * To share the selected assets with other users through a link, select the **[!UICONTROL Email]** check box. An email notification is sent to the users with the download link. To know how to download assets from shared links, see [downloading assets from shared links](../using/brand-portal-link-share.md#main-pars-header-1703469193).  

      ![](assets/download-link.png)

      >[!NOTE]
      >
      >The download link on email notification expires after 45 days.
      >
      >The administrators can customize email messages, that is, logo, description, and footer, using the [Branding](../using/brand-portal-branding.md) feature.


    * You can select a predefined image preset or create a custom dynamic rendition from the **[!UICONTROL Download]** dialog box. 

      To apply a [custom image preset to the asset and its renditions](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), select the **[!UICONTROL Dynamic Rendition(s)]** check box. Specify the image preset properties (such as size, format, color space, resolution, and image modifier) to apply the custom image preset while downloading the asset and its renditions. To download only the dynamic renditions, clear the **[!UICONTROL Asset(s)]** check box.

      ![](assets/dynamic-rendition.png)

      >[!NOTE]
      >
      >Brand Portal supports configuring Dynamic Media in both - Hybird and Scene 7 mode. 
      >
      >(*If AEM author instance is running on **Dynamic Media Hybrid mode***)
      >
      >To preview or download dynamic renditions of an asset, ensure that the dynamic media is enabled and the asset's Pyramid tiff rendition exists at the AEM Assets author instance from where the assets have been published. When an asset is published to Brand Portal, its Pyramid tiff rendition is also published.
      
  
    * To preserve the Brand Portal folder hierarchy while downloading assets, select the **[!UICONTROL Create separate folder for each asset]** check box. By default, the Brand Portal folder hierarchy is ignored and all the assets are downloaded in one folder in your local system.

1. Click **[!UICONTROL Download]**.

   The assets (and renditions if selected) are downloaded as a zip file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions. 

   If you are not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), the original renditions of the selected assets are not downloaded. 

   >[!NOTE]
   >
   >Assets that are individually downloaded are visible in the assets download report. However, if a folder containing assets is downloaded, the folder and assets are not displayed in the assets download report.
-->

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

