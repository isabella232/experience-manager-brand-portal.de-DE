---
title: Veröffentlichen von Vorgaben, Schemata und Facetten in Brand Portal
seo-title: Veröffentlichen von Vorgaben, Schemata und Facetten in Brand Portal
description: Erfahren Sie, wie Sie Vorgaben, Schemata und Facetten in Brand Portal veröffentlichen.
seo-description: Erfahren Sie, wie Sie Vorgaben, Schemata und Facetten in Brand Portal veröffentlichen.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: veröffentlichen
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: Referenz
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Veröffentlichen von Vorgaben, Schemata und Facetten in Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

In diesem Artikel wird beschrieben, wie Vorgaben, Metadatenschemata und benutzerdefinierte Suchfacetten aus der AEM-Autoreninstanz in Brand Portal veröffentlicht werden. Mit der Veröffentlichungsfunktion können Unternehmen die Bildvorgaben, Metadaten-Schemata und Suchfacetten wiederverwenden, die in der AEM Author-Instanz erstellt/geändert wurden, wodurch doppelte Bemühungen reduziert werden.

>[!NOTE]
>
>Die Funktion zum Veröffentlichen von Bildvorgaben, Metadatenschemata und Suchfacetten aus der AEM-Autoreninstanz in Brand Portal ist ab AEM 6.2 SP1-CFP7 und AEM 6.3 SP 1-CFP 1 (6.3.1.1) verfügbar.

## Veröffentlichen von Bildvorgaben in Brand Portal {#publish-image-presets-to-brand-portal}

Bildvorgaben sind eine Gruppe von Größenangaben und Formatierungsbefehlen, die zum Zeitpunkt der Bildbereitstellung angewendet werden. Bildvorgaben können in Brand Portal erstellt und geändert werden. Wenn die AEM Author-Instanz im dynamischen Medienmodus ausgeführt wird, können Benutzer auch Vorgaben im AEM Author erstellen und sie im AEM Assets Brand Portal veröffentlichen, um zu vermeiden, dass dieselben Vorgaben im Markenportal erneut erstellt werden.\
Nachdem die Vorgabe erstellt wurde, wird sie als dynamische Wiedergabe in der Wiedergabeschiene der Asset-Detailseite und im Dialogfeld „Download“ angezeigt.

>[!NOTE]
>
>If AEM Author instance is not running in [!UICONTROL Dynamic Media Mode] (customer has not purchased Dynamic Media), then the [!UICONTROL Pyramid TIFF]  rendition of the assets are not created at the time of upload. Image presets or dynamic renditions work on [!UICONTROL Pyramid TIFF] of an asset, so if [!UICONTROL Pyramid TIFF] is not available on AEM Author instance then it is not available on Brand Portal as well. Daher sind in der Wiedergabeschiene der Asset-Detailseite und im Dialogfeld „Download“ keine dynamischen Wiedergaben verfügbar.

So veröffentlichen Sie Bildvorgaben in Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/ click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Image Presets]**.
2. Wählen Sie in der Liste der Bildvorgaben eine oder mehrere Bildvorgaben aus und klicken/tippen Sie auf **[!UICONTROL In Brand Portal veröffentlichen]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Wenn Benutzer auf **[!UICONTROL In Brand Portal veröffentlichen]** klicken, werden die Bildvorgaben zur Veröffentlichung in die Warteschlange gestellt. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

Rückgängigmachen der Veröffentlichung einer Bildvorgabe aus dem Markenportal

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the **[!UICONTROL Tools]** icon and navigate to **[!UICONTROL Assets &gt; Image Presets]**.
2. Wählen Sie eine Bildvorgabe aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]aus.**

## Veröffentlichen des Metadatenschemas in Brand Portal  {#publish-metadata-schema-to-brand-portal}

Im Metadatenschema sind das Layout und die Eigenschaften beschrieben, die auf der Eigenschaftenseite von Assets/Sammlungen angezeigt werden.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

If users have edited the default schema on AEM Author instance and are willing to use the same schema as default schema on the Brand Portal, they can simply publish the metadata schema forms to Brand Portal. In einem solchen Szenario wird das Standardschema im Markenportal durch die Standardschemata überschrieben, die von der AEM Author-Instanz veröffentlicht wurden.

If users have created a custom schema on AEM Author instance, they can publish the custom schema to Brand Portal instead of re-creating the same custom schema there. Benutzer können dieses benutzerdefinierte Schema auf jeden Ordner und jede Sammlung in Brand Portal anwenden.

