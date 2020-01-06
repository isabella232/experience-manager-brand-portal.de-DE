---
title: Erstellen von Beitragsordnern
seo-title: Erstellen von Beitragsordnern
description: 'Hier erhalten Sie einen Einblick in das Erstellen eines Beitragsordners in AEM Assets. '
seo-description: Hier erhalten Sie einen Einblick in das Erstellen eines Beitragsordners in AEM Assets.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 22b327619eb73c0099f903bb7314d2cb2d796bc4

---


# Erstellen von Beitragsordnern {#create-contribution-folder}

AEM-Administratoren und Nicht-Admin-Benutzer, die zum Erstellen eines neuen Ordners berechtigt sind, können in AEM Assets einen **Beitragsordner** erstellen.
Um einen **Beitragsordner** zu erstellen, erstellen Sie einen neuen Ordner vom Typ &quot; **Asset Contribution**&quot;und stellen Sie sicher, dass der erstellte neue Ordner für die Übermittlung von Assets durch Brand Portal-Benutzer geöffnet ist.  Dadurch wird automatisch ein Workflow ausgelöst, mit dem zwei weitere Unterordner namens **FREIGEGEBEN** und **NEU** im neu erstellten **Beitragsordner** erstellt werden.

**Erstellen eines neuen Beitragsordners:**
1. Melden Sie sich bei Ihrer AEM-Autoreninstanz an.
Standard-URL: http:// localhost:4502/aem/start.html
1. Navigieren Sie zu **[!UICONTROL Assets > Dateien]**.
Es werden alle vorhandenen Ordner im AEM Assets-Repository aufgelistet.
1. Klicken Sie auf **[!UICONTROL Erstellen]**, um einen neuen Ordner zu erstellen. Das Popup-Fenster „Ordner erstellen“ wird geöffnet.
1. Geben Sie den **[!UICONTROL Titel]**und den**[!UICONTROL  Namen]** des Ordners ein und aktivieren Sie das Kontrollkästchen **[!UICONTROL Asset-Beitrag]**.
Wir empfehlen, Kleinbuchstaben ohne Leerzeichen zu verwenden, um den Ordner zu benennen.
1. Klicken Sie auf **[!UICONTROL Erstellen]**.   ![](assets/create-contribution-folder.png)
1. Der neu erstellte Beitragsordner wird im AEM Assets-Repository aufgelistet.
1. Klicken Sie, um den Beitragsordner zu öffnen. Es werden zwei Unterordner angezeigt: **[!UICONTROL FREIGEGEBEN]**und**[!UICONTROL  NEU]**. Diese werden automatisch im Beitragsordner erstellt.\
   ![](assets/contribution-folder.png)

Sie können jetzt die Eigenschaften des Beitragsordners konfigurieren. Siehe [Konfigurieren von Eigenschaften von Beitragsordnern](brand-portal-configure-contribution-folder-properties.md).

>[!NOTE]
>
>Stellen Sie sicher, dass Sie dem Beitragsordner einen entsprechenden Namen geben, da Sie den Ordnernamen nach der Erstellung nicht ändern können.