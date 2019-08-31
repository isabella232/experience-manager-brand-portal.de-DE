---
title: Freigeben von Assets als Link
seo-title: Freigeben von Assets als Link
description: AEM Assets Brand Portal-Administratoren können Links mehrerer Assets für autorisierte interne Benutzer und externe Einheiten (einschließlich Partnern und Anbietern) freigeben. Bearbeiter können nur die Assets anzeigen und freigeben, die für sie freigegeben wurden.
seo-description: AEM Assets Brand Portal-Administratoren können Links mehrerer Assets für autorisierte interne Benutzer und externe Einheiten (einschließlich Partnern und Anbietern) freigeben. Bearbeiter können nur die Assets anzeigen und freigeben, die für sie freigegeben wurden.
uuid: 8889 ac 24-c 56 d -4 a 47-b 792-80 c 34 ffb 5 c 3 f
contentOwner: bdhar
content-type: Referenz
topic-tags: Freigabe
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: f 3573219-3 c 58-47 ba -90 db -62 b 003 d 8 b 9 aa
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Freigeben von Assets als Link {#share-assets-as-a-link}

AEM Assets Brand Portal-Administratoren können Links mehrerer Assets für autorisierte interne Benutzer und externe Einheiten (einschließlich Partnern und Anbietern) freigeben. Bearbeiter können nur die Assets anzeigen und freigeben, die für sie freigegeben wurden.

Die Freigabe von Assets über einen Link bietet eine praktische Möglichkeit, diese für externe Parteien zur Verfügung zu stellen, da sich die Empfänger nicht bei Brand Portal anmelden müssen, um auf die Assets zuzugreifen.

Der Zugriff auf Linkfreigaben ist auf Bearbeiter und Administratoren beschränkt. For more information, see [Managing users, groups, and user roles](../using/brand-portal-adding-users.md#manage-user-roles).

>[!NOTE]
>
>Auf 5 GB Postload-Download ist über die Linkfreigabe in Brand Portal zulässig.

Führen Sie folgende Schritte aus, um Elemente als Link freizugeben:

1. Klicken Sie links auf das Überlagerungssymbol und wählen Sie dann **[!UICONTROL Navigation]**.

   ![](assets/siderail.png)

2. From the siderail on the left, click **[!UICONTROL Files]** to share folders or images. To share collections, click **[!UICONTROL Collections]**.

   ![](assets/navigationrail.png)

3. Wählen Sie die Ordner oder Sammlungen aus, die Sie als Link freigeben möchten.

   ![](assets/asset-link-share.png)

4. From the toolbar at the top, click the **[!UICONTROL Share Link]** icon.

   The **[!UICONTROL Link Sharing]** dialog box appears.

   ![](assets/link-sharing.png)

   >[!NOTE]
   >
   >The **[!UICONTROL Share Link]** field displays an automatically created asset link. Standardmäßig läuft der Link nach 7 Tagen ab. Sie können den Link kopieren und separat an Benutzer weitergeben oder ihn über das Dialogfeld **[!UICONTROL Linkfreigabe]freigeben.**

5. Geben Sie im Feld „E-Mail-Adresse“ die E-Mail-Adresse des Benutzers ein, für den Sie den Link freigeben möchten. Sie können den Link für mehrere Benutzer freigeben.

   Wenn der Benutzer zu Ihrem Unternehmen gehört, wählen Sie die E-Mail-Adresse des Benutzers in den vorgeschlagenen Dropdown-Listeneinträgen aus. If the user is external, type the complete email ID and press **[!UICONTROL Enter]**; the email ID is added to the list of users.

   ![](assets/link-sharing-text.png)

6. In the **[!UICONTROL Subject]** box, type a subject for the asset you want to share.
7. In the **[!UICONTROL Message]** box, type a message if necessary.
8. In the **[!UICONTROL Expiration]** field, use the date picker to specify an expiration date and time for the link. Standardmäßig ist das Ablaufdatum auf 7 Tage nach dem Datum der Linkfreigabe gesetzt.

   The assets shared through the link expire after crossing the date and time specified in the **[!UICONTROL Expiration]** field. For information about the behavior of expired assets and changes in the permissible activities based on user roles in Brand Portal, see [Manage digital rights of assets](../using/manage-digital-rights-of-assets.md#asset-expiration).

9. Klicken Sie auf **[!UICONTROL Freigeben]**. Eine Meldung bestätigt, dass der Link für die Benutzer freigegeben wurde. Benutzer erhalten eine E-Mail mit dem Link.

   ![](assets/link-sharing-email.png)

   >[!NOTE]
   >
   >Administratoren können die E-Email-Nachrichten anpassen, die das Anpassen von Logo, Beschreibung und Fußzeile mit [Branding](../using/brand-portal-branding.md) -Funktionen beinhalten.

## Herunterladen von Assets von freigegebenen Links {#download-assets-from-shared-links}

Klicken Sie auf den Link in der E-Mail, um das freigegebene Asset anzuzeigen. Die Seite „AEM-Linkfreigabe“ wird geöffnet.

So laden Sie die freigegebenen Assets herunter:

1. Click the assets and then click **[!UICONTROL Download]** icon from the toolbar.

   ![](assets/assets-shared-link.png)

   >[!NOTE]
   >
   >Derzeit können Sie je nach Dateiformat eine Vorschau und eine Miniaturansicht nur für bestimmte Assets erstellen. Weitere Informationen zu den unterstützen Dateiformaten finden Sie unter [Unterstützte Vorschauen und Miniaturen für Asset-Formate](#preview-thumbnail-support).

   >[!NOTE]
   >
   >Wenn die Assets, die Sie herunterladen, auch lizenzierte Assets enthalten, werden Sie zur Seite **[!UICONTROL Copyright-Management]weitergeleitet.** In this page, select the licensed assets, click **[!UICONTROL Agree]**, and then click **[!UICONTROL Download]**. Wenn Sie ablehnen, werden nur die nicht lizenzierten Assets heruntergeladen.\
   >License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in [!DNL AEM Assets].

   ![](assets/licensed-asset-download.png)

   The [!UICONTROL Download] dialog box appears.
   ![](assets/download-linkshare.png)

   * To speed up the download of asset files shared as the link, select **[!UICONTROL Enable download acceleration]** option and [follow the wizard](../using/accelerated-download.md#download-workflow-using-file-accelerator). To know more about the fast download of assets on Brand Portal refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).
[! UICONTROL
2. To download the renditions of assets in addition to the assets from the shared link, select **[!UICONTROL Rendition(s)]** option. **Wenn Sie dies tun, wird** die Option "Systemdarstellungen ausschließen" standardmäßig aktiviert. Dies verhindert, dass vorkonfigurierte Ausgabeformate zusammen mit genehmigten Assets oder deren benutzerdefinierten Ausgabeformaten heruntergeladen werden.

   However, to allow auto-generated renditions to download along with custom renditions, deselect the **[!UICONTROL Exclude System Renditions]** option.

   >[!NOTE]
   >
   >Original renditions are not downloaded using the shared link if the user who shared the assets as a link is not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).

   ![](assets/download-linkshare-autoren.png)

3. Tap/ click **[!UICONTROL Download]**. Die Assets (und Ausgabeformate, sofern ausgewählt) werden als ZIP-Datei in Ihren lokalen Ordner heruntergeladen. Es wird jedoch keine ZIP-Datei erstellt, wenn ein einzelnes Asset ohne eines der Ausgabeformate heruntergeladen wird. Dies gewährleistet einen schnellen Download.

>[!NOTE]
>
>Brand Portal verhindert das Herunterladen von Assets mit einer Dateigröße von mehr als 5 GB.

## Unterstützte Vorschauen und Miniaturen für Asset-Formate {#preview-thumbnail-support}

Die folgende Matrix listet die Asset-Formate auf, für die Brand Portal Miniaturen und Vorschauen unterstützt:

| Asset-Format | Miniatur-Unterstützung | Vorschau-Unterstützung |
|--------------|-------------------|-----------------|
| PNG | ✓ | ✓ |
| GIF | ✓ | ✓ |
| TIFF | ✓ | ✕ |
| JPEG | ✓ | ✓ |
| BMP | ✓ | ✕ |
| PNM* | nicht vorhanden | nicht vorhanden |
| PGM* | nicht vorhanden | nicht vorhanden |
| PBM* | nicht vorhanden | nicht vorhanden |
| PPM* | nicht vorhanden | nicht vorhanden |
| PSD | ✓ | ✕ |
| EPS | nicht vorhanden | ✕ |
| DNG | ✓ | ✕ |
| PICT | ✓ | ✕ |
| PSB* | ✓ | ✕ |
| JPG | ✓ | ✓ |
| AI | ✓ | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| ODT* | ✕ | ✕ |
| PDF | ✓ | ✕ |
| HTML | ✕ | ✕ |
| RTF | ✕ | ✕ |
| TXT | ✓ | ✕ |
| XLS | ✕ | ✕ |
| XLSX | ✕ | ✕ |
| ODS | ✕ | ✕ |
| PPT | ✓ | ✕ |
| PPTX | ✕ | ✕ |
| ODP | ✕ | ✕ |
| INDD | ✓ | ✕ |
| PS | ✕ | ✕ |
| QXP | ✕ | ✕ |
| EPUB | ✓ | ✕ |
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
| JAR | ✓ | ✕ |
| RAR | nicht vorhanden | ✕ |
| TAR | nicht vorhanden | ✕ |
| ZIP | ✓ | ✕ |

Die folgende Legende erläutert die in der Matrix verwendeten Symbole:

| Symbol | Bedeutung |
|---|---|
| ✓ | Dieses Dateiformat unterstützt diese Funktion. |
| ✕ | Dieses Dateiformat unterstützt diese Funktion nicht |
| nicht vorhanden | Diese Funktion kann auf dieses Dateiformat nicht angewendet werden |
| * | Nach der Veröffentlichung der Assets in Brand Portal ist für diese Funktion Add-on-Unterstützung für dieses Dateiformat in der AEM-Autoreninstanz erforderlich, jedoch nicht in Brand Portal |

## Aufheben der Freigabe von Assets als Link {#unshare-assets-shared-as-a-link}

Gehen Sie wie folgt vor, um die Freigabe eines Assets als Link aufzuheben:

1. To view the assets you shared as links, click the overlay icon on the left, and choose **[!UICONTROL Navigation]**.

   ![](assets/siderail.png)

2. From the siderail, click **[!UICONTROL Shared Links]**.

   ![](assets/navigationrail.png)

3. Überprüfen Sie die freigegebenen Links, die in der Liste angezeigt werden.
4. To unshare a link from the list, select it and click the bin icon next to the link entry, or the **[!UICONTROL Unshare]** icon from the toolbar at the top.

   ![](assets/unshare-links.jpg)

   >[!NOTE]
   >
   >Die Anzeige der freigegebenen Links ist benutzerdefiniert. Die Funktion zeigt nicht alle Links an, die von allen Benutzern eines Mandanten freigegebenen werden.

5. In the warning message box, click **[!UICONTROL Continue]** to confirm unshare. Der Eintrag für den Link wird aus der Liste freigegebener Links entfernt.