>[!NOTE]
>
>Standardschemata können nicht im Markenportal veröffentlicht werden, wenn sie in der AEM-Instanz gesperrt sind (d. h., sie werden nicht bearbeitet).

![](assets/default-schema-form.png)

>[!NOTE]
>
>If a folder has a schema applied on AEM Author instance, the same schema must also exist on the Brand Portal to maintain the consistency in the asset properties page on AEM Author and Brand Portal.

So veröffentlichen Sie ein Metadatenschema aus der AEM-Autoreninstanz in Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets &gt; Metadata Schemas]**.
2. Wählen Sie ein Metadatenschema aus und wählen Sie oben die Option **[!UICONTROL In Brand Portal veröffentlichen]aus.**

>[!NOTE]
>
>Wenn Benutzer auf **[!UICONTROL In Brand Portal veröffentlichen]** klicken, werden die Metadatenschemata zur Veröffentlichung in die Warteschlange gestellt. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

So machen Sie die Veröffentlichung eines Metadatenschemas in Brand Portal rückgängig:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets &gt; Metadata Schemas]**.
2. Wählen Sie ein Metadatenschema aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]aus.**

## Veröffentlichen von Suchfacetten in Brand Portal {#publish-search-facets-to-brand-portal}

Suchformulare stellen Benutzern in Brand Portal die Funktion [Facettensuche](../using/brand-portal-search-facets.md) bereit. Suchfacetten bieten eine größere Granularität für Suchvorgänge im Markenportal. Alle dem Suchformular [hinzugefügten Eigenschaften](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) sind für Benutzer als Suchfacetten in Suchfiltern verfügbar.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

If you are willing to use custom search form **[!UICONTROL Assets Admin Search Rail]** from AEM Author instance, then instead of re-creating the same form on Brand Portal you can publish the customized search form from AEM Author instance to Brand Portal.

>[!NOTE]
>
>Locked search form **[!UICONTROL Assets Admin Search Rail]** on AEM Assets cannot be published to Brand Portal unless it is edited. Nach der Bearbeitung und Veröffentlichung im Markenportal überschreibt dieses Suchformular das Suchformular im Markenportal.

So veröffentlichen Sie die bearbeitete Suchfacette aus der AEM-Autoreninstanz in Brand Portal:

1. Tap/click the AEM logo, and then go to **[!UICONTROL Tools]** &gt; **[!UICONTROL General]** &gt; **[!UICONTROL Search Forms]**.
2. Wählen Sie das bearbeitete Suchformular aus und wählen Sie **[!UICONTROL In Brand Portal veröffentlichen aus]**.

   >[!NOTE]
   >
   >Wenn Benutzer auf **[!UICONTROL In Brand Portal veröffentlichen]** klicken, werden Suchfacetten zur Veröffentlichung in die Warteschlange gestellt. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

So machen Sie die Veröffentlichung von Suchformularen in Brand Portal rückgängig:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL General &gt; Search Forms]**.
2. Wählen Sie das Suchformular aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]** aus.

>[!NOTE]
>
>Beim **[!UICONTROL Rückgängigmachen der Veröffentlichung in Brand Portal]** bleibt in Brand Portal das Standardsuchformular erhalten. Das letzte vor der Veröffentlichung verwendete Suchformular wird nicht wiederhergestellt.

### Beschränkungen {#limitations}

1. Few search predicates are not applicable to search filters on the Brand Portal. Wenn diese Sucheigenschaften als Teil des Suchformulars aus der AEM-Autoreninstanz in Brand Portal veröffentlicht werden, werden sie herausgefiltert. Die Benutzer sehen daher weniger Prognosen im veröffentlichten Formular im Markenportal. Weitere Informationen finden Sie in der [Liste aller verwendbaren Sucheigenschaften in Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

2. For [!UICONTROL Options Predicate], if a user is using any custom path to read options at AEM Author instance, it won't work at the Brand Portal. Diese zusätzlichen Pfade und Optionen werden nicht mit dem Suchformular in Brand Portal veröffentlicht. In this case, users can select the **[!UICONTROL Manual]** option in **[!UICONTROL Add Options]** within **[!UICONTROL Options Predicate]** to add these options manually at Brand Portal.

![](assets/options-predicate-manual.png)
