---
title: Verwenden von Metadatenschema-Formularen
seo-title: Verwenden von Metadatenschema-Formularen
description: Ein Metadatenschema beschreibt das Layout der Eigenschaftsseite und die für Assets angezeigten Metadateneigenschaften, die das betreffende Schema verwenden. Mit dem für ein Asset angewendeten Schema legen Sie fest, welche Metadatenfelder auf der Eigenschaftsseite des Assets angezeigt werden.
seo-description: Ein Metadatenschema beschreibt das Layout der Eigenschaftsseite und die für Assets angezeigten Metadateneigenschaften, die das betreffende Schema verwenden. Mit dem für ein Asset angewendeten Schema legen Sie fest, welche Metadatenfelder auf der Eigenschaftsseite des Assets angezeigt werden.
uuid: 1 a 944 a 3 b -5152-425 f-b 1 ea-bfe 3331 de 928
content-type: Referenz
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: Administration
discoiquuid: 500 b 46 da-ef 67-46 a 0-a 069-192 f 4 b 1 a 0 eca
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Verwenden von Metadatenschema-Formularen {#use-the-metadata-schema-form}

Ein Metadatenschema beschreibt das Layout der Eigenschaftsseite und die für Assets angezeigten Metadateneigenschaften, die das betreffende Schema verwenden. Mit dem für ein Asset angewendeten Schema legen Sie fest, welche Metadatenfelder auf der Eigenschaftsseite des Assets angezeigt werden.

The **Properties** page for each asset includes default metadata properties depending upon the MIME type of the asset. Administratoren können den Metadatenschema-Editor verwenden, um vorhandene Schemas zu ändern oder benutzerdefinierte Metadatenschemata hinzuzufügen. [!DNL AEM] Assets [!DNL Brand Portal] enthalten Standardformulare für Assets verschiedener MIME-Typen. Sie können jedoch auch benutzerdefinierte Formulare für solche Assets hinzufügen.

## Hinzufügen von Metadatenschema-Formularen {#add-a-metadata-schema-form}

Gehen Sie wie folgt vor, um ein neues Metadatenschema-Formular zu erstellen:

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **Metadatenschemata**.

   ![](assets/navigation-panel.png)

3. On the **Metadata Schema Forms** page, click **Create**.

   ![](assets/create-metadata-schema-form.png)

4. In the **Create Schema Form** dialog box, specify the title of the Schema form, and then click **Create** to complete the form creation process.

   ![](assets/create-schema-form.png)

## Bearbeiten von Metadatenschema-Formularen {#edit-a-metadata-schema-form}

Sie können ein neu hinzugefügtes oder vorhandenes Metadatenschema-Formular bearbeiten. Das Metadatenschema-Formular enthält aus dem übergeordneten Objekt abgeleitete Inhalte, einschließlich Registerkarten und Formularelementen innerhalb von Registerkarten. Sie können diese Formularelemente einem Feld innerhalb eines Metadatenknotens zuordnen bzw. dafür konfigurieren.

Sie können dem Metadatenschema-Formular neue Registerkarten oder Formularelemente hinzufügen. Die (vom übergeordneten Objekt) abgeleiteten Registerkarten und Formularelemente sind gesperrt. Sie können auf untergeordneter Ebene nicht geändert werden.

Gehen Sie wie folgt vor, um ein Metadatenschema-Formular zu bearbeiten:

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **Metadatenschemata**.
3. From the **Metadata Schema Forms** page, select a schema form to edit its properties, for example, **collection**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >Nicht bearbeitete Vorlagen sind mit einem **Sperrsymbol** gekennzeichnet. Wenn Sie eine Vorlage anpassen, wird das **Sperrsymbol** vor der Vorlage ausgeblendet.

4. Klicken Sie oben in der Symbolleiste auf **Bearbeiten**.

   Die Seite **Metadatenschema-Editor** wird mit der Registerkarte **Allgemein** auf der linken Seite und der Registerkarte **Formular erstellen** auf der rechten Seite geöffnet.

5. In the **Metadata Schema Editor** page, customize the **Properties** page of the asset by dragging one or more components from a list of component types in the **Build Form** tab to the **Basic** tab.

   ![](assets/metadata-schemaeditor-page.png)

6. To configure a component, select it and modify its properties in the **Settings** tab.

### Komponenten auf der Registerkarte „Formular erstellen“{#components-in-the-build-form-tab}

The **Build Form** tab lists items that you can use in your schema form. The **Settings** tab provides the attributes of each item that you select in the **Build Form** tab. The following table lists the form items available in the **Build Form** tab:

| Komponentenname | Beschreibung |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bereichs-Kopfzeile | Fügen Sie eine Abschnittsüberschrift für eine Liste allgemeiner Komponenten hinzu. |
| Einzelzeilentext | Fügen Sie eine einzeilige Texteigenschaft hinzu. Diese wird als Zeichenfolge gespeichert. |
| Text mit mehreren Werten | Fügen Sie eine Texteigenschaft mit mehreren Werten hinzu. Diese wird als Zeichenfolgen-Array gespeichert. |
| Nummer | Fügen Sie eine Zahlenkomponente hinzu. |
| Datum | Fügen Sie eine Datumskomponente hinzu. |
| Dropdown | Fügen Sie eine Dropdownliste hinzu. |
| Standard-Tags | Fügen Sie ein Tag hinzu. **Hinweis:** Administratoren müssen ggf. den Pfadwert ändern, `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`wenn sie das Metadatenschemaformular veröffentlichen, bei [!DNL AEM]`/etc/tags/<custom_tag_namespace>`dem der Pfad beispielsweise keine Mandanten-Informationen enthält. |
| Smart-Tags | Auto-detected tags if you have purchased and configured the [!DNL AEM] smart tags add-on. |
| Ausgeblendetes Feld | Fügen Sie ein ausgeblendetes Feld hinzu. Dieses wird beim Speichern des Assets als POST-Parameter gesendet. |
| Asset referenziert von | Fügen Sie diese Komponente hinzu, um eine Liste der vom Asset referenzierten Assets anzuzeigen. |
| Asset-Verweise | Fügen Sie dies hinzu, um eine Liste der Assets anzuzeigen, die das Asset referenzieren. |
| Asset-Bewertung | Average rating of an asset added from [!DNL AEM] Assets before it is published to [!DNL Brand Portal]. |
| Kontextuelle Metadaten | Zur Steuerung der Anzeige anderer Metadaten auf der Seite Eigenschaften von Assets. |

>[!NOTE]
>
>Do not use **Product References** as it is not functional.

#### Bearbeiten von Metadatenkomponenten {#edit-the-metadata-component}

Um die Eigenschaften einer Metadatenkomponente im Formular zu bearbeiten, klicken Sie auf die Komponente und bearbeiten Sie ihre Eigenschaften auf der Registerkarte **Einstellungen**.

* **Feldbeschriftung**: Der Name der Metadateneigenschaft, die auf der Seite Eigenschaften des Assets angezeigt wird.

* **Zu Eigenschaft zuordnen**: Der Wert dieser Eigenschaft liefert den relativen Pfad/Namen zum Asset-Knoten für dessen Speicherort im CRX-Repository. Sie beginnt mit „**./**“, um anzugeben, dass der Pfad sich unter dem Knoten des Assets befindet.

Im Folgenden finden Sie die gültigen Werte für diese Eigenschaft:

-- `./jcr:content/metadata/dc:title`: Stores the value at the asset's metadata node as the property `dc:title`.

-- `./jcr:created`: Displays the jcr property at the asset's node. Wenn Sie diese Eigenschaften für Ansichtseigenschaften konfigurieren, wird empfohlen, dass Sie sie mit „Bearbeitung deaktivieren“ markieren, da sie geschützt sind. Andernfalls tritt der Fehler „Assets konnten nicht geändert werden“ auf, wenn Sie die Eigenschaften des Assets speichern.

* **Platzhalter**: Mit dieser Eigenschaft können Sie Benutzern relevante Informationen zur Metadateneigenschaft angeben.
* **Erforderlich**: Mit dieser Eigenschaft können Sie eine Metadateneigenschaft auf der Eigenschaftsseite als obligatorisch markieren.
* **Bearbeitung deaktivieren**: Mit dieser Eigenschaft können Sie verhindern, dass eine Metadateneigenschaft auf der Eigenschaftsseite bearbeitet werden kann.
* **Leeres Feld schreibgeschützt anzeigen**: Markieren Sie diese Eigenschaft, um eine Metadateneigenschaft auch dann auf der Eigenschaftsseite anzuzeigen, wenn sie keinen Wert aufweist. Standardmäßig werden Metadateneigenschaften ohne Werte nicht auf der Eigenschaftsseite aufgeführt.
* **Beschreibung**: Mit dieser Eigenschaft können Sie eine kurze Beschreibung für die Metadatenkomponente hinzufügen.
* **Löschen-Symbol**: Klicken Sie auf dieses Symbol, um eine Komponente aus dem Schemaformular zu löschen.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Alle Metadaten-Felder sind im Asset-Editorformular für Metadaten schreibgeschützt. Since metadata of the asset must be edited in [!DNL AEM] Assets before an asset is published to [!DNL Brand Portal].

#### Hinzufügen oder Löschen von Registerkarten im Schemaformular {#add-or-delete-a-tab-in-the-schema-form}

The default schema form includes the **Basic** and **Advanced** tabs. Mit dem Schema-Editor können Sie Registerkarten hinzufügen oder löschen.

![](assets/add_delete_tabs_metadataschemaform.png)

* To add a new tab on a schema form, click **+**. Standardmäßig hat die neue Registerkarte den Namen "Unbenannt -1" . Sie können den Namen auf der Registerkarte **Einstellungen** ändern.

![](assets/add-tab-metadata-form.png)

* Klicken Sie **auf x**, um eine Registerkarte zu löschen. Klicken Sie auf **Speichern**, um die Änderungen zu speichern.

## Anwenden eines Metadatenschemas auf Ordner {#apply-a-metadata-schema-to-a-folder}

[!DNL Brand Portal] ermöglicht die Anpassung und Kontrolle des Metadatenschemas, sodass die Seite **Eigenschaften** eines Assets nur die gewünschten Informationen anzeigt. Um die auf der Seite **Eigenschaften** angezeigten Metadaten zu kontrollieren, entfernen Sie die erforderlichen Metadaten aus dem Metadatenschema-Formular und wenden Sie sie auf den entsprechenden Ordner an.

Gehen Sie wie folgt vor, um ein Metadatenschema-Formular auf einen Ordner anzuwenden:

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **Metadatenschemata**.

3. From the **Metadata Schema Forms** page, select the schema form that you want to apply to an asset, for example, **clothing**.

   ![](assets/apply-metadata-schema-form-to-folder.png)

4. From the toolbar at the top, click **Apply to Folder(s)**.

5. Wählen Sie auf der Seite **Ordner auswählen** den Ordner aus, auf den das Metadatenschema **Kleidung** angewendet werden soll, zum Beispiel **Handschuhe**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

6. Klicken Sie auf **Anwenden**, um das Metadatenschema-Formular auf den Ordner anzuwenden.

   Die im Metadatenschema-Formular **Kleidung** verfügbaren Metadaten werden auf den Ordner **Handschuhe** angewendet und auf der Seite **Eigenschaften** des Ordners angezeigt.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Wenn Sie ein Schema mit verschachtelten Schemata auf einen Ordner mit Videodateien anwenden, werden die Metadaten-Eigenschaften für die Videodateien möglicherweise nicht richtig gerendert. Um sicherzustellen, dass die Metadaten-Eigenschaften richtig gerendert werden, entfernen Sie die verschachtelten Schemata und wenden Sie nur das übergeordnete Schema auf den Ordner an.

## Löschen von Metadaten-Schemaformularen {#delete-a-metadata-schema-form}

[!DNL Brand Portal]In können Sie nur benutzerdefinierte Schemaformulare löschen. Die Standardschemaformulare/-vorlagen können nicht gelöscht werden. Sie können aber alle benutzerdefinierten Änderungen in diesen Formularen löschen.

Um ein Formular zu löschen, wählen Sie das Formular aus und klicken Sie auf das Symbol **Löschen**.

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Wenn Sie benutzerspezifische Änderungen an einem Standardformular löschen, wird das **Sperrsymbol** wieder vor dem Formularnamen in der Metadatenschema-Benutzeroberfläche angezeigt, um zu kennzeichnen, dass das Formular wieder in den Standardzustand versetzt wurde.

## Schemaformulare für MIME-Typen {#schema-forms-for-mime-types}

### Hinzufügen neuer Formulare für MIME-Typen {#adding-new-forms-for-mime-types}

Zusätzlich zu den Standardformularen können Sie auch benutzerdefinierte Formulare für Assets mit verschiedenen MIME-Typen hinzufügen oder ein neues Formular unter dem entsprechenden Formulartyp erstellen. For example, to add a new template for the **image/png** subtype, create the form under the "image" forms. Der Titel für das Schemaformular ist der Name des Untertyps. In diesem Fall lautet der Titel "png" .

#### Verwenden einer vorhandenen Schemavorlage für verschiedene MIME-Typen {#using-an-existing-schema-template-for-various-mime-types}

You can use an existing template for a different MIME type. For example, use the **image/jpeg** form for assets of MIME type **image/png**.

In this case, create a new node at `/etc/dam/metadataeditor/mimetypemappings` in the CRX repository. Geben Sie einen Namen für den Knoten an und definieren Sie die folgenden Eigenschaften:

| **Name** | **Typ** | **Wert** |
|---|---|---|
| exposedmimetype | Zeichenfolge | image/jpeg |
| mimetypes | String[] | image/png |

* **exposedmimetype**: Name des vorhandenen Formulars, das zugeordnet werden soll
* **mimetypes**: Liste der MIME-Typen, die das im **exposedmimetype** -Attribut definierte Formular verwenden

[!DNL Brand Portal] ordnet die folgenden MIME-Typen und Schemaformulare zu:

| **Schemaformular** | **MIME-Typen** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

Im Folgenden finden Sie eine Liste der standardmäßigen Metadaten-Eigenschaften:

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr:content/metadata/videoCodec
* jcr:content/metadata/audioCodec
* jcr:content/metadata/dc:title
* jcr:content/metadata/dc:description
* jcr:content/metadata/xmpMM:InstanceID
* jcr:content/metadata/xmpMM:DocumentID
* jcr:content/metadata/dam:sha1
* jcr:content/metadata/dam:solutionContext
* jcr:content/metadata/videoBitrate
* jcr:content/metadata/audioBitrate
* jcr:content/usages/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr:content/onTime
* jcr:content/offTime
* jcr:content/metadata/dam:size
* jcr:content/metadata/tiff:ImageWidth
* jcr:content/metadata/tiff:ImageLength
