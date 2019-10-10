---
title: Erstellen des Beitragsordners
seo-title: Erstellen des Beitragsordners
description: 'Hier erhalten Sie einen Einblick in das Erstellen eines Beitragsordners in AEM Assets. '
seo-description: Hier erhalten Sie einen Einblick in das Erstellen eines Beitragsordners in AEM Assets.
uuid: null
content-type: Referenz
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Create contribution folder {#create-contribution-folder}

AEM-Benutzer (Administratoren/Nicht-Admin-Benutzer) können in AEM Assets mit einer zusätzlichen **Asset Contribution** -Eigenschaft neue Ordner erstellen, um sicherzustellen, dass der erstellte neue Ordner für die Asset-Übermittlung durch Brand Portal-Benutzer geöffnet ist.  Dadurch wird automatisch ein Workflow ausgelöst, der zwei weitere Unterordner im neu erstellten Ordner " **Contribution** "erstellt, die als **SHARED** und **NEW** bezeichnet werden.

**So erstellen Sie einen neuen Beitragsordner:**
1. Anmelden bei Ihrer AEM-AutoreninstanzStandard-URL: http:// localhost:4502/aem/start.html
1. Navigieren Sie zu **[!UICONTROL Assets &gt; Dateien]**. Es werden alle vorhandenen Ordner im AEM Assets-Repository aufgelistet.
1. Click **[!UICONTROL Create]** to create a new folder. Popup-Fenster "Ordner erstellen"wird geöffnet.
1. Geben Sie **[!UICONTROL Titel]** und **[!UICONTROL Name]** des Ordners ein und markieren Sie das Kontrollkästchen **[!UICONTROL Asset Contribution]**.
Es wird empfohlen, kleine Alphabete ohne Leerzeichen zu verwenden, um den Ordner zu benennen.
1. Klicken Sie auf **[!UICONTROL Erstellen]**.
   ![](assets/create-contribution-folder.png)
1. Der neu erstellte Beitragsordner wird im AEM Assets-Repository aufgelistet.
1. Klicken Sie auf , um den Beitragsordner zu öffnen, sehen Sie zwei Unterordner -**[!UICONTROL SHARED]** und **[!UICONTROL NEW]** werden automatisch im Beitragsordner erstellt.\
   ![](assets/contribution-folder.png)

Jetzt können Sie die Eigenschaften des neu erstellten Beitragsordners konfigurieren. Siehe Eigenschaften [des Beitragsordners](brand-portal-configure-contribution-folder-properties.md)konfigurieren.