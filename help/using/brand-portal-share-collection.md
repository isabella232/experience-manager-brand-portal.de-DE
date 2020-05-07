---
title: Freigeben von Sammlungen
seo-title: Freigeben von Sammlungen
description: AEM Assets Brand Portal-Administratoren können Sammlungen oder Smart-Sammlungen für autorisierte Benutzer freigeben oder deren Freigabe aufheben. Bearbeiter können nur die Sammlungen anzeigen und freigeben, die sie selbst erstellt haben, die für sie freigegeben wurden oder die als „Öffentlich“ festgelegt sind.
seo-description: AEM Assets Brand Portal-Administratoren können Sammlungen oder Smart-Sammlungen für autorisierte Benutzer freigeben oder deren Freigabe aufheben. Bearbeiter können nur die Sammlungen anzeigen und freigeben, die sie selbst erstellt haben, die für sie freigegeben wurden oder die als „Öffentlich“ festgelegt sind.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: ht
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: ht
source-wordcount: '512'
ht-degree: 100%

---


# Sammlungen in Brand Portal freigeben {#share-collections-bp}

AEM Assets Brand Portal-Administratoren können Sammlungen oder Smart-Sammlungen für autorisierte Benutzer freigeben oder deren Freigabe aufheben. Bearbeiter können nur die Sammlungen anzeigen und freigeben, die sie selbst erstellt haben, die für sie freigegeben wurden oder die als „Öffentlich“ festgelegt sind. Bearbeiter können jedoch eine öffentliche Sammlung nicht in eine nicht öffentliche Sammlung ändern.

>[!NOTE]
>
>Bearbeiter können eine öffentliche Sammlung nicht in eine nicht öffentliche Sammlung ändern. Daher steht für sie das Kontrollkästchen **[!UICONTROL Öffentliche Sammlung]** im Dialogfeld **[!UICONTROL Einstellungen für Sammlung]** nicht zur Verfügung.

## Freigeben von Sammlungen {#share-collection}

Gehen Sie wie folgt vor, um eine Sammlung freizugeben:

1. Klicken Sie links auf das Überlagerungssymbol und wählen Sie dann **[!UICONTROL Navigation]**.

   ![](assets/contenttree-1.png)

1. Klicken Sie links in der Seitenleiste auf **[!UICONTROL Sammlungen]**.

   ![](assets/access_collections.png)

1. Führen Sie in der Konsole **[!UICONTROL Sammlungen]** einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Sammlung, die Sie freigeben möchten. Klicken Sie in den verfügbaren Schnellzugriff-Miniaturansichten der Sammlung auf das Symbol **[!UICONTROL Einstellungen]**.
   ![](assets/settings_thumbnail.png)

   * Wählen Sie die Sammlung aus, die Sie freigeben möchten. Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Einstellungen]**.
   ![](assets/collection-sharing.png)

1. Wählen Sie im Dialogfeld [!UICONTROL Einstellungen für Sammlung] die Benutzer oder Gruppen aus, für die Sie die Sammlung freigeben möchten, und wählen Sie für einen Benutzer oder eine Gruppe die Rolle aus, die seiner bzw. ihrer globalen Rolle entspricht. Weisen Sie zum Beispiel die Rolle „Bearbeiter“ einem globalen Bearbeiter und die Rolle „Betrachter“ einem globalen Betrachter zu.

   Um die Sammlung dagegen für alle Benutzer unabhängig von der Gruppenmitgliedschaft und Rolle verfügbar zu machen, aktivieren Sie das Kontrollkästchen **[!UICONTROL Öffentliche Sammlung]**, damit die Sammlung als „Öffentlich“ festgelegt ist.

   >[!NOTE]
   >
   >Sie können festlegen, dass Nicht-Administrator-Benutzer Sammlungen nicht als „Öffentlich“ festlegen können, um zu verhindern, dass eine große Anzahl öffentlicher Sammlungen erstellt wird. Auf diese Weise wird Systemspeicherplatz eingespart. Unternehmen können die Konfigurationseinstellung **[!UICONTROL Erstellung öffentlicher Sammlungen zulassen]** in den [!UICONTROL Allgemeinen Einstellungen] im Admin Tools-Bereich deaktivieren.

   ![](assets/collection_sharingadduser.png)

   Bearbeiter können eine öffentliche Sammlung nicht in eine nicht öffentliche Sammlung ändern. Daher steht für sie das Kontrollkästchen **[!UICONTROL Öffentliche Sammlung]** im Dialogfeld **[!UICONTROL Einstellungen für Sammlung]** nicht zur Verfügung.

   ![](assets/collection-setting-editor.png)

1. Wählen Sie **[!UICONTROL Hinzufügen]** und dann **[!UICONTROL Speichern]** aus. Die Sammlung wird für die ausgewählten Benutzer freigegeben.

   >[!NOTE]
   >
   >Die Rolle der Benutzer legt fest, welchen Zugriff sie auf die Assets und Ordner in der Sammlung erhalten. Wenn ein Benutzer keinen Zugriff auf Assets hat, wird eine leere Sammlung für den Benutzer freigegeben. Die Rolle der Benutzer legt außerdem fest, welche Aktionen ihnen für die Sammlung zur Verfügung stehen.

## Freigabe von Sammlungen aufheben     {#unshare-a-collection}

Gehen Sie wie folgt vor, um die Freigabe einer zuvor freigegebenen Sammlung aufzuheben:

1. Wählen Sie in der Konsole **[!UICONTROL Sammlungen]** die Sammlung aus, deren Freigabe Sie aufheben möchten.

   Klicken Sie in der Symbolleiste auf **[!UICONTROL Einstellungen]**.

   ![](assets/collection_settings.png)

1. Klicken Sie im Dialogfeld **[!UICONTROL Einstellungen für Sammlung]** unter **[!UICONTROL Mitglieder]** auf das Symbol **[!UICONTROL x]** neben Benutzern oder Gruppen, um sie aus der Liste der Benutzer zu entfernen, für die die Sammlung freigegeben ist.

   ![](assets/unshare_collection.png)

1. Klicken Sie in der Warnmeldung auf **[!UICONTROL Bestätigen]**, um das Aufheben der Freigabe zu bestätigen.

   Klicken Sie auf **[!UICONTROL Speichern]**.

1. Melden Sie sich bei Brand Portal mit den Anmeldeinformationen des Benutzers an, den Sie aus der freigegebenen Liste entfernt haben. Die Sammlung wird aus der Konsole **[!UICONTROL Sammlungen]** entfernt.
