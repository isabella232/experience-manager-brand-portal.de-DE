---
title: Veröffentlichen von Tags in Brand Portal
seo-title: Veröffentlichen von Tags in Brand Portal
description: Erfahren Sie, wie Sie Tags aus AEM Assets in Brand Portal veröffentlichen.
seo-description: Erfahren Sie, wie Sie Tags aus AEM Assets in Brand Portal veröffentlichen.
uuid: 4167367 e -1 af 8-476 b -97 a 5-730 c 43 bd 0816
topic-tags: veröffentlichen
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: Referenz
discoiquuid: 3 c 8 e 9251-195 d -4 c 56-a 9 a 9-27 bc 8 b 2 a 82 a 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Veröffentlichen von Tags in Brand Portal {#publish-tags-to-brand-portal}

Erfahren Sie, wie Sie Tags aus AEM Assets in Brand Portal veröffentlichen.

Tags sind nützlich zum Verwalten von Assets und verbessern die Suchbarkeit der Assets, mit denen sie verknüpft sind. Tags sind vergleichbar mit Suchbegriffen oder Bezeichnungen (Metadaten), die den Assets beigefügt sind. Mithilfe von Tags werden Assets bei einer Suche schnell gefunden. Informationen dazu, wie Tags den Assets in AEM Assets zugewiesen werden, finden Sie im Artikel [Verwenden von Tags zum Verwalten von Assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Tags (die mit Assets und Sammlungen in AEM verknüpft sind) werden automatisch in Brand Portal veröffentlicht, wenn Sie Assets (und Sammlungen) mit verknüpften Tags in Brand Portal. Die veröffentlichten Tags sind hilfreich bei der Suche nach verknüpften Assets.

>[!NOTE]
>
>Daher wird empfohlen, Tags exklusiv in Brand Portal zu veröffentlichen, bevor Assets (und Sammlungen) veröffentlicht werden, mit denen die Tags verknüpft sind. Hierdurch werden Assets (und Sammlungen) schneller in Brand Portal veröffentlicht.

## Manage tags {#manage-tags}

You can use the pre-existing tags to attach to an asset or create new tags from AEM Tags console (**[!UICONTROL Tools | Tagging | AEM Tags]**). In beiden Fällen müssen Sie die Tags zuerst in Brand Portal veröffentlichen und sie dann mit den entsprechenden Assets verknüpfen.

Führen Sie die folgenden Schritte aus, um Tags in AEM zu erstellen, in Brand Portal zu veröffentlichen und mit den entsprechenden Assets (oder Sammlungen) zu verknüpfen:

1. **Erstellen von Tags**
Sign in to AEM Author instance with administrative privileges, and access **[!UICONTROL AEM Tags]** console from global navigation:

   1. **[!UICONTROL Werkzeuge auswählen]**

   2. **[!UICONTROL Allgemein auswählen]**

   3. **[!UICONTROL Tagging auswählen]**

2. Select **[!UICONTROL Create]** and then select **[!UICONTROL Create Tag]** option.
3. Geben Sie Folgendes an:

   * **[!UICONTROL Titel]**
      *(Erforderlich)* Der Anzeigetitel für das Tag.
   * **[!UICONTROL Name]**
      *(Erforderlich)* Ein Name für das Tag. Wenn Sie keinen festlegen, wird ein gültiger Knotenname aus dem Titel erstellt. See [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Beschreibung**
      *(Optional)* Eine Beschreibung des Tags.
   * **Tag-Pfad** JCR-Pfad des Tags.

4. Wählen Sie **[!UICONTROL Übermitteln]aus, um das Tag zu erstellen.**

   Nachdem Sie ein Tag auf der AEM-Instanz erstellt haben, ist das Tag für die Angehängung an ein Asset verfügbar (unter Verwendung des Abschnitts "Eigenschaften" oder" Tags verwalten" dieses Assets).

5. **Veröffentlichen Sie das Tag in Brand Portal**.

   Go to **[!UICONTROL AEM Tags]** console ([!UICONTROL Tools | Tagging | AEM Tags]), select the desired tag and Publish to Brand Portal.

6. **Hängen Sie das Tag an ein Asset (oder eine Sammlung)** an.

   Wählen Sie ein Asset (oder eine Sammlung) aus und hängen Sie das gewünschte Tag mithilfe des Bereichs „Eigenschaften“ oder „Tags verwalten“ dieses Assets an. To know more about how to assign tags to assets in AEM Assets, refer [use tags to organize assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

7. **Veröffentlichen Sie die Assets (oder Sammlungen) in Brand Portal**.\
   Wenn Sie ein Asset (oder eine Sammlung) in Brand Portal veröffentlichen, ist das beigefügte Tag auch in Brand Portal verfügbar.

   Um das angehängte Tag im entsprechenden Asset (oder in der Sammlung) in Brand Portal zu sehen, melden Sie sich bei Brand Portal an und wählen Sie das Asset im Bereich „Eigenschaften“ aus.

## Suche priorisieren {#search-promote}

In AEM Assets Brand Portal können Sie bestimmte Assets priorisieren, damit sie in den Suchanfragen, die auf einem Suchbegriff-Tag basieren, ganz oben in den Suchergebnissen erscheinen.

Um ein Asset für einen Suchbegriff zu priorisieren, führen Sie die folgenden Schritte aus:

1. Öffnen Sie die Seite **[!UICONTROL Eigenschaften]eines Assets in der AEM-Autoreninstanz.**
2. Navigieren Sie zur Registerkarte **[!UICONTROL Erweitert].**
3. In **[!UICONTROL Search Promote]** within **[!UICONTROL Elevate for search keywords]** section, select **[!UICONTROL Add]** to add the search keywords or tags.

   ![](assets/search-promote.png)

4. Speichern Sie die Änderungen.
5. Veröffentlichen Sie das Asset in Brand Portal.
6. Melden Sie sich bei Brand Portal an. Rufen Sie die Registerkarte **[!UICONTROL Erweitert]** im Bereich **Eigenschaften]des Assets auf.[!UICONTROL **
Note that the **[!UICONTROL Search Promote]** keyword is also visible in the Properties of that asset.
