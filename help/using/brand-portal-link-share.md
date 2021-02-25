---
title: Freigeben von Assets als Link
seo-title: Freigeben von Assets als Link
description: AEM Assets Brand Portal-Administratoren können Links mehrerer Assets für autorisierte interne Benutzer und externe Einheiten (einschließlich Partnern und Anbietern) freigeben. Bearbeiter können nur die Assets anzeigen und freigeben, die für sie freigegeben wurden.
seo-description: AEM Assets Brand Portal-Administratoren können Links mehrerer Assets für autorisierte interne Benutzer und externe Einheiten (einschließlich Partnern und Anbietern) freigeben. Bearbeiter können nur die Assets anzeigen und freigeben, die für sie freigegeben wurden.
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
translation-type: tm+mt
source-git-commit: fab0855e8d30e7b6ddf9b4ae5b2ce1fb627c81ce
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 70%

---


# Freigeben von Assets als Link {#share-assets-as-a-link}

Adobe Experience Manager Assets Brand Portal-Administratoren können Links mehrerer Assets für autorisierte interne Benutzer und externe Entitäten, einschließlich Partner und Anbieter, freigeben. Bearbeiter können nur die Assets anzeigen und freigeben, die für sie freigegeben wurden.

Die Freigabe von Assets über einen Link ist eine praktische Methode, um die Assets für externe Parteien verfügbar zu machen, ohne dass diese sich bei Brand Portal anmelden müssen.

<!-- Link sharing access is restricted to editors and administrators. 
-->

