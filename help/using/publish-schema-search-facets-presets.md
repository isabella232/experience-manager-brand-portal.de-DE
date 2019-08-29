---
title: Veröffentlichen von Vorgaben, Schema und Facetten in Brand Portal
seo-title: Veröffentlichen von Vorgaben, Schema und Facetten in Brand Portal
description: Erfahren Sie, wie Sie Vorgaben, Schema und Facetten in Brand Portal veröffentlichen.
seo-description: Erfahren Sie, wie Sie Vorgaben, Schema und Facetten in Brand Portal veröffentlichen.
uuid: c 836 d 9 bb -074 a -4113-9 c 91-b 2 bf 7658 b 88 d
topic-tags: veröffentlichen
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: Referenz
discoiquuid: bc 305 abc -9373-4 d 33-9179-0 a 5 f 3904 b 352
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Veröffentlichen von Vorgaben, Schema und Facetten in Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

The article delves into publishing image presets, metadata schemas, and custom search facets from [!DNL AEM] Author instance to [!DNL Brand Portal]. Publishing capability enables organizations to reuse the image presets, metadata schemas, and search facets created/modified at [!DNL AEM] Author instance thereby reducing duplicate efforts.

>[!NOTE]
>
>The capability to publish image presets, metadata schema, and search facets from [!DNL AEM] Author instance to [!DNL Brand Portal] is available [!DNL AEM 6.2 SP1-CFP7] and [!DNL AEM 6.3 SP 1-CFP 1 (6.3.1.1)] onwards.

## Veröffentlichen von Bildvorgaben in Brand Portal {#publish-image-presets-to-brand-portal}

Bildvorgaben sind eine Gruppe von Größenangaben und Formatierungsbefehlen, die zum Zeitpunkt der Bildbereitstellung angewendet werden. Image presets can be created and modified at [!DNL Brand Portal]. Alternatively, if [!DNL AEM] Author instance is running in dynamic media mode then users can create presets at the [!DNL AEM] Author and publish them to [!DNL AEM Assets Brand Portal], and avoid re-creating the same presets at [!DNL Brand Portal].\
Nachdem die Vorgabe erstellt wurde, wird sie als dynamisches Ausgabeformat in der Wiedergabeschiene der Asset-Detailseite und im Download-Dialogfeld angezeigt.

>[!NOTE]
>
>Wenn [!DNL AEM] die Autoreninstanz nicht im Modus [!DNL Dynamic Media] ausgeführt wird (Kunde hat nicht gekauft [!DNL Dynamic Media]), wird die [!UICONTROL Pyramid TIFF] -Darstellung der Assets nicht zum Zeitpunkt des Uploads erstellt. Bildvorgaben oder dynamische Darstellungen funktionieren auf [!UICONTROL Pyramid TIFF] eines Assets. Wenn [!UICONTROL Pyramid TIFF] nicht auf [!DNL AEM] der Authoring-Instanz verfügbar ist, ist sie auch nicht verfügbar [!DNL Brand Portal] . Demzufolge sind keine dynamischen Darstellungen in der Darstellungsleiste der Seite mit den Asset-Details vorhanden und das Dialogfeld wird heruntergeladen.

To publish image presets to [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the [!DNL AEM] logo to access the global navigation console and tap/ click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Image Presets]**.
2. Select the image preset or multiple image presets from the list of image presets and click/ tap **[!UICONTROL Publish to Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>When users click **[!UICONTROL Publish to Brand Portal]** the image presets are queued for publishing. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

Rückgängigmachen der Veröffentlichung einer Bildvorgabe aus [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the [!DNL AEM] logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Image Presets]**.
2. Wählen Sie eine Bildvorgabe aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]aus.**

## Veröffentlichen des Metadatenschemas in Brand Portal  {#publish-metadata-schema-to-brand-portal}

Im Metadatenschema sind das Layout und die Eigenschaften beschrieben, die auf der Eigenschaftenseite von Assets/Sammlungen angezeigt werden.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

If users have edited the default schema on [!DNL AEM] Author instance and are willing to use the same schema as default schema on the [!DNL Brand Portal], they can simply publish the metadata schema forms to [!DNL Brand Portal]. In such a scenario, the default schema at [!DNL Brand Portal] is over-ridden by the default schemas published from [!DNL AEM] Author instance.

