---
title: Freigeben von Sammlungen
seo-title: Freigeben von Sammlungen
description: AEM Assets Brand Portal-Administratoren können Sammlungen oder Smart-Sammlungen für autorisierte Benutzer freigeben oder deren Freigabe aufheben. Bearbeiter können nur die Sammlungen anzeigen und freigeben, die sie selbst erstellt haben, die für sie freigegeben wurden oder die als „Öffentlich“ festgelegt sind.
seo-description: AEM Assets Brand Portal-Administratoren können Sammlungen oder Smart-Sammlungen für autorisierte Benutzer freigeben oder deren Freigabe aufheben. Bearbeiter können nur die Sammlungen anzeigen und freigeben, die sie selbst erstellt haben, die für sie freigegeben wurden oder die als „Öffentlich“ festgelegt sind.
uuid: 965 f 39 cd -1378-42 c 1-a 58 a -01 e 1 bf 825 aa 3
contentOwner: bdhar
content-type: Referenz
topic-tags: Freigabe
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: f 053013 e -5981-419 f -927 e-b 5 bb 1 d 47 eae 2
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Sammlungen auf Markenportal freigeben {#share-collections-bp}

AEM Assets Brand Portal-Administratoren können Sammlungen oder Smart-Sammlungen für autorisierte Benutzer freigeben oder deren Freigabe aufheben. Bearbeiter können nur die Sammlungen anzeigen und freigeben, die sie selbst erstellt haben, die für sie freigegeben wurden oder die als „Öffentlich“ festgelegt sind. Bearbeiter können jedoch eine öffentliche Sammlung nicht in eine nicht öffentliche Sammlung ändern.

>[!NOTE]
>
>Editors cannot change a public collection to a non-public collection and, therefore, do not have [!UICONTROL Public Collection] checkbox available in [!UICONTROL Collection Settings] dialog.

## Freigeben von Sammlungen {#share-collection}

Gehen Sie wie folgt vor, um eine Sammlung freizugeben:

1. Klicken Sie links auf das Überlagerungssymbol und wählen Sie dann **[!UICONTROL Navigation]**.

   ![](assets/contenttree-1.png)

2. From the siderail on the left, click **[!UICONTROL Collections]**.

   ![](assets/access_collections.png)

3. Führen Sie in der Konsole **[!UICONTROL Sammlungen]einen der folgenden Schritte aus:**

   * Bewegen Sie den Mauszeiger über die Sammlung, die Sie freigeben möchten. Klicken Sie in den verfügbaren Schnellzugriff-Miniaturansichten der Sammlung auf das Symbol **[!UICONTROL Einstellungen].**
   ![](assets/settings_thumbnail.png)

   * Wählen Sie die Sammlung aus, die Sie freigeben möchten. From the toolbar at the top, click **[!UICONTROL Settings]**.
   ![](assets/collection-sharing.png)

4. In the [!UICONTROL Collection Settings] dialog box, select the users or groups with whom you want to share the collection and select the role for a user or a group to match their global role. Weisen Sie zum Beispiel die Rolle „Bearbeiter“ einem globalen Bearbeiter und die Rolle „Betrachter“ einem globalen Betrachter zu.

   Alternatively, to make the collection available to all users irrespective of their group membership and role, make it public by selecting the **[!UICONTROL Public Collection]** check-box.

   >[!NOTE]
   >
   >Sie können festlegen, dass Nicht-Administrator-Benutzer Sammlungen nicht als „Öffentlich“ festlegen können, um zu verhindern, dass eine große Anzahl öffentlicher Sammlungen erstellt wird. Auf diese Weise wird Systemspeicherplatz eingespart. Organizations can disable the **[!UICONTROL Allow public collections creation]** configuration from [!UICONTROL General] settings available in admin tools panel.

   ![](assets/collection_sharingadduser.png)

   Editors cannot change a public collection to a non-public collection and, therefore, do not have [!UICONTROL Public Collection] check-box available in [!UICONTROL Collection Settings] dialog.

   ![](assets/collection-setting-editor.png)

5. Select **[!UICONTROL Add]**, and then **[!UICONTROL Save]**. Die Sammlung wird für die ausgewählten Benutzer freigegeben.

   >[!NOTE]
   >
   >Die Rolle der Benutzer legt fest, welchen Zugriff sie auf die Assets und Ordner in der Sammlung erhalten. Wenn ein Benutzer keinen Zugriff auf Assets hat, wird eine leere Sammlung für den Benutzer freigegeben. Die Rolle der Benutzer legt außerdem fest, welche Aktionen ihnen für die Sammlung zur Verfügung stehen.

## Freigabe von Sammlungen aufheben {#unshare-a-collection}

Gehen Sie wie folgt vor, um die Freigabe einer zuvor freigegebenen Sammlung aufzuheben:

1. Wählen Sie in der Konsole [!UICONTROL Sammlungen] die Sammlung aus, deren Freigabe Sie aufheben möchten.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

2. On the [!UICONTROL Collection Settings] dialog box, under [!UICONTROL Members], click the **[!UICONTROL x]** symbol next to users or groups to remove them from the list of users you shared the collection with.

   ![](assets/unshare_collection.png)

3. Klicken Sie in der Warnmeldung auf **[!UICONTROL Bestätigen], um das Aufheben der Freigabe zu bestätigen.**

   Klicken Sie auf **[!UICONTROL Speichern]**.

4. Melden Sie sich bei Brand Portal mit den Anmeldeinformationen des Benutzers an, den Sie aus der freigegebenen Liste entfernt haben. Die Sammlung wird aus der Konsole **[!UICONTROL Sammlungen]entfernt.**
