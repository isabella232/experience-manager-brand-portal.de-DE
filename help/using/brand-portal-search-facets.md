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
source-git-commit: ea7fdd2df0696ed309227fa77e3f79d0141bcb58

---


# Verwenden benutzerdefinierter Suchfacetten {#use-custom-search-facets}

Administratoren können Sucheigenschaften zum Bereich „Filter“ hinzufügen, um die Suche anzupassen und die Suchfunktion auf diese Weise vielseitiger zu gestalten.

[!DNL Brand Portal] unterstützt [die facettierte Suche](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) nach granularen Suchen der genehmigten Marken-Assets, was aufgrund des [**Filters "Filter** " möglich](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)ist. Search facets are made available on Filters panel through **Search Form** in the admin tools. Auf der Seite „Suchformular“ in den Admin Tools gibt es ein Standardformular namens „Asset-Admin-Suchschienenseite“. Administratoren können jedoch den Standardbereich „Filter“ durch Bearbeiten des Standardsuchformulars „Asset-Admin-Suchschienenseite“ anpassen, um die Suchfunktion durch Hinzufügen, Ändern oder Entfernen von Sucheigenschaften vielseitiger zu machen.

You can use various search predicates to customize the **Filters** panel. Fügen Sie beispielsweise die Eigenschaft Eigenschaft hinzu, um nach Assets zu suchen, die einer einzelnen Eigenschaft entsprechen, die Sie in dieser Eigenschaft angeben. Fügen Sie die Optionen hinzu, um nach Assets zu suchen, die einem oder mehreren Werten entsprechen, die Sie für eine bestimmte Eigenschaft angeben. Fügen Sie die Datumsbereichseigenschaft hinzu, um nach Assets zu suchen, die innerhalb eines bestimmten Datumsbereichs erstellt wurden.

>[!NOTE]
>
>[!DNL AEM] Ermöglicht es Unternehmen, [die angepassten Suchformulare von [! DNL AEM], anstatt](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) [!DNL Brand Portal]dasselbe Formular erneut zu erstellen [!DNL Brand Portal].

## Hinzufügen von Sucheigenschaften {#add-a-search-predicate}

Gehen Sie wie folgt vor, um Sucheigenschaften dem Bereich **Filter** hinzuzufügen:

