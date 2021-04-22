---
title: Veröffentlichen von Tags in Brand Portal
seo-title: Veröffentlichen von Tags in Brand Portal
description: Erfahren Sie, wie Sie Tags aus AEM Assets in Brand Portal veröffentlichen.
seo-description: Erfahren Sie, wie Sie Tags aus AEM Assets in Brand Portal veröffentlichen.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
translation-type: ht
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: ht
source-wordcount: '623'
ht-degree: 100%

---

# Veröffentlichen von Tags in Brand Portal {#publish-tags-to-brand-portal}

Erfahren Sie, wie Sie Tags aus AEM Assets in Brand Portal veröffentlichen.

Tags sind nützlich zum Verwalten von Assets und verbessern die Suchbarkeit der Assets, mit denen sie verknüpft sind. Tags sind vergleichbar mit Suchbegriffen oder Bezeichnungen (Metadaten), die den Assets beigefügt sind. Mithilfe von Tags werden Assets bei einer Suche schnell gefunden. Informationen dazu, wie Tags den Assets in AEM Assets zugewiesen werden, finden Sie im Artikel [Verwenden von Tags zum Verwalten von Assets](https://helpx.adobe.com/de/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Tags (die mit Assets und Sammlungen in AEM verknüpft sind) werden automatisch in Brand Portal veröffentlicht, wenn die Assets (und Sammlungen) mit verknüpften Tags in Brand Portal veröffentlicht werden. Die veröffentlichten Tags sind hilfreich bei der Suche nach verknüpften Assets.

>[!NOTE]
>
>Daher wird empfohlen, Tags exklusiv in Brand Portal zu veröffentlichen, bevor Assets (und Sammlungen) veröffentlicht werden, mit denen die Tags verknüpft sind. Hierdurch werden Assets (und Sammlungen) schneller in Brand Portal veröffentlicht.

## Tags verwalten {#manage-tags}

Sie können bereits vorhandene Tags über die AEM-Tags-Konsole (**[!UICONTROL Tools | Tagging | AEM-Tags]**) an ein Asset anhängen oder neue Tags erstellen. In beiden Fällen müssen Sie die Tags zuerst in Brand Portal veröffentlichen und sie dann mit den entsprechenden Assets verknüpfen.

Führen Sie die folgenden Schritte aus, um Tags in AEM zu erstellen, in Brand Portal zu veröffentlichen und mit den entsprechenden Assets (oder Sammlungen) zu verknüpfen:

1. **Erstellen von Tags**
Melden Sie sich mit Administratorrechten bei der AEM-Autoreninstanz an und greifen Sie über die globale Navigation auf die **[!UICONTROL AEM-Tags]**-Konsole zu:

   1. Wählen Sie **[!UICONTROL Tools]**

   1. Wählen Sie **[!UICONTROL Allgemein]**

   1. Wählen Sie **[!UICONTROL Tagging]**

1. Klicken Sie auf **[!UICONTROL Erstellen]** und wählen Sie dann die Option **[!UICONTROL Tag erstellen]**.
1. Geben Sie Folgendes an:

   * **[!UICONTROL Titel]**

      *(erforderlich)* Ein Anzeigetitel für das Tag.
   * **[!UICONTROL Name]**
      *(erforderlich)* Ein Name für das Tag. Wenn Sie keinen festlegen, wird ein gültiger Knotenname aus dem Titel erstellt. Siehe [TagID](https://helpx.adobe.com/de/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Beschreibung**

      *(optional)* Eine Beschreibung des Tags.
   * **Tag-Pfad** JCR-Pfad des Tags.

1. Wählen Sie **[!UICONTROL Übermitteln]** aus, um das Tag zu erstellen.

   Sobald Sie ein Tag in der AEM-Instanz erstellt haben, kann es an ein Asset angehängt werden (im Bereich „Eigenschaften“ oder „Tags verwalten“ dieses Assets).

1. **Veröffentlichen Sie das Tag in Brand Portal**.

   Navigieren Sie zur Konsole **[!UICONTROL AEM-Tags]** ([!UICONTROL Tools | Tagging | AEM-Tags]), wählen Sie das gewünschte Tag aus und veröffentlichen Sie es in Brand Portal.

1. **Hängen Sie das Tag an ein Asset (oder eine Sammlung)** an.

   Wählen Sie ein Asset (oder eine Sammlung) aus und hängen Sie das gewünschte Tag mithilfe des Bereichs „Eigenschaften“ oder „Tags verwalten“ dieses Assets an. Informationen dazu, wie Tags den Assets in AEM Assets zugewiesen werden, finden Sie im Artikel [Verwenden von Tags zum Organisieren von Assets](https://helpx.adobe.com/de/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

1. **Veröffentlichen Sie die Assets (oder Sammlungen) in Brand Portal**.\
   Wenn Sie ein Asset (oder eine Sammlung) in Brand Portal veröffentlichen, ist das beigefügte Tag auch in Brand Portal verfügbar.

   Um das angehängte Tag im entsprechenden Asset (oder in der Sammlung) in Brand Portal zu sehen, melden Sie sich bei Brand Portal an und wählen Sie das Asset im Bereich „Eigenschaften“ aus.

## Suche priorisieren {#search-promote}

In AEM Assets Brand Portal können Sie bestimmte Assets priorisieren, damit sie in den Suchanfragen, die auf einem Suchbegriff-Tag basieren, ganz oben in den Suchergebnissen erscheinen.

Gehen Sie wie folgt vor, um ein Asset für einen Suchbegriff zu priorisieren:

1. Öffnen Sie die Seite **[!UICONTROL Eigenschaften]** eines Assets in der AEM-Autoreninstanz.
1. Navigieren Sie zur Registerkarte **[!UICONTROL Erweitert]**.
1. Klicken Sie in **[!UICONTROL Suche priorisieren]** im Bereich **[!UICONTROL Für Suchbegriffe erhöhen]** auf **[!UICONTROL Hinzufügen]**, um die Suchbegriffe oder Tags hinzuzufügen.

   ![](assets/search-promote.png)

1. Speichern Sie die Änderungen.
1. Veröffentlichen Sie das Asset in Brand Portal.
1. Melden Sie sich bei Brand Portal an. Rufen Sie die Registerkarte **[!UICONTROL Erweitert]** im Bereich **[!UICONTROL Eigenschaften]** des Assets auf.
Beachten Sie, dass der Suchbegriff aus **[!UICONTROL Suche priorisieren]** auch in den Eigenschaften dieses Assets sichtbar ist.
