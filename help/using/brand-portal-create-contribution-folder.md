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
translation-type: ht
source-git-commit: 9c3002429d003c67b8e3f2770d5b9e39d053b20b
workflow-type: ht
source-wordcount: '291'
ht-degree: 100%

---


# Erstellen von Beitragsordnern {#create-contribution-folder}

AEM-Administratoren und Benutzer ohne Administratorrechte, die zum Erstellen eines neuen Ordners berechtigt sind, können in AEM Assets einen **Beitragsordner** erstellen.
Um einen **Beitragsordner** zu erstellen, erstellen Sie einen neuen Ordner des Typs **Asset-Beitrag** und stellen Sie sicher, dass der neu erstellte Ordner von Brand Portal-Benutzern für die Übermittlung von Assets nutzbar ist.  Dadurch wird automatisch ein Workflow ausgelöst, mit dem zwei weitere Unterordner namens **SHARED** und **NEW** im neu erstellten **Beitragsordner** erstellt werden.

**Erstellen eines neuen Beitragsordners:**
1. Melden Sie sich bei Ihrer AEM-Autoreninstanz an.
Standard-URL: http:// localhost:4502/aem/start.html
1. Navigieren Sie zu **[!UICONTROL Assets > Dateien]**.
Es werden alle vorhandenen Ordner im AEM Assets-Repository aufgelistet.
1. Klicken Sie auf **[!UICONTROL Erstellen]**, um einen neuen Ordner zu erstellen. Das Popup-Fenster „Ordner erstellen“ wird geöffnet.
1. Geben Sie **[!UICONTROL Titel]** und **[!UICONTROL Name]** des Ordners ein und aktivieren Sie das Kontrollkästchen **[!UICONTROL Asset-Beiträge]**.
Wir empfehlen, Kleinbuchstaben ohne Leerzeichen zu verwenden, um den Ordner zu benennen.
1. Klicken Sie auf **[!UICONTROL Erstellen]**.
   ![](assets/create-contribution-folder.png)
1. Der neu erstellte Beitragsordner wird im AEM Assets-Repository aufgelistet.
1. Klicken Sie, um den Beitragsordner zu öffnen. Es werden zwei Unterordner angezeigt: **[!UICONTROL FREIGEGEBEN]** und **[!UICONTROL NEU]**. Diese werden automatisch im Beitragsordner erstellt.\
   ![](assets/contribution-folder.png)

Sie können jetzt die Eigenschaften des Beitragsordners konfigurieren. Siehe [Konfigurieren von Eigenschaften von Beitragsordnern](brand-portal-configure-contribution-folder-properties.md).

>[!NOTE]
>
>Benutzer ohne Administratorrechte können Beitragsordner nur erstellen und freigeben. Stellen Sie sicher, dass Sie einen geeigneten Namen für den Beitragsordner angeben, da Benutzer ohne Administratorrechte Beitragsordner nicht ändern oder löschen können.
>
>Die Verschachtelung des Beitragsordners wird nicht unterstützt. Sie können mehrere Beitragsordner in einem Ordner erstellen, aber keinen Beitragsordner in einem anderen Beitragsordner.

