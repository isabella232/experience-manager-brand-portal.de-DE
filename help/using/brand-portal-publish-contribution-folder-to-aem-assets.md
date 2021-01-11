---
title: Veröffentlichen in den Beitragsordner in AEM Assets
seo-title: Veröffentlichen in den Beitragsordner in AEM Assets
description: Hier erhalten Sie einen Einblick in die Veröffentlichung des Beitragsordners in AEM Assets in Brand Portal.
seo-description: Hier erhalten Sie einen Einblick in die Veröffentlichung des Beitragsordners in AEM Assets in Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 6eb01e2eec7de6b704976c990fb6ffacbc67471a
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 70%

---


# Veröffentlichen von Beitragsordnern in AEM Assets {#publish-contribution-folder-to-aem}

Brand Portal-Benutzer können den Beitragsordner in AEM Assets veröffentlichen, ohne Zugriff auf die AEM-Autoreninstanz zu benötigen.

Vergewissern Sie sich, dass Sie die [Asset-Anforderungen](brand-portal-download-asset-requirements.md) erfüllt haben, und laden Sie die neu erstellten Assets in den Ordner **NEU** im Beitragsordner hoch. Siehe [Hochladen von Assets in den Beitragsordner](brand-portal-upload-assets-to-contribution-folder.md).

**Veröffentlichen des Beitragsordners:**

1. Melden Sie sich bei Ihrer Brand Portal-Instanz an.

1. Wählen Sie den Beitragsordner im Brand Portal-Dashboard aus.
1. Klicken Sie auf **[!UICONTROL In AEM veröffentlichen]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem.png)

In verschiedenen Phasen des Veröffentlichungs-Workflows wird eine E-Mail-/Pulsbenachrichtigung an den Brand Portal-Benutzer und an Brand Portal-Administratoren gesendet:
1. **In Warteschlange** - Eine Benachrichtigung wird an den Brand Portal-Benutzer und Brand Portal-Administratoren gesendet, wenn ein Publishing-Workflow in Brand Portal ausgelöst wird.

1. **Abgeschlossen** - Eine Benachrichtigung wird an den Brand Portal-Benutzer und Brand Portal-Administratoren gesendet, wenn der Beitragsordner erfolgreich in AEM Assets veröffentlicht wurde.


**Status des Veröffentlichungsauftrags**

Es gibt zwei Berichte, die Administratoren zur Ansicht des Status der Asset-Beitragsordner verwenden können, die vom Markenportal nach AEM Assets veröffentlicht wurden.

* Navigieren Sie im Markenportal zu **[!UICONTROL Tools]** > **[!UICONTROL Asset Contribution Status]**. Dieser Bericht spiegelt den Status aller Veröffentlichungsaufträge in den verschiedenen Phasen des Veröffentlichungs-Workflows wider.

   ![](assets/contribution-folder-status.png)

* Navigieren Sie in der AEM Assets-Autoreninstanz zu **[!UICONTROL Tools]** > **[!UICONTROL Aufträge]**. Dieser Bericht spiegelt den finalen Status (Erfolg oder Fehler) aller Veröffentlichungsaufträge wider.

   ![](assets/publishing-status.png)




