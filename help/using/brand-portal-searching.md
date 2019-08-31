---
title: Suchen von Assets in Brand Portal
seo-title: Asset-Suche und gespeicherte Suche in AEM Brand Portal
description: Mit der Brand Portal-Suchfunktion können Sie schnell mithilfe von Omnisearch nach relevanten Assets suchen. Mit Suchfiltern können Sie die Suche weiter einschränken. Speichern Sie Ihre Suchen als Smart-Sammlungen, um sie später wiederverwenden zu können.
seo-description: Mit der Brand Portal-Suchfunktion können Sie schnell mithilfe von Omnisearch nach relevanten Assets suchen. Mit Suchfiltern können Sie die Suche weiter einschränken. Speichern Sie Ihre Suchen als Smart-Sammlungen, um sie später wiederverwenden zu können.
uuid: c 2955198-bdc 0-4853-a 13 a -661 e 6 a 9 ec 61 f
contentOwner: bdhar
content-type: Referenz
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: Searchandpromote
discoiquuid: dc 751 cd 7-f 663-46 d 2-84 c 4-5 bb 12 a 4 fe 1 ba
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Suchen von Assets in Brand Portal {#search-assets-on-brand-portal}

Mit der Suchfunktion für Markenportal können Sie schnell nach relevanten Assets suchen, indem Sie omnisearch verwenden und die Suche mit Filtern nutzen, um die Suche weiter einzuschränken. Sie können Ihre Suchvorgänge als Smart-Sammlungen für die Zukunft speichern.

## Suchen von Assets mithilfe von Omnisearch {#search-assets-using-omnisearch}

So suchen Sie in Brand Portal nach Assets:

1. From the toolbar, click the **[!UICONTROL Search]** icon, or press the "**[!UICONTROL /]**" key to launch Omnisearch.

   ![](assets/omnisearchicon-1.png)

2. Geben Sie in das Suchfeld einen Suchbegriff für die Assets ein, die Sie suchen möchten.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Hierfür sind mindestens 3 Zeichen in Omnisearch erforderlich, damit Suchvorschläge angezeigt werden.

3. Wählen Sie aus den relevanten Vorschlägen in der Dropdown-Liste ein Asset aus, auf das Sie schnell zugreifen möchten.

   ![](assets/assets-search-result.png)

   *Asset-Suche mithilfe von Omnisearch*

## Suche mithilfe von Facetten im Bereich „Filter“{#search-using-facets-in-filters-panel}

Suchfacetten im Bereich „Filter“ fügen Granularität zu Ihrer Suche hinzu und machen die Suchfunktion effizient. Suchfacetten verwenden mehrere Dimensionen (predicates), mit denen Sie komplizierte Suchvorgänge durchführen können. Sie können einfach einen Drilldown zur gewünschten Detailtiefe durchführen, um die Suche zu konzentrieren.

Wenn Sie beispielsweise nach einem Bild suchen, können Sie auswählen, ob Sie ein Bitmap- oder ein Vektorbild möchten. Sie können den Umfang der Suche weiter verringern, indem Sie den MIME-Typ für das Bild in der Dateityp-Suchfacette angeben. Wenn Sie nach Dokumenten suchen, können Sie auf ähnliche Weise das gewünschte Format festlegen, z. B. PDF oder MS Word.

![Filter-Bedienfeld im Marken-portalfilter](assets/file-type-search.png "-Bedienfeld im Markenportal")

The [!UICONTROL Filters] panel includes a few standard facets, such as- [!UICONTROL Path Browser], [!UICONTROL File Type], [!UICONTROL File Size], [!UICONTROL Status], and [!UICONTROL Orientation]. However, you can [add custom search facets](../using/brand-portal-search-facets.md) or remove specific search facets from the [!UICONTROL Filters] panel by adding or removing predicates in the underlying Search Form. See the list of the available and usable [search predicates on Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

To apply filters to your search, using the available [search facets](../using/brand-portal-search-facets.md):

1. Click the overlay icon and select **[!UICONTROL Filter]**.

   ![](assets/selectorrail.png)

2. Wählen Sie im Bereich **[!UICONTROL Filter]auf der linken Seite die entsprechenden Optionen aus, um die relevanten Filter anzuwenden.**
Verwenden Sie beispielsweise die folgenden Standardfilter:

   * **[!UICONTROL Pfad-Browser]** , um Assets in einem bestimmten Verzeichnis zu suchen. The default search path of the predicate for Path Browser is **[!UICONTROL /content/dam/mac/&lt;tenant-id&gt;/]**, which can be configured by editing the default search form.
   >[!NOTE]
   >
   >To non-admin users, [!UICONTROL Path Browser] in [!UICONTROL Filter] panel shows only the content structure of the folders (and their ancestor folders) shared with them.\
   >Für Admin-Benutzer ermöglicht der Path Browser die Navigation zu einem beliebigen Ordner im Brand Portal.

   * **[!UICONTROL Dateityp]** , um den Typ (Bild, Dokument, Multimedia, Archiv) der gesuchten Asset-Datei anzugeben. Darüber hinaus können Sie den Umfang Ihrer Suche einschränken. Geben Sie zum Beispiel den MIME-Typ (TIFF, Bitmap, GIMP-Bilder) für Bilder oder Formate (PDF oder MS Word) für die Dokumente an.
   * **[!UICONTROL Dateigröße]** , um nach Assets basierend auf ihrer Größe zu suchen. Sie können die untere und obere Grenze für den Größenbereich ausgeben, um Ihre Suche einzuschränken und die Maßeinheit für die Suche anzugeben.
   * **[!UICONTROL Status]** , um auf Asset-Status basierende Assets wie Genehmigung (Genehmigt, Änderungen angefordert, Abgelehnt, Ausstehend) und Ablauf zu suchen.
   * **[!UICONTROL Durchschnittliche Bewertung]** zur Suche nach Assets basierend auf der Bewertung der Assets.
   * **[!UICONTROL Ausrichtung]** zur Suche nach Assets basierend auf der Ausrichtung (horizontal, vertikal, quadrat) der Assets.
   * **[!UICONTROL Stil]**, um basierend auf dem Stil (farbig, einfarbig) der Assets nach Assets zu suchen. 
   * **[!UICONTROL Videoformat]**, um basierend auf dem Format von Video-Assets (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM) nach Video-Assets zu suchen.
   Sie können im Bereich „Filter“ [benutzerdefinierte Suchfacetten](../using/brand-portal-search-facets.md) verwenden, indem Sie das zugrunde liegende Suchformular bearbeiten.

   * **[!UICONTROL Wenn im Suchformular verwendet, können Sie mithilfe von Eigenschaftsprädikat]** nach Assets suchen, die mit einer Metadateneigenschaft übereinstimmen, der das Prädikat zugeordnet ist.\
      Wenn beispielsweise Eigenschaftspredicate zugeordnet [!UICONTROL `jcr:content /metadata/dc:title`]ist, können Sie Assets auf Grundlage ihres Titels suchen.\
      Die [!UICONTROL Eigenschaftseigenschaft] unterstützt die Textsuche nach:

      **Unvollständige Begriffe**
Wenn Sie die Asset-Suche mithilfe unvollständiger Suchbegriffe in den Eigenschaften einer Property ermöglichen möchten, aktivieren Sie im Suchformular das Kontrollkästchen **[!UICONTROL Unvollständiger Suchbegriff].**\
      Auf diese Weise können Sie nach gewünschten Assets suchen, selbst wenn Sie nicht den genauen Wortlaut/die genauen Begriffe angeben, die in den Asset-Metadaten verwendet werden.\
      Sie können:
* Geben Sie ein Wort in der gesuchten Wortgruppe in der Facette im Filter-Bedienfeld ein. For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
* Geben Sie einen Teil des Wortes ein, das im Suchbegriff vorkommt, und setzen Sie in die Lücken das Platzhalterzeichen (*) ein.
Beispiel für die Suche nach:
      **climb *** gibt alle Assets zurück, die mit den Zeichen "globb" in ihrem Titelausdruck beginnen.
      *** climb** gibt alle Assets zurück, die mit Zeichen enden, die mit Zeichen "globb" in ihrem Titelausdruck enden.
      *** climb *** gibt alle Assets zurück, die die Zeichen "globb" in ihrem Titelausdruck zusammenfasst.\
      **Für nicht zwischen Groß- und Kleinschreibung basierende Texte**,
um die Groß-/Kleinschreibung in Eigenschaftseigenschaften zuzulassen, aktivieren Sie **[!UICONTROL das Kontrollkästchen "Schreibweise]** ignorieren" im Suchformular. Bei der Textsuche im Eigenschaftsprädikat wird standardmäßig zwischen Groß- und Kleinschreibung unterschieden.
   >[!NOTE]
   >
   >Nach Aktivierung des Kontrollkästchens **[!UICONTROL Teilsuche]** wird [!UICONTROL Groß-/Kleinschreibung ignorieren] standardmäßig aktiviert.

   ![](assets/wildcard-prop-1.png)

   Die Suchergebnisse werden entsprechend den angewendeten Filtern angezeigt, zusammen mit der Anzahl der Suchergebnisse.

   ![](assets/omnisearch-with-filters.png)

   Asset-Suchergebnis mit Suchergebniszählung

3. Sie können einfach zu einem Element in den Suchergebnissen navigieren und mit der Schaltfläche „Zurück“ in Ihrem Browser zum selben Suchergebnis zurückkehren, ohne die Suchabfrage erneut starten zu müssen.

## Suchen als Smart-Sammlung speichern {#save-your-searches-as-smart-collection}

Sie können die Sucheinstellungen als Smart-Sammlung speichern, damit Sie dieselbe Suche zu einem späteren Zeitpunkt wiederholen können, ohne die Einstellungen erneut vornehmen zu müssen.

So speichern Sie die Sucheinstellungen als Smart-Sammlung:

1. Tap/ click **[!UICONTROL Save Smart Collection]** and provide a name for the smart collection.

   Damit die Smart-Sammlung von allen Benutzern verwendet werden kann, aktivieren Sie die Option **[!UICONTROL Öffentlich]**. Eine Meldung bestätigt, dass die Smart-Sammlung erstellt und zur Liste der gespeicherten Suchen hinzugefügt wurde.

   >[!NOTE]
   >
   >Benutzer ohne Administratorrechte können daran gehindert werden, Smart-Sammlungen öffentlich zu machen. So kann verhindert werden, dass Benutzer ohne Administratorrechte eine große Anzahl öffentlicher Smart-Sammlungen im Portal der Organisation erstellen. Organizations can disable the **[!UICONTROL Allow public smart collections creation]** configuration from **[!UICONTROL General]** settings available in admin tools panel.

   ![](assets/save_smartcollectionui.png)

2. Um die Smart-Sammlung unter einem anderen Namen zu speichern, aktivieren oder deaktivieren Sie das Kontrollkästchen **[!UICONTROL Öffentlich]** und klicken Sie auf **[!UICONTROL Smart-Sammlung bearbeiten]**.

   ![](assets/edit_smartcollection.png)

3. Wählen Sie im Dialogfeld **[!UICONTROL Smart-Sammlung bearbeiten]** die Option **Speichern unter]aus und geben Sie einen Namen für die Smart-Sammlung ein.[!UICONTROL ** Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/saveas_smartsearch.png)
