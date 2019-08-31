---
title: Anwenden von Bildvorgaben oder dynamischen Ausgabeformaten
seo-title: Anwenden von Bildvorgaben oder dynamischen Ausgabeformaten
description: 'Wie ein Makro ist eine Bildvorgabe eine vordefinierte Sammlung aus Größenangaben und Formatierungsbefehlen, die unter einem Namen gespeichert wird. Mithilfe von Bildvorgaben kann AEM Assets Brand Portal Bilder in unterschiedlichen Größen, Formaten und Eigenschaften dynamisch liefern. '
seo-description: 'Wie ein Makro ist eine Bildvorgabe eine vordefinierte Sammlung aus Größenangaben und Formatierungsbefehlen, die unter einem Namen gespeichert wird. Mithilfe von Bildvorgaben kann AEM Assets Brand Portal Bilder in unterschiedlichen Größen, Formaten und Eigenschaften dynamisch liefern. '
uuid: a 3 c 8705 c -5 fbd -472 c -8 b 61-f 65 b 3 e 552 c 1 b
content-type: Referenz
topic-tags: Administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: a 512 dfa 0-fef 3-4 c 3 f-a 389-a 0 a 3 a 7415 bac
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Anwenden von Bildvorgaben oder dynamischen Ausgabeformaten {#apply-image-presets-or-dynamic-renditions}

Wie ein Makro ist eine Bildvorgabe eine vordefinierte Sammlung aus Größenangaben und Formatierungsbefehlen, die unter einem Namen gespeichert wird. Mithilfe von Bildvorgaben kann AEM Assets Brand Portal Bilder in unterschiedlichen Größen, Formaten und Eigenschaften dynamisch liefern.

Bildvorgaben werden verwendet, um dynamische Ausgabeformate von Bildern zu generieren, die als Vorschau angezeigt oder heruntergeladen werden können. Wenn Sie eine Vorschau von Bildern und deren Ausgabeformaten anzeigen, können Sie eine Vorgabe auswählen, um Bilder gemäß den Spezifikationen Ihres Administrators umzuformatieren.

Um dynamische Darstellungen eines Assets in Brand Portal anzuzeigen, stellen Sie sicher, dass die Pyramid-TIFF-Darstellung auf der AEM-Autoreninstanz vorhanden ist, von der aus Sie in Brand Portal veröffentlichen. Wenn Sie das Asset veröffentlichen, wird auch dessen PTIFF-Ausgabeformat in Brand Portal veröffentlicht. Es gibt keine Möglichkeit, das PTIFF-Ausgabeformat in Brand Portal zu generieren.

>[!NOTE]
>
>Beim Herunterladen von Bildern und deren Ausgabeformaten gibt es keine Möglichkeit, aus den vorhandenen Vorgaben auszuwählen. Stattdessen können Sie die Eigenschaften für eine benutzerdefinierte Bildvorgabe festlegen. Weitere Informationen finden Sie unter [Anwenden von Bildvorgaben beim Herunterladen von Bildern](../using/brand-portal-image-presets.md#main-pars-text-1403412644).

Weitere Informationen zu den Parametern, die für das Erstellen von Bildvorgaben erforderlich sind, finden Sie unter [Verwalten von Bildvorgaben](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html).

## Erstellen von Bildvorgaben {#create-an-image-preset}

Administratoren können Bildvorgaben erstellen, die auf der Asset-Detailseite als dynamische Ausgabeformate angezeigt werden. Sie können völlig neue Bildvorgaben erstellen oder eine vorhandene Vorgabe unter einem neuen Namen speichern. Wenn Sie Bildvorgaben erstellen, wählen Sie eine Größe für die Bildbereitstellung und die Formatierungsbefehle aus. Wenn ein Bild für die Anzeige bereitgestellt wird, wird die Darstellung entsprechend den ausgewählten Befehlen optimiert.
Nur Administratoren können Bildvorgaben in Brand Portal erstellen.

Nur Administratoren können Bildvorgaben in Brand Portal erstellen.

>[!NOTE]
>
>Dynamische Ausgabeformate werden für Assets erstellt, für die PTIFF verfügbar ist. Wenn also für ein Asset kein Pyramid TIFF-Ausgabeformat in AEM erstellt und in Brand Portal veröffentlicht wird, können nur die zugehörigen Systemausgaben exportiert werden. Dynamische Ausgabeformate werden aber als Option angezeigt.
Der Dynamic Media Hybrid-Modus muss in AEM (Autoreninstanz) aktiviert sein, damit das Pyramid TiFF (PTIFF)-Format eines Assets erstellt werden kann. Wenn ein solches Asset in Brand Portal veröffentlicht wird, werden Bildvorgaben angewendet und dynamische Darstellungen angezeigt.

1. Klicken Sie in der AEM-Symbolleiste oben auf das Adobe-Logo, um auf Verwaltungswerkzeuge zuzugreifen.

   ![](assets/AEMlogo.png)

2. From the administrative tools panel, click **[!UICONTROL Image Presets]**.

   ![](assets/admin-tools-panel-4.png)

3. Klicken Sie auf der Seite „Bildvorgaben“ auf **[!UICONTROL Erstellen]**.

   ![](assets/image_preset_homepage.png)

4. In the **[!UICONTROL Edit Image Preset]** page, enter values into the **[!UICONTROL Basic]** and **[!UICONTROL Advanced]** tabs as appropriate, including a name. Die Optionen werden in den Optionen für die [Bildvorgabe](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options) hervorgehoben. Vorgaben werden im linken Bereich angezeigt und können nur zusammen mit anderen Assets verwendet werden.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >You can also use the **[!UICONTROL Edit Image Preset]** page to edit the properties of an existing image preset. To edit an image preset, select it from the image presets page, and click **[!UICONTROL Edit]**.

5. Klicken Sie auf **[!UICONTROL Speichern]**. Die Bildvorgabe wird erstellt und auf der Seite „Bildvorgaben“ angezeigt.
6. Um eine Bildvorgabe zu löschen, wählen Sie sie auf der Seite „Bildvorgaben“ aus und klicken Sie auf **[!UICONTROL Löschen]**. Klicken Sie auf der Bestätigungsseite auf **[!UICONTROL Löschen], um den Vorgang zu bestätigen.** Die Bildvorgabe wird von der Seite „Bildvorgaben“ entfernt.

## Anwenden von Bildvorgaben beim Anzeigen der Bildvorschau  {#apply-image-presets-when-previewing-images}

Wenn Sie eine Vorschau von Bildern und deren Ausgabeformaten anzeigen, können Sie eine vorhandene Vorgabe auswählen, um Bilder gemäß den Spezifikationen Ihres Administrators umzuformatieren.

1. Klicken Sie auf der Marken-Portal-Oberfläche auf ein Bild, um es zu öffnen.
2. Click the overlay icon on the left, and choose **[!UICONTROL Renditions]**.

   ![](assets/image-preset-previewrenditions.png)

3. From the **[!UICONTROL Renditions]** list, select the appropriate dynamic rendition, for example, **[!UICONTROL Thumbnail]**. Das Vorschaubild wird basierend auf Ihrer Auswahl des Ausgabeformats dargestellt.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Anwenden von Bildvorgaben beim Herunterladen von Bildern {#apply-image-presets-when-downloading-images}

Beim Herunterladen von Bildern und deren Darstellungen aus dem Markenportal können Sie nicht aus den vorhandenen Bildvorgaben auswählen. Sie können jedoch die Bildvorgabeneigenschaften anpassen, damit Sie die gewünschten Bilder neu formatieren können.

1. Führen Sie auf der Marken-Portal-Oberfläche einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über das Bild, das Sie herunterladen möchten. From the quick action thumbnails available, click the **[!UICONTROL Download]** icon.
   ![](assets/downloadsingleasset.png)

   * Wählen Sie das Bild aus, das Sie herunterladen möchten. From the toolbar at the top, click the **[!UICONTROL Download]** icon.
   ![](assets/downloadassets.png)

2. Wählen Sie im Dialogfeld **[!UICONTROL Herunterladen]die erforderlichen Optionen aus, je nachdem, ob Sie das Asset mit oder ohne dessen Ausgabeformate herunterladen möchten.**

   ![](assets/donload-assets-dialog.png)

3. Um dynamische Ausgabeformate der Assets herunterzuladen, wählen Sie die Option **[!UICONTROL Dynamische Ausgabe(n)]aus.**
4. Sie können jedoch auch die Bildvorgabeneigenschaften anpassen, damit Sie die gewünschten Bilder und deren Ausgabeformate beim Herunterladen dynamisch neu formatieren können. Geben Sie hierfür Größe, Format, Farbraum, Auflösung und Bild-Modifikator an.

   ![](assets/dynamicrenditions.png)

5. Klicken Sie auf **[!UICONTROL Herunterladen]**. Die dynamischen Ausgabeformate werden in einer ZIP-Datei zusammen mit dem Bild sowie dessen Ausgabeformaten, die Sie herunterladen möchten, heruntergeladen. Wenn nur ein Asset heruntergeladen wird, wird jedoch keine Zip-Datei erstellt, um den Download zu beschleunigen.
