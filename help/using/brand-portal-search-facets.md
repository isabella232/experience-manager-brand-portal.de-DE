---
title: Verwenden benutzerdefinierter Suchfacetten
seo-title: Verwenden benutzerdefinierter Suchfacetten
description: Administratoren können Sucheigenschaften zum Bereich „Filter“ hinzufügen, um die Suche anzupassen und die Suchfunktion auf diese Weise vielseitiger zu gestalten.
seo-description: Administratoren können Sucheigenschaften zum Bereich „Filter“ hinzufügen, um die Suche anzupassen und die Suchfunktion auf diese Weise vielseitiger zu gestalten.
uuid: 986 fba 5 a-fac 5-4128-ac 75-d 04 da 5 b 52 d 45
content-type: Referenz
topic-tags: Administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 19 faa 28-246 b -42 c 7-869 f -97 c 95 c 7 a 1349
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Verwenden benutzerdefinierter Suchfacetten {#use-custom-search-facets}

Administrators can add search predicates to the [!UICONTROL Filters] panel to customize search and make the search functionality versatile.

Brand Portal supports [faceted search](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) for granular searches of approved brand assets, which is possible due to [**Filters** panel](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Search facets are made available on Filters panel through **[!UICONTROL Search Form]** in the admin tools. Auf der Seite „Suchformular“ in den Admin Tools gibt es ein Standardformular namens „Asset-Admin-Suchschienenseite“. Administratoren können jedoch den Standardbereich „Filter“ durch Bearbeiten des Standardsuchformulars „Asset-Admin-Suchschienenseite“ anpassen, um die Suchfunktion durch Hinzufügen, Ändern oder Entfernen von Sucheigenschaften vielseitiger zu machen.

You can use various search predicates to customize the **[!UICONTROL Filters]** panel. Fügen Sie beispielsweise die Eigenschaft Eigenschaft hinzu, um nach Assets zu suchen, die einer einzelnen Eigenschaft entsprechen, die Sie in dieser Eigenschaft angeben. Fügen Sie die Optionen hinzu, um nach Assets zu suchen, die einem oder mehreren Werten entsprechen, die Sie für eine bestimmte Eigenschaft angeben. Fügen Sie die Datumsbereichseigenschaft hinzu, um nach Assets zu suchen, die innerhalb eines bestimmten Datumsbereichs erstellt wurden.

>[!NOTE]
>
>AEM allows organizations to [publish the customized search forms from AEM Author](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) to Brand Portal, instead of re-creating the same form on Brand Portal.

## Hinzufügen von Sucheigenschaften {#add-a-search-predicate}

Gehen Sie wie folgt vor, um Sucheigenschaften dem Bereich **[!UICONTROL Filter]hinzuzufügen:**

1. Um auf Verwaltungstools zuzugreifen, klicken Sie auf das AEM-Logo in der Symbolleiste oben.

   ![](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **[!UICONTROL Suchformulare]**.

   ![](assets/navigation-panel-1.png)

3. In the **[!UICONTROL Search Forms]** page, select **[!UICONTROL Assets Admin Search Rail]**.

   ![](assets/search-forms-page.png)

4. Klicken Sie in der Symbolleiste oben auf **[!UICONTROL Bearbeiten], um die Seite „Suchformular bearbeiten“ zu öffnen.**

   ![](assets/edit-search-form-1.png)

5. In the [!UICONTROL Edit Search Form] page, drag a predicate from the [!UICONTROL Select Predicate] tab to the main pane. For example, drag **[!UICONTROL Property Predicate]**.

   Das Feld **[!UICONTROL Eigenschaft]** wird im Hauptbereich angezeigt und die Registerkarte **Einstellungen[!UICONTROL auf der rechten Seite zeigt die Eigenschaftsprädikate an.]**

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >Mit der Kopfzeilenbeschriftung auf der Registerkarte **[!UICONTROL Einstellungen]wird der Typ der gewählten Eigenschaft identifiziert.**

6. Geben Sie auf der Registerkarte **[!UICONTROL Einstellungen]eine Beschriftung, Platzhaltertext und eine Beschreibung für das Eigenschaftsprädikat ein.**

   * Select **[!UICONTROL Partial Search]**, if you want to allow partial phrase search (and wildcard search) of assets-based on the specified property value. Das Prädikat unterstützt standardmäßig die Volltextsuche.
   * Select **[!UICONTROL Ignore Case]**, if you want the asset search based on property value to be non-case sensitive. Standardmäßig wird bei der Suche nach Eigenschaftswerten im Suchfilter zwischen Groß- und Kleinschreibung unterschieden.
   >[!NOTE]
   >
   >Nach Aktivierung des Kontrollkästchens **[!UICONTROL Teilsuche]** wird [!UICONTROL Groß-/Kleinschreibung ignorieren] standardmäßig aktiviert.

7. In the [!UICONTROL Property Name] field, open property picker and select the property based on which the search is performed. Alternativ können Sie einen Namen für die Eigenschaft eingeben. Geben Sie z [!UICONTROL `  jcr :content/metadata/dc:title`] . [!UICONTROL `./jcr:content/metadata/dc:title`]B. ein oder.

   ![](assets/title-prop.png)

8. Klicken Sie auf **[!UICONTROL Fertig], um die Einstellungen zu speichern.**
9. From the [!UICONTROL Assets] user interface, click the overlay icon and choose **[!UICONTROL Filter]** to navigate to the **[!UICONTROL Filters]** panel. The **[!UICONTROL Property]** predicate is added to the panel.

   ![](assets/property-filter-panel.png)

10. Geben Sie in das Textfeld **[!UICONTROL Eigenschaft]einen Titel für das Asset ein, das gesucht werden soll.** Zum Beispiel "Adobe" . Wenn Sie eine Suche durchführen, werden Assets, deren Titel „Adobe“ entspricht, in den Suchergebnissen angezeigt.

## Liste der Sucheigenschaften {#list-of-search-predicates}

Similar to the way you add a **[!UICONTROL Property]** predicate, you can add the following predicates to the **[!UICONTROL Filters]** panel:

| **Eigenschaftsname** | **Beschreibung** | **Eigenschaften** |
|-------|-------|----------|
| [!UICONTROL Pfadbrowser] | Sucheigenschaft, um Assets in einem bestimmten Speicherort zu suchen. **Hinweis:***Für einen angemeldeten Benutzer zeigt der Pfad-Browser auf Filter nur die Inhaltsstruktur der Ordner (und deren Vorgänger) an, die für den Benutzer freigegeben wurden.* <br> Administratoren können nach Assets in einem beliebigen Ordner suchen, indem sie mit dem Pfadbrowser zu diesem Ordner navigieren. <br> Benutzer ohne Administratorrechte können die Assets in einem Ordner (Zugriff darauf) durchsuchen, indem sie in den Pfad-Browser navigieren. | <ul><li>Feldbezeichnung</li><li>Pfad</li><li>Beschreibung</li></ul> |
| [!UICONTROL Eigenschaft] | Sucht nach Assets basierend auf einer bestimmten Metadaten-Eigenschaft. **Hinweis:***Beim Auswählen der partiellen Suche ist standardmäßig "Groß-/Kleinschreibung ignorieren" ausgewählt*. | <ul><li>Feldbezeichnung</li><li>Platzhalter</li><li>Eigenschaftsname</li><li>Teilsuche</li><li>Groß-/Kleinschreibung ignorieren</li><li> Beschreibung</li></ul> |
| [!UICONTROL Mehrwert-Eigenschaft] | Similar to property predicate but allows multiple input values, separated by a delimiter (default is COMMA[,]) assets matching any of the input values are returned in results. | <ul><li>Feldbezeichnung</li><li>Platzhalter</li><li>Eigenschaftsname</li><li>Trennzeichen-Unterstützung</li><li>Groß-/Kleinschreibung ignorieren</li><li>Beschreibung</li></ul> |
| [!UICONTROL Tags] | Sucheigenschaft, um Assets basierend auf Tags zu suchen. Sie können die Pfadeigenschaft konfigurieren, um verschiedene Tags in der Tag-Liste zu füllen. * Hinweis: Administratoren müssen ggf. den Pfadwert ändern, [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]wenn sie das Suchformular über AEM veröffentlichen, wo der Pfad beispielsweise keine Mandanten-Informationen enthält [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Pfad</li><li>Beschreibung</li></ul> |
| [!UICONTROL Pfad] | Sucheigenschaft, um Assets in einem bestimmten Speicherort zu suchen. | <ul><li>Feldbezeichnung</li><li>Pfad</li><li>Beschreibung</li></ul> |  |
| [!UICONTROL Relatives Datum] | Sucheigenschaft, um Assets basierend auf dem relativen Datum ihrer Erstellung zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Relatives Datum</li></ul> |
| [!UICONTROL Bereich] | Sucheigenschaft, um Assets innerhalb eines bestimmten Eigenschaftswert-Bereichs zu suchen. Im Filterbedienfeld können Sie die minimalen und maximalen Eigenschaftswerte für den Bereich festlegen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| [!UICONTROL Datumsbereich] | Sucheigenschaft, um Assets zu suchen, die innerhalb eines bestimmten Bereichs für eine Datumseigenschaft erstellt wurden. Im Bereich „Filter“ können Sie das Start- und das Enddatum angeben. | <ul><li>Feldbezeichnung</li><li>Platzhalter</li><li>Eigenschaftsname</li><li>Textbereich (von)</li><li>Textbereich (bis)</li><li>Beschreibung</li></ul> |
| [!UICONTROL Datum] | Sucheigenschaft für eine Schieberegler-basierte Suche nach Assets basierend auf einer Datumseigenschaft | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| [!UICONTROL Dateigröße] | Sucheigenschaft, um Assets basierend auf ihrer Größe zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Pfad</li><li>Beschreibung</li></ul> |
| [!UICONTROL Asset zuletzt geändert] | Sucheigenschaft, um Assets basierend auf dem Datum der letzten Änderung zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| [!UICONTROL Genehmigungsstatus] | Sucheigenschaft, um Assets basierend auf der Genehmigungsstatus-Eigenschaft zu suchen. Der Eigenschaftsname lautet standardmäßig **dam:status**. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| [!UICONTROL Checkout-Status] | Sucheigenschaft, um Assets basierend auf dem Checkout-Status eines Assets zum Zeitpunkt der Veröffentlichung aus AEM Assets zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| [!UICONTROL Ausgecheckt von] | Sucheigenschaft, um Assets basierend auf dem Benutzer zu suchen, der das Asset ausgecheckt hat. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| [!UICONTROL Gültigkeitsstatus] | Suchen Sie Predicate, um Assets basierend auf dem Ablaufstatus zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| [!UICONTROL Mitglied der Sammlung] | Sucheigenschaft, um Assets basierend darauf zu suchen, ob ein Asset zu einer Sammlung gehört. | Beschreibung |
| [!UICONTROL Ausgeblendet] | This predicate is not explicitly visible to the end users and is used for any hidden constraints typically for restricting search results type to **dam:Asset**. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |

>[!NOTE]
>
>Do not use **[!UICONTROL Options Predicate]**, **[!UICONTROL Publish Status Predicate]**, and **[!UICONTROL Rating Predicate]** as these predicates are not functional in Brand Portal.

## Löschen von Sucheigenschaften {#delete-a-search-predicate}

Führen Sie die folgenden Schritte aus, um eine Sucheigenschaft zu löschen:

1. Klicken Sie auf das Adobe-Logo, um auf die Admin Tools zuzugreifen.

   ![](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **[!UICONTROL Suchformulare]**.

   ![](assets/navigation-panel-2.png)

3. In the **[!UICONTROL Search Forms]** page, select **[!UICONTROL Assets Admin Search Rail]**.

   ![](assets/search-forms-page.png)

4. Klicken Sie in der Symbolleiste oben auf **[!UICONTROL Bearbeiten], um die Seite „Suchformular bearbeiten“ zu öffnen.**

   ![](assets/edit-search-form-2.png)

5. In the [!UICONTROL Edit Search Form] page, from the main pane, select the predicate you want to delete. For example, select **[!UICONTROL Property Predicate]**.

   Die Registerkarte **[!UICONTROL Einstellungen]auf der rechten Seite zeigt die Eigenschaftsprädikat-Felder an.**

6. Klicken Sie zum Löschen des Eigenschaftsprädikats auf das Papierkorbsymbol. Klicken Sie im Dialogfeld **[!UICONTROL Feld löschen]** auf **Löschen], um die Löschaktion zu bestätigen.[!UICONTROL **

   Das Feld **[!UICONTROL Eigenschaftsprädikat]** wird vom Hauptbereich entfernt und die Registerkarte **Eigenschaften]wird leer angezeigt.[!UICONTROL **

   ![](assets/search-form-delete-predicate.png)

7. To save the changes, click **[!UICONTROL Done]** in the toolbar.
8. From the **[!UICONTROL Assets]** user interface, click the overlay icon and choose **[!UICONTROL Filter]** to navigate to the **[!UICONTROL Filters]** panel. The **[!UICONTROL Property]** predicate is removed from the panel.

   ![](assets/property-predicate-removed.png)