Weitere Informationen finden Sie unter [Verwalten von Benutzern, Gruppen und Benutzerrollen](../using/brand-portal-adding-users.md#manage-user-roles).

>[!NOTE]
>
>Mit der Linkfreigabe-Funktion in Brand Portal können ZIP-Dateien mit bis zu 5 GB heruntergeladen werden.


Im Folgenden werden die Schritte zum Freigeben von Assets als Link beschrieben:

1. Melden Sie sich bei Ihrem Markenportal-Mandanten an. Standardmäßig wird die Ansicht **[!UICONTROL Files]** geöffnet, die alle veröffentlichten Assets und Ordner enthält.

1. Wählen Sie die Assets oder Ordner aus, die Sie freigeben möchten, oder navigieren Sie zur Ansicht **[!UICONTROL Kollektionen]**, um die erstellten Sammlungen freizugeben.

   ![select-multiple-assets](assets/select-assets-new.png)

1. Klicken Sie oben in der Symbolleiste auf das Symbol **[!UICONTROL Linkfreigabe]**.

   Das Dialogfeld **[!UICONTROL Linkfreigabe]** wird angezeigt.

   ![](assets/link-sharing.png)

   * Geben Sie im Feld „E-Mail-Adresse“ die E-Mail-Adresse des Benutzers ein, für den Sie den Link freigeben möchten. Sie können den Link für mehrere Benutzer freigeben. Wenn der Benutzer zu Ihrem Unternehmen gehört, wählen Sie die E-Mail-Adresse des Benutzers in den vorgeschlagenen Dropdown-Listeneinträgen aus. Wenn es sich um einen externen Benutzer handelt, geben Sie die vollständige E-Mail-Adresse ein und drücken Sie die **[!UICONTROL Eingabetaste]**. Die E-Mail-Adresse wird der Liste der Benutzer hinzugefügt.

      ![](assets/link-sharing-text.png)

   * Geben Sie in das Feld **[!UICONTROL Betreff]** einen Betreff für das freizugebende Asset ein.
   * Geben Sie bei Bedarf eine Nachricht in das Feld **[!UICONTROL Nachricht]** ein.
   * Verwenden Sie im Feld **[!UICONTROL Ablauf]** die Datumsauswahl, um Ablaufdatum und -uhrzeit für den Link festzulegen. Standardmäßig ist das Ablaufdatum auf 7 Tage nach dem Datum der Linkfreigabe gesetzt.
   * Aktivieren Sie das Kontrollkästchen **[!UICONTROL Herunterladen der Originaldatei]** zulassen, damit die Empfänger die ursprüngliche Darstellung herunterladen können.

   Die über den Link freigegebenen Assets laufen nach dem Datum und der Uhrzeit ab, die im Feld **[!UICONTROL Ablauf]** angegeben sind. Informationen zum Verhalten abgelaufener Assets und Änderungen bei den zulässigen Aktivitäten basierend auf den Benutzerrollen in Brand Portal finden Sie unter [Digital Rights Management für Assets](../using/manage-digital-rights-of-assets.md#asset-expiration).

   >[!NOTE]
   >
   >Die standardmäßige Ablaufzeit für den Link beträgt 7 Tage. Der Link muss mit dem Dialogfeld **[!UICONTROL Linkfreigabe]** per E-Mail an die Benutzer gesendet werden. Kopieren Sie den Link nicht und geben Sie ihn nicht separat frei.

1. Klicken Sie auf **[!UICONTROL Freigeben]**. Eine Meldung bestätigt, dass der Link für die Benutzer freigegeben wurde. Benutzer erhalten eine E-Mail mit dem freigegebenen Link.

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >Administratoren können die E-Mail-Nachrichten anpassen. Dies umfasst das Anpassen von Logo, Beschreibung und Fußzeile mit der Funktion [Branding](../using/brand-portal-branding.md).

## Herunterladen von Assets von freigegebenen Links {#download-assets-from-shared-links}

Klicken Sie auf den Link in der E-Mail, um auf das freigegebene Asset zuzugreifen. Die Seite „AEM-Linkfreigabe“ wird geöffnet.

Gehen Sie wie folgt vor, um die freigegebenen Assets herunterzuladen:

1. Klicken Sie auf die Assets oder Ordner und klicken Sie dann in der Symbolleiste auf das Symbol **[!UICONTROL Herunterladen]**.

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >Derzeit können Sie je nach dem jeweiligen Dateiformat nur für bestimmte Assets eine Vorschau und Miniaturen generieren. Weitere Informationen zu den unterstützen Dateiformaten finden Sie unter [Unterstützte Vorschauen und Miniaturen für Asset-Formate](#preview-thumbnail-support).

1. Das Dialogfeld **[!UICONTROL Download]** wird angezeigt.

   ![download-dialog](assets/download-dialog-box-new.png)

1. Standardmäßig ist die Einstellung **[!UICONTROL Schneller Download]** in **[!UICONTROL Download-Einstellungen]** aktiviert. Daher wird das Herunterladen mit IBM Aspera Connect über ein Bestätigungsfeld fortgesetzt.

   Um weiterhin **[!UICONTROL Schnelles Herunterladen]** zu verwenden, klicken Sie auf **[!UICONTROL Zulassen]**.

   Alle ausgewählten Darstellungen werden in einen ZIP-Ordner heruntergeladen, der einen separaten Ordner für jedes Asset enthält.

   >[!NOTE]
   >
   >Wenn ein Ordner, eine Sammlung oder mehr als 20 Assets zum Herunterladen ausgewählt sind, wird das Dialogfeld **[!UICONTROL Herunterladen]** übersprungen und alle für den Benutzer verfügbaren Asset-Darstellungen mit Ausnahme der dynamischen Darstellungen werden in einen ZIP-Ordner heruntergeladen. Für jedes Asset im ZIP-Ordner wird ein eigener Ordner erstellt.

   >[!NOTE]
   >
   >Original-Ausgabeformate werden nicht über den freigegebenen Link heruntergeladen, wenn der Benutzer, der die Assets als Link freigegeben hat, nicht [vom Administrator autorisiert wurde, auf die Original-Ausgabeformate zuzugreifen](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).


>[!NOTE]
>
>Brand Portal verhindert das Herunterladen von Assets mit einer Dateigröße von mehr als 5 GB.

<!--
1. The **[!UICONTROL Download]** dialog box appears.

   ![](assets/download-linkshare.png)

    * To speed up the download of asset files shared as the link, select **[!UICONTROL Enable download acceleration]** option and [follow the wizard](../using/accelerated-download.md#download-workflow-using-file-accelerator). To know more about the fast download of assets on Brand Portal refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).
    
1. To download the renditions of assets in addition to the assets from the shared link, select **[!UICONTROL Rendition(s)]** option. When you do so, **[!UICONTROL Exclude System Renditions]** option appears that is selected by default. This prevents the download of out-of-the-box renditions along with approved assets or their custom renditions.

   However, to allow auto-generated renditions to download along with custom renditions, deselect the **[!UICONTROL Exclude System Renditions]** option.

   >[!NOTE]
   >
   >Original renditions are not downloaded using the shared link if the user who shared the assets as a link is not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).

   ![](assets/download-linkshare-autoren.png)

1. Click **[!UICONTROL Download]**. The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

>[!NOTE]
>
>Brand Portal restricts downloading assets larger than 5GB per file size.
-->

## Unterstützte Vorschauen und Miniaturen für Asset-Formate {#preview-thumbnail-support}

Die folgende Matrix listet die Asset-Formate auf, für die Brand Portal Miniaturen und Vorschauen unterstützt:

| Asset-Format | Miniatur-Unterstützung | Vorschau-Unterstützung |
|--------------|-------------------|-----------------|
| PNG | ✓ | they |
| GIF | they | they |
| TIFF | they | ✕ |
| JPEG | they | they |
| BMP | they | ✕ |
| PNM* | nicht vorhanden | nicht vorhanden |
| PGM* | nicht vorhanden | nicht vorhanden |
| PBM* | nicht vorhanden | nicht vorhanden |
| PPM* | nicht vorhanden | nicht vorhanden |
| PSD | they | ✕ |
| EPS | nicht vorhanden | ✕ |
| DNG | they | ✕ |
| PICT | they | ✕ |
| PSB* | they | ✕ |
| JPG | they | they |
| AI | they | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| ODT* | ✕ | ✕ |
| PDF | they | ✕ |
| HTML | ✕ | ✕ |
| RTF | ✕ | ✕ |
| TXT | they | ✕ |
| XLS | ✕ | ✕ |
| XLSX | ✕ | ✕ |
| ODS | ✕ | ✕ |
| PPT | they | ✕ |
| PPTX | ✕ | ✕ |
| ODP | ✕ | ✕ |
| INDD | they | ✕ |
| PS | ✕ | ✕ |
| QXP | ✕ | ✕ |
| EPUB | they | ✕ |
| AAC | ✕ | ✕ |
| MIDI | ✕ | ✕ |
| 3GP | ✕ | ✕ |
| MP3 | ✕ | ✕ |
| MP4 | ✕ | ✕ |
| OGA | ✕ | ✕ |
| OGG | ✕ | ✕ |
| RA | ✕ | ✕ |
| WAV | ✕ | ✕ |
| WMA | ✕ | ✕ |
| DVI | ✕ | ✕ |
| FLV | ✕ | ✕ |
| M4V | ✕ | ✕ |
| MPG | ✕ | ✕ |
| OGV | ✕ | ✕ |
| MOV | ✕ | ✕ |
| WMV | ✕ | ✕ |
| SWF | ✕ | ✕ |
| TGZ | nicht vorhanden | ✕ |
| JAR | they | ✕ |
| RAR | nicht vorhanden | ✕ |
| TAR | nicht vorhanden | ✕ |
| ZIP | they | ✕ |

Die folgende Legende erläutert die in der Matrix verwendeten Symbole:

| Symbol | Bedeutung |
|---|---|
| they | Dieses Dateiformat unterstützt diese Funktion |
| ✕ | Dieses Dateiformat unterstützt diese Funktion nicht |
| nicht vorhanden | Diese Funktion kann auf dieses Dateiformat nicht angewendet werden |
| * | Nach der Veröffentlichung der Assets in Brand Portal ist für diese Funktion Add-on-Unterstützung für dieses Dateiformat in der AEM-Autoreninstanz erforderlich, jedoch nicht in Brand Portal |

## Aufheben der Freigabe von Assets als Link {#unshare-assets-shared-as-a-link}

Gehen Sie wie folgt vor, um die Freigabe eines Assets als Link aufzuheben:

1. Wenn Sie sich beim Markenportal anmelden, wird standardmäßig die Ansicht **[!UICONTROL File]** geöffnet. Um die Assets, die Sie als Links freigegeben haben, Ansicht, navigieren Sie zur Ansicht **[!UICONTROL Freigegebene Links]**.

1. Überprüfen Sie die freigegebenen Links, die in der Liste angezeigt werden.

   ![](assets/shared-links.png)

1. Um die Freigabe eines Links aus der Liste aufzuheben, wählen Sie ihn aus und klicken Sie auf das Symbol **[!UICONTROL Freigabe aufheben]** in der Symbolleiste oben.

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >Die Anzeige der freigegebenen Links ist benutzerdefiniert. Die Funktion zeigt nicht alle Links an, die von allen Benutzern eines Mandanten freigegebenen werden.

1. Klicken Sie in der Warnmeldung auf **[!UICONTROL Weiter]**, um das Aufheben der Freigabe zu bestätigen. Der Eintrag für den Link wird aus der Liste freigegebener Links entfernt.
