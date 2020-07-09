---
title: Erstellen von Beitragsordnern
seo-title: Erstellen von Beitragsordnern
description: 'Hier erhalten Sie einen Einblick in das Erstellen eines Beitragsordners in AEM Assets. '
seo-description: Hier erhalten Sie einen Einblick in das Erstellen eines Beitragsordners in AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 7ec61993e627f07c20a2e5a2b43f2daa629622d6
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 28%

---


# Erstellen von Beitragsordnern {#create-contribution-folder}


AEM-Administratoren und Nicht-Admin-Benutzer, die zum Erstellen eines neuen Ordners berechtigt sind, können einen Beitragsordner in AEM Assets erstellen.
Um einen Beitragsordner zu erstellen, erstellen Sie einen neuen Ordner vom Typ Asset Contribution, wobei sichergestellt wird, dass der erstellte neue Ordner für die Übermittlung von Assets durch die Benutzer von Brand Portal geöffnet ist.  Dadurch wird automatisch ein Workflow ausgelöst, der zwei weitere Unterordner im Beitragsordner erstellt, die als SHARED und NEW bezeichnet werden.

>[!NOTE]
>
>Sie können mehrere Beitragsordner in einem Ordner erstellen, aber Sie dürfen keinen Beitragsordner in einem anderen Beitragsordner erstellen.


So erstellen Sie einen Beitragsordner:
1. Melden Sie sich bei Ihrer AEM-Autoreninstanz an.

   Die Standard-URL lautet http:// localhost:4502/aem/start.html.

1. Navigate to **[!UICONTROL Assets]** > **[!UICONTROL Files]**. It lists all the existing folders in the AEM Assets repository.

1. Klicken Sie auf **[!UICONTROL Erstellen]**, um einen neuen Ordner zu erstellen. **[!UICONTROL Das Dialogfeld &quot;Ordner]** erstellen&quot;wird geöffnet.

1. Enter **[!UICONTROL Title]** and **[!UICONTROL Name]** of the folder and enable the **[!UICONTROL Asset Contribution]** checkbox.
Es wird empfohlen, Kleinbuchstaben ohne Leerzeichen zu verwenden, um den Ordner zu benennen.

1. Klicken Sie auf **[!UICONTROL Erstellen]**. Sie können den Beitragsordner im AEM Assets-Repository anzeigen.

   >[!NOTE]
   >
   >Ein Benutzer ohne Administratorrechte kann einen Asset-Beitragsordner erstellen und freigeben, ihn jedoch nicht ändern oder löschen.

   ![](assets/create-contribution-folder.png)

1. Klicken Sie, um den Beitragsordner zu öffnen. Es werden zwei Unterordner angezeigt: **[!UICONTROL FREIGEGEBEN]** und **[!UICONTROL NEU]**. Diese werden automatisch im Beitragsordner erstellt.

   ![](assets/contribution-folder.png)

You can now [configure the contribution folder properties](brand-portal-configure-contribution-folder-properties.md).


