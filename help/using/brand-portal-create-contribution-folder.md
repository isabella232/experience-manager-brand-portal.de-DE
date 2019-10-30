---
title: Erstellen von Beitragsordnern
seo-title: Erstellen von Beitragsordnern
description: 'Hier erhalten Sie einen Einblick in das Erstellen eines Beitragsordners in AEM Assets. '
seo-description: Hier erhalten Sie einen Einblick in das Erstellen eines Beitragsordners in AEM Assets.
uuid: null
content-type: Referenz
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: ht
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Erstellen von Beitragsordnern {#create-contribution-folder}

AEM-Benutzer (Administratoren/Benutzer ohne Administratorrechte) können in AEM Assets neue Ordner mit der zusätzlichen Eigenschaft **Asset-Beitrag** erstellen, um sicherzustellen, dass die neu erstellten Ordner von Brand Portal-Benutzern für die Übermittlung von Assets nutzbar sind. Dadurch wird automatisch ein Workflow ausgelöst, mit dem zwei weitere Unterordner namens **FREIGEGEBEN** und **NEU** im neu erstellten **Beitragsordner** erstellt werden.

**Erstellen eines neuen Beitragsordners:**
1. Melden Sie sich bei Ihrer AEM-Autoreninstanz an.
Standard-URL: http:// localhost:4502/aem/start.html
1. Navigieren Sie zu **[!UICONTROL Assets &gt; Dateien]**.
Es werden alle vorhandenen Ordner im AEM Assets-Repository aufgelistet.
1. Klicken Sie auf **[!UICONTROL Erstellen]**, um einen neuen Ordner zu erstellen. Das Popup-Fenster „Ordner erstellen“ wird geöffnet.
1. Geben Sie den **[!UICONTROL Titel]** und den **[!UICONTROL Namen]** des Ordners ein und aktivieren Sie das Kontrollkästchen **[!UICONTROL Asset-Beitrag]**.
Wir empfehlen, Kleinbuchstaben ohne Leerzeichen zu verwenden, um den Ordner zu benennen.
1. Klicken Sie auf **[!UICONTROL Erstellen]**.
   ![](assets/create-contribution-folder.png)
1. Der neu erstellte Beitragsordner wird im AEM Assets-Repository aufgelistet.
1. Klicken Sie, um den Beitragsordner zu öffnen. Es werden zwei Unterordner angezeigt: **[!UICONTROL FREIGEGEBEN]** und **[!UICONTROL NEU]**. Diese werden automatisch im Beitragsordner erstellt.\
   ![](assets/contribution-folder.png)

Jetzt können Sie die Eigenschaften des neu erstellten Beitragsordners konfigurieren. Siehe [Konfigurieren von Eigenschaften von Beitragsordnern](brand-portal-configure-contribution-folder-properties.md).