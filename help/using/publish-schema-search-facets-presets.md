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
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Veröffentlichen von Vorgaben, Schema und Facetten in Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

In diesem Artikel wird beschrieben, wie Vorgaben, Metadatenschemata und benutzerdefinierte Suchfacetten aus der AEM-Autoreninstanz in Brand Portal veröffentlicht werden. Mit der Veröffentlichungsfunktion können Unternehmen die Bildvorgaben, Metadaten-Schemata und Suchfacetten wiederverwenden, die auf der AEM-Autoreninstanz erstellt/geändert wurden, sodass doppelte Bemühungen vermieden werden.

>[!NOTE]
>
>Die Funktion zum Veröffentlichen von Bildvorgaben, Metadatenschemata und Suchfacetten aus der AEM-Autoreninstanz in Brand Portal ist ab AEM 6.2 SP1-CFP7 und AEM 6.3 SP 1-CFP 1 (6.3.1.1) verfügbar.

## Veröffentlichen von Bildvorgaben in Brand Portal {#publish-image-presets-to-brand-portal}

Bildvorgaben sind eine Gruppe von Größenangaben und Formatierungsbefehlen, die zum Zeitpunkt der Bildbereitstellung angewendet werden. Bildvorgaben können in Brand Portal erstellt und geändert werden. Wenn die AEM Authoring-Instanz im dynamischen Medienmodus ausgeführt wird, können Benutzer auch Vorgaben für AEM Author erstellen und auf AEM Assets Brand Portal veröffentlichen und vermeiden, dieselben Vorgaben erneut in Brand Portal zu erstellen.\
Nachdem die Vorgabe erstellt wurde, wird sie als dynamisches Ausgabeformat in der Wiedergabeschiene der Asset-Detailseite und im Download-Dialogfeld angezeigt.

>[!NOTE]
>
>Wenn die AEM-Autoreninstanz nicht im [!UICONTROL dynamischen Medienmodus] ausgeführt wird (Kunden hat dynamische Medien nicht gekauft), wird die [!UICONTROL Pyramid TIFF] -Darstellung der Assets nicht zum Zeitpunkt des Uploads erstellt. Image presets or dynamic renditions work on [!UICONTROL Pyramid TIFF] of an asset, so if [!UICONTROL Pyramid TIFF] is not available on AEM Author instance then it is not available on Brand Portal as well. Demzufolge sind keine dynamischen Darstellungen in der Darstellungsleiste der Seite mit den Asset-Details vorhanden und das Dialogfeld wird heruntergeladen.

So veröffentlichen Sie Bildvorgaben in Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/ click the Tools icon and navigate to **[!UICONTROL Assets]** &gt; **[!UICONTROL Image Presets]**.
2. Select the image preset or multiple image presets from the list of image presets and click/ tap **[!UICONTROL Publish to Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>When users click **[!UICONTROL Publish to Brand Portal]** the image presets are queued for publishing. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

Rückgängigmachen der Veröffentlichung einer Bildvorgabe aus dem Markenportal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the **[!UICONTROL Tools]** icon and navigate to **[!UICONTROL Assets &gt; Image Presets]**.
2. Wählen Sie eine Bildvorgabe aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]aus.**

## Veröffentlichen des Metadatenschemas in Brand Portal  {#publish-metadata-schema-to-brand-portal}

Im Metadatenschema sind das Layout und die Eigenschaften beschrieben, die auf der Eigenschaftenseite von Assets/Sammlungen angezeigt werden.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Wenn Benutzer das Standardschema in der AEM-Autoreninstanz bearbeitet haben und bereit sind, dasselbe Schema als Standardschema im Brand Portal zu verwenden, können sie einfach die Metadatenschemaformulare im Brand Portal veröffentlichen. In einem solchen Szenario wird das Standardschema unter Markenportal durch die Standardschemas ersetzt, die aus der AEM-Autoreninstanz veröffentlicht wurden.

Wenn Benutzer ein benutzerdefiniertes Schema für die AEM-Autoreninstanz erstellt haben, können sie das benutzerdefinierte Schema in Brand Portal veröffentlichen, anstatt dasselbe benutzerspezifische Schema erneut zu erstellen. Benutzer können dieses benutzerdefinierte Schema auf jeden Ordner und jede Sammlung in Brand Portal anwenden.

>[!NOTE]
>
>Standardschemas können nicht im Markenportal veröffentlicht werden, wenn sie auf der AEM-Instanz gesperrt sind (d. h. sie werden nicht bearbeitet).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Wenn in einem Ordner ein Schema auf die AEM-Autoreninstanz angewendet wird, muss dasselbe Schema auch im Markenportal vorhanden sein, damit die Konsistenz auf der Asset-Eigenschaftenseite in AEM Author und Brand Portal gewahrt bleibt.

So veröffentlichen Sie ein Metadatenschema aus der AEM-Autoreninstanz in Brand Portal:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets &gt; Metadata Schemas]**.
2. Wählen Sie ein Metadatenschema aus und wählen Sie oben die Option **[!UICONTROL In Brand Portal veröffentlichen]aus.**

>[!NOTE]
>
>When users click **[!UICONTROL Publish to Brand Portal]**, the metadata schemas are queued for publishing. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

So machen Sie die Veröffentlichung eines Metadatenschemas in Brand Portal rückgängig:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL Assets &gt; Metadata Schemas]**.
2. Wählen Sie ein Metadatenschema aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]aus.**

## Veröffentlichen von Suchfacetten in Brand Portal {#publish-search-facets-to-brand-portal}

Suchformulare stellen Benutzern in Brand Portal die Funktion [Facettensuche](../using/brand-portal-search-facets.md) bereit. Suchfacetten geben eine größere Granularität für die Suche nach Markenportal ein. Alle dem Suchformular [hinzugefügten Eigenschaften](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) sind für Benutzer als Suchfacetten in Suchfiltern verfügbar.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

If you are willing to use custom search form **[!UICONTROL Assets Admin Search Rail]** from AEM Author instance, then instead of re-creating the same form on Brand Portal you can publish the customized search form from AEM Author instance to Brand Portal.

>[!NOTE]
>
>Locked search form **[!UICONTROL Assets Admin Search Rail]** on AEM Assets cannot be published to Brand Portal unless it is edited. Nach dem Bearbeiten und Veröffentlichen im Markenportal überschreibt dieses Suchformular das Suchformular im Markenportal.

So veröffentlichen Sie die bearbeitete Suchfacette aus der AEM-Autoreninstanz in Brand Portal:

1. Tap/click the AEM logo, and then go to **[!UICONTROL Tools]** &gt; **[!UICONTROL General]** &gt; **[!UICONTROL Search Forms]**.
2. Wählen Sie das bearbeitete Suchformular aus und wählen Sie **[!UICONTROL In Brand Portal veröffentlichen aus]**.

   >[!NOTE]
   >
   >When users click **[!UICONTROL Publish to Brand Portal]**, the search facets are queued for publishing. Benutzern wird empfohlen, anhand des Protokolls der Replikationsagenten zu überprüfen, ob die Veröffentlichung erfolgreich war.

So machen Sie die Veröffentlichung von Suchformularen in Brand Portal rückgängig:

1. In AEM Author instance, tap/ click the AEM logo to access the global navigation console and tap/click the Tools icon and navigate to **[!UICONTROL General &gt; Search Forms]**.
2. Wählen Sie das Suchformular aus und wählen Sie oben die Option **[!UICONTROL Aus Brand Portal löschen]aus.**

>[!NOTE]
>
>Beim **[!UICONTROL Rückgängigmachen der Veröffentlichung aus]** der Markenportalaktion wird das Standardsuchformular im Brand Portal und das letzte vor der Veröffentlichung verwendete Suchformular nicht wiederhergestellt.

### Beschränkungen {#limitations}

1. Einige Suchvorhersagen sind nicht auf Suchfilter im Markenportal anwendbar. Wenn diese Sucheigenschaften als Teil des Suchformulars aus der AEM-Autoreninstanz in Brand Portal veröffentlicht werden, werden sie herausgefiltert. Benutzer sehen daher weniger Vorhersagen im veröffentlichten Formular im Markenportal. Sehen Sie sich die [Liste aller verwendbaren Sucheigenschaften in Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates) an.

2. For [!UICONTROL Options Predicate], if a user is using any custom path to read options at AEM Author instance, it won't work at the Brand Portal. Diese zusätzlichen Pfade und Optionen werden nicht mit dem Suchformular in Brand Portal veröffentlicht. In this case, users can select the **[!UICONTROL Manual]** option in **[!UICONTROL Add Options]** within **[!UICONTROL Options Predicate]** to add these options manually at Brand Portal.

![](assets/options-predicate-manual.png)
