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
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Veröffentlichen von Tags in Brand Portal {#publish-tags-to-brand-portal}

Learn how to publish tags from [!DNL AEM] Assets to [!DNL Brand Portal].

Tags sind nützlich zum Verwalten von Assets und verbessern die Suchbarkeit der Assets, mit denen sie verknüpft sind. Tags sind vergleichbar mit Suchbegriffen oder Bezeichnungen (Metadaten), die den Assets beigefügt sind. Mithilfe von Tags werden Assets bei einer Suche schnell gefunden. To know how to assign tags to assets in [!DNL AEM] Assets, refer [use tags to organize assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Tags (associated with assets and collections in [!DNL AEM]) are auto-published to [!DNL Brand Portal] when the assets (and collections) with associated tags are published to [!DNL Brand Portal]. Die veröffentlichten Tags sind hilfreich bei der Suche nach verknüpften Assets.

>[!NOTE]
>
>It is, however, recommended to exclusively publish tags to [!DNL Brand Portal] before publishing the assets (and collections) with which the tags are associated. This ensures faster publishing of the assets (and collections) to [!DNL Brand Portal].

## Manage tags {#manage-tags}

You can use the pre-existing tags to attach to an asset or create new tags from [!DNL AEM] Tags console (**Tools | Tagging |[!DNL AEM]Tags**). In both the scenarios you must first publish the tags to [!DNL Brand Portal] and then associate them with appropriate assets.

To create tags on [!DNL AEM], publish the tags on [!DNL Brand Portal], and associate the tags with appropriate assets (or collections), follow these steps:

1. **Erstellen Sie Tags**,
die sich bei [!DNL AEM] der Autoreninstanz mit Administratorrechten anmelden, und greifen Sie über die globale Navigation auf **[!DNL AEM]Tag** -Konsole zu:

   1. **Werkzeuge auswählen**

   2. **Allgemein auswählen**

   3. **Tagging auswählen**

2. Select **Create** and then select **Create Tag** option.
3. Geben Sie Folgendes an:

   * **Titel**
      *(Erforderlich)* Der Anzeigetitel für das Tag.
   * **Name**
      *(Erforderlich)* Ein Name für das Tag. Wenn Sie keinen festlegen, wird ein gültiger Knotenname aus dem Titel erstellt. See [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Beschreibung**
      *(Optional)* Eine Beschreibung des Tags.
   * **Tag-Pfad** JCR-Pfad des Tags.

4. Wählen Sie **Übermitteln** aus, um das Tag zu erstellen.

   Once you have created a tag on [!DNL AEM] instance, the tag will be available to be attached to an asset (using Properties section or Manage Tags section of that asset).

5. **Veröffentlichen Sie das Tag auf[!DNL Brand Portal]**.

   Go to **[!DNL AEM]Tags** console (Tools | Tagging | [!DNL AEM] Tags), select the desired tag and Publish to **[!DNL Brand Portal]**.

6. **Hängen Sie das Tag an ein Asset (oder eine Sammlung)** an.

   Wählen Sie ein Asset (oder eine Sammlung) aus und hängen Sie das gewünschte Tag mithilfe des Bereichs „Eigenschaften“ oder „Tags verwalten“ dieses Assets an. To know more about how to assign tags to assets in [!DNL AEM] Assets, refer [use tags to organize assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

7. **Veröffentlichen Sie Assets (oder Sammlungen) auf[!DNL Brand Portal]**.\
   When you publish an asset (or collection) to [!DNL Brand Portal], the attached tag is also available on [!DNL Brand Portal].

   To see the attached tag on the respective asset (or collection) in [!DNL Brand Portal], log in to [!DNL Brand Portal] and select the asset, under Properties section you will see the attached Tag.

## Suche priorisieren {#search-promote}

[!DNL AEM]In Assets können Sie bestimmte Assets priorisieren, damit sie in den Suchanfragen, die auf einem Suchbegriff-Tag basieren, ganz oben in den Suchergebnissen erscheinen.[!DNL Brand Portal]

Um ein Asset für einen Suchbegriff zu priorisieren, führen Sie die folgenden Schritte aus:

1. Open the **Properties** page of an asset on [!DNL AEM] author instance.
2. Navigieren Sie zur Registerkarte **Erweitert**.
3. In **Search Promote** within **Elevate for search keywords** section, select **Add** to add the search keywords or tags.

   ![](assets/search-promote.png)

4. Speichern Sie die Änderungen.
5. Publish the asset to [!DNL Brand Portal].
6. Log in to [!DNL Brand Portal]. Rufen Sie die Registerkarte **Erweitert** im Bereich **Eigenschaften**des Assets auf.
Note that the **Search Promote** keyword is also visible in the Properties of that asset.