1. To access administrative tools, click the [!DNL AEM] logo from the toolbar at the top.

   ![](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **Suchformulare**.

   ![](assets/navigation-panel-1.png)

3. Wählen Sie auf der Seite **Suchformulare** die Option **Asset-Admin-Suchschiene** aus.

   ![](assets/search-forms-page.png)

4. Klicken Sie in der Symbolleiste oben auf **Bearbeiten**, um die Seite „Suchformular bearbeiten“ zu öffnen.

   ![](assets/edit-search-form-1.png)

5. In the **Edit Search Form** page, drag a predicate from the **Select Predicate** tab to the main pane. For example, drag **Property Predicate**.

   Das Feld **Eigenschaft** wird im Hauptbereich angezeigt und die Registerkarte **Einstellungen** auf der rechten Seite zeigt die Eigenschaftsprädikate an.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >Mit der Kopfzeilenbeschriftung auf der Registerkarte **Einstellungen** wird der Typ der gewählten Eigenschaft identifiziert.

6. Geben Sie auf der Registerkarte **Einstellungen** eine Beschriftung, Platzhaltertext und eine Beschreibung für das Eigenschaftsprädikat ein.

   * Select **Partial Search**, if you want to allow partial phrase search (and wildcard search) of assets-based on the specified property value. Das Prädikat unterstützt standardmäßig die Volltextsuche.
   * Select **Ignore Case**, if you want the asset search based on property value to be non-case sensitive. Standardmäßig wird bei der Suche nach Eigenschaftswerten im Suchfilter zwischen Groß- und Kleinschreibung unterschieden.
   >[!NOTE]
   >
   >Nach Aktivierung des Kontrollkästchens **Teilsuche** wird **Groß-/Kleinschreibung ignorieren** standardmäßig aktiviert.

7. In the **Property Name** field, open property picker and select the property based on which the search is performed. Alternativ können Sie einen Namen für die Eigenschaft eingeben. For example, enter `  jcr :content/metadata/dc:title` or `./jcr:content/metadata/dc:title`.

   ![](assets/title-prop.png)

8. Klicken Sie auf **Fertig**, um die Einstellungen zu speichern.
9. From the **Assets** user interface, click the overlay icon and choose **Filter** to navigate to the **Filters** panel. The **Property** predicate is added to the panel.

   ![](assets/property-filter-panel.png)

10. Geben Sie in das Textfeld **Eigenschaft** einen Titel für das Asset ein, das gesucht werden soll. Geben Sie beispielsweise „Adobe“ ein. Wenn Sie eine Suche durchführen, werden Assets, deren Titel „Adobe“ entspricht, in den Suchergebnissen angezeigt.

## Liste der Sucheigenschaften {#list-of-search-predicates}

Similar to the way you add a **Property** predicate, you can add the following predicates to the **Filters** panel:

| **Eigenschaftsname** | **Beschreibung** | **Eigenschaften** |
|-------|-------|----------|
| Pfadbrowser | Sucheigenschaft, um Assets in einem bestimmten Speicherort zu suchen. **Hinweis:***Für einen angemeldeten Benutzer zeigt der Pfad-Browser auf Filter nur die Inhaltsstruktur der Ordner (und deren Vorgänger) an, die für den Benutzer freigegeben wurden.* <br> Administratoren können nach Assets in einem beliebigen Ordner suchen, indem sie mit dem Pfadbrowser zu diesem Ordner navigieren. <br> Benutzer ohne Administratorrechte können die Assets in einem Ordner (Zugriff darauf) durchsuchen, indem sie in den Pfad-Browser navigieren. | <ul><li>Feldbezeichnung</li><li>Pfad</li><li>Beschreibung</li></ul> |
| Eigenschaft | Sucht nach Assets basierend auf einer bestimmten Metadaten-Eigenschaft. **Hinweis:***Beim Auswählen der partiellen Suche ist standardmäßig "Groß-/Kleinschreibung ignorieren" ausgewählt*. | <ul><li>Feldbezeichnung</li><li>Platzhalter</li><li>Eigenschaftsname</li><li>Teilsuche</li><li>Groß-/Kleinschreibung ignorieren</li><li> Beschreibung</li></ul> |
| Mehrwert-Eigenschaft | Similar to property predicate but allows multiple input values, separated by a delimiter (default is COMMA[,]) assets matching any of the input values are returned in results. | <ul><li>Feldbezeichnung</li><li>Platzhalter</li><li>Eigenschaftsname</li><li>Trennzeichen-Unterstützung</li><li>Groß-/Kleinschreibung ignorieren</li><li>Beschreibung</li></ul> |
| Tags | Sucheigenschaft, um Assets basierend auf Tags zu suchen. Sie können die Pfadeigenschaft konfigurieren, um verschiedene Tags in der Tag-Liste zu füllen. *Hinweis: Administratoren müssen ggf. den Pfadwert ändern, z.* `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`*B. wenn sie das Suchformular veröffentlichen[!DNL AEM], wo der Pfad beispielsweise keine Mandanten-Informationen enthält*`/etc/tags/<custom_tag_namespace>`. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Pfad</li><li>Beschreibung</li></ul> |
| Pfad | Sucheigenschaft, um Assets in einem bestimmten Speicherort zu suchen. | <ul><li>Feldbezeichnung</li><li>Pfad</li><li>Beschreibung</li></ul> |  |
| Relatives Datum | Sucheigenschaft, um Assets basierend auf dem relativen Datum ihrer Erstellung zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Relatives Datum</li></ul> |
| Bereich | Sucheigenschaft, um Assets innerhalb eines bestimmten Eigenschaftswert-Bereichs zu suchen. Im Filterbedienfeld können Sie die minimalen und maximalen Eigenschaftswerte für den Bereich festlegen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| Datumsbereich | Sucheigenschaft, um Assets zu suchen, die innerhalb eines bestimmten Bereichs für eine Datumseigenschaft erstellt wurden. Im Bereich „Filter“ können Sie das Start- und das Enddatum angeben. | <ul><li>Feldbezeichnung</li><li>Platzhalter</li><li>Eigenschaftsname</li><li>Textbereich (von)</li><li>Textbereich (bis)</li><li>Beschreibung</li></ul> |
| Datum | Sucheigenschaft für eine Schieberegler-basierte Suche nach Assets basierend auf einer Datumseigenschaft | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| Dateigröße | Sucheigenschaft, um Assets basierend auf ihrer Größe zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Pfad</li><li>Beschreibung</li></ul> |
| Asset zuletzt geändert | Sucheigenschaft, um Assets basierend auf dem Datum der letzten Änderung zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| Genehmigungsstatus | Sucheigenschaft, um Assets basierend auf der Genehmigungsstatus-Eigenschaft zu suchen. Der Eigenschaftsname lautet standardmäßig **dam:status**. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| Checkout-Status | Search predicate to search assets based on the check-out status of an asset when it was published from [!DNL AEM] Assets. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| Ausgecheckt von | Sucheigenschaft, um Assets basierend auf dem Benutzer zu suchen, der das Asset ausgecheckt hat. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| Gültigkeitsstatus | Suchen Sie Predicate, um Assets basierend auf dem Ablaufstatus zu suchen. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |
| Mitglied der Sammlung | Sucheigenschaft, um Assets basierend darauf zu suchen, ob ein Asset zu einer Sammlung gehört. | Beschreibung |
| Ausgeblendet | Diese Eigenschaft ist für Endbenutzer nicht ausdrücklich sichtbar und wird bei versteckten Beschränkungen verwendet, meist zum Einschränken der Suchergebnistypen auf **dam:Asset**. | <ul><li>Feldbezeichnung</li><li>Eigenschaftsname</li><li>Beschreibung</li></ul> |

>[!NOTE]
>
>Do not use **Options Predicate**, **Publish Status Predicate**, and **Rating Predicate** as these predicates are not functional in [!DNL Brand Portal].

## Löschen von Sucheigenschaften {#delete-a-search-predicate}

Führen Sie die folgenden Schritte aus, um eine Sucheigenschaft zu löschen:

1. Klicken Sie auf das Adobe-Logo, um auf die Admin Tools zuzugreifen.

   ![](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **Suchformulare**.

   ![](assets/navigation-panel-2.png)

3. Wählen Sie auf der Seite **Suchformulare** die Option **Asset-Admin-Suchschiene** aus.

   ![](assets/search-forms-page.png)

4. Klicken Sie in der Symbolleiste oben auf **Bearbeiten**, um die Seite „Suchformular bearbeiten“ zu öffnen.

   ![](assets/edit-search-form-2.png)

5. In the **Edit Search Form** page, from the main pane, select the predicate you want to delete. For example, select **Property Predicate**.

   Die Registerkarte **Einstellungen** auf der rechten Seite zeigt die Eigenschaftsprädikat-Felder an.

6. Klicken Sie zum Löschen des Eigenschaftsprädikats auf das Papierkorbsymbol. Klicken Sie im Dialogfeld **Feld löschen** auf **Löschen**, um die Löschaktion zu bestätigen.

   Das Feld **Eigenschaftsprädikat** wird vom Hauptbereich entfernt und die Registerkarte **Eigenschaften** wird leer angezeigt.

   ![](assets/search-form-delete-predicate.png)

7. To save the changes, click **Done** in the toolbar.
8. From the **Assets** user interface, click the overlay icon and choose **Filter** to navigate to the **Filters** panel. The **Property** predicate is removed from the panel.

   ![](assets/property-predicate-removed.png)