If users have created a custom schema on [!DNL AEM] Author instance, they can publish the custom schema to [!DNL Brand Portal] instead of re-creating the same custom schema there. Users can then apply this custom schema to any folder/ collection in [!DNL Brand Portal].

>[!NOTE]
>
>Default schemas cannot be published to the [!DNL Brand Portal] if they are locked at the [!DNL AEM] instance (that is they are unedited).

![](assets/default-schema-form.png)

>[!NOTE]
>
>If a folder has a schema applied on [!DNL AEM] Author instance, the same schema must also exist on the [!DNL Brand Portal] to maintain the consistency in the asset properties page on [!DNL AEM] Author and [!DNL Brand portal].

To publish a metadata schema from [!DNL AEM] Author instance to [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Metadata Schemas]**.
2. Wählen Sie ein Metadatenschema aus und wählen Sie oben die Option **[!UICONTROL In Brand Portal veröffentlichen]aus.**

>[!NOTE]
>
>When users click **[!UICONTROL Publish to Brand Portal]**, the metadata schemas are queued for publishing. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

To unpublish a metadata schema from [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the [!DNL AEM] logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Metadata Schemas]**.
2. Wählen Sie ein Metadatenschema aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]aus.**

## Veröffentlichen von Suchfacetten in Brand Portal {#publish-search-facets-to-brand-portal}

Search forms provide the capability of [faceted search](../using/brand-portal-search-facets.md) to users on [!DNL Brand Portal]. Search facets impart greater granularity to searches on [!DNL Brand Portal]. Alle dem Suchformular [hinzugefügten Eigenschaften](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) sind für Benutzer als Suchfacetten in Suchfiltern verfügbar.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

If you are willing to use custom search form **[!UICONTROL Assets Admin Search Rail]** from [!DNL AEM] Author instance, then instead of re-creating the same form on [!DNL Brand Portal] you can publish the customized search form from [!DNL AEM] Author instance to [!DNL Brand Portal].

>[!NOTE]
>
>Locked search form **[!UICONTROL Assets Admin Search Rail]** on AEM Assets cannot be published to [!DNL Brand Portal] unless it is edited. Once edited and published to [!DNL Brand Portal], this search form overrides the search form on [!DNL Brand Portal].

To publish the edited search facet from [!DNL AEM] Author instance to [!DNL Brand Portal]:

1. Tap/click the [!DNL AEM] logo, and then go to **[!UICONTROL Tools]** &gt; **[!UICONTROL General]** &gt; **[!UICONTROL Search Forms]**.
2. Wählen Sie das bearbeitete Suchformular aus und wählen Sie **[!UICONTROL In Brand Portal veröffentlichen aus]**.

   >[!NOTE]
   >
   >When users click **[!UICONTROL Publish to Brand Portal]**, the search facets are queued for publishing. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

To unpublish search forms from [!DNL Brand Portal]:

1. In [!DNL AEM] Author instance, tap/ click the [!DNL AEM] logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL General]** &gt; **[!UICONTROL Search Forms]**.
2. Wählen Sie das Suchformular aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]aus.**

>[!NOTE]
>
>Beim **[!UICONTROL Rückgängigmachen der Veröffentlichung aus]** der Markenportalaktion wird das Standardsuchformular im Brand Portal und das letzte vor der Veröffentlichung verwendete Suchformular nicht wiederhergestellt.

### Beschränkungen {#limitations}

1. Few search predicates are not applicable to search filters on the [!DNL Brand Portal]. When these search predicates are published as part of the search form from [!DNL AEM] Author instance to [!DNL Brand Portal], they are filtered out. Users, therefore, see less number of predicates in the published form at the [!DNL Brand Portal]. Sehen Sie sich die [Liste aller verwendbaren Sucheigenschaften in Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates) an.

2. For [!UICONTROL Options] predicate, if a user is using any custom path to read options at AEM Author instance, it won't work at the Brand Portal. Diese zusätzlichen Pfade und Optionen werden nicht mit dem Suchformular in Brand Portal veröffentlicht. In this case, users can select the **[!UICONTROL Manual]** option in **[!UICONTROL Add Options]** within **[!UICONTROL Options Predicate]** to add these options manually at [!DNL Brand Portal].

![](assets/options-predicate-manual.png)
