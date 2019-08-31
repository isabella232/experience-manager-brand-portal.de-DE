---
title: Verwalten von Benutzern, Gruppen und Benutzerrollen
seo-title: Verwalten von Benutzern, Gruppen und Benutzerrollen
description: Administratoren können mit Adobe Admin Console Benutzer und Produktprofile für AEM Assets Brand Portal erstellen und ihre Rollen mithilfe der Brand Portal-Benutzeroberfläche verwalten. Diese Berechtigung ist für Betrachter und Bearbeiter nicht verfügbar.
seo-description: Administratoren können mit Adobe Admin Console Benutzer und Produktprofile für AEM Assets Brand Portal erstellen und ihre Rollen mithilfe der Brand Portal-Benutzeroberfläche verwalten. Diese Berechtigung ist für Betrachter und Bearbeiter nicht verfügbar.
uuid: 0 dc 1867 c -6 d 1 b -4 d 0 d-a 25 e -0 df 207 c 269 b 8
content-type: Referenz
topic-tags: Administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: ba 468 e 80-d 077-4 af 6-b 782-238 fc 557 e 22 b
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Manage Users, Groups, and User Roles {#manage-users-groups-and-user-roles}

Administratoren können mit Adobe Admin Console Benutzer und Produktprofile für AEM Assets Brand Portal erstellen und ihre Rollen mithilfe der Brand Portal-Benutzeroberfläche verwalten. Diese Berechtigung ist für Betrachter und Bearbeiter nicht verfügbar.

In [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview), you can view all the products associated with your organization. Bei diesen Produkten kann es sich um beliebige Experience Cloud-Lösungen handeln, z. B. Adobe Analytics, Adobe Target oder AEM Brand Portal. Sie müssen das Produkt „AEM Brand Portal“ wählen und Produktprofile anlegen.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

Diese Produktprofile werden alle 8 Stunden mit der Marken-Portal-Benutzeroberfläche synchronisiert und als Gruppen in Brand Portal angezeigt. Nachdem Sie Benutzer hinzugefügt und Produktprofile erstellt und Benutzer zu diesen Produktprofilen hinzugefügt haben, können Sie Benutzern und Gruppen im Markenportal Rollen zuweisen.

>[!NOTE]
>
>To create groups in Brand Portal, from Adobe [!UICONTROL Admin Console], use **[!UICONTROL Products &gt; Product Profiles]**, instead of **[!UICONTROL User page &gt; User Groups]**. Product profiles in Adobe [!UICONTROL Admin Console] are used to create groups in Brand Portal.

## Hinzufügen von Benutzern {#add-a-user}

If you are a product administrator, use Adobe [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) to create users and assign them to product profiles (*formerly known as product configurations*), which show as groups in Brand Portal. Sie können mit Gruppen Massenvorgänge wie Rollenverwaltung und Asset-Freigabe durchführen.

>[!NOTE]
Neue Benutzer ohne Zugriff auf Brand Portal können über den Brand Portal-Anmeldebildschirm den Zugriff anfordern. Weitere Informationen finden Sie unter [Anfordern von Zugriff auf Brand Portal](../using/brand-portal.md#request-access-to-brand-portal). After you receive access request notifications in your notification area, click the relevant notification and then click **[!UICONTROL Grant Access]**. Sie können auch den Link in der Zugriffsanforderungs-E-Mail erhalten. Next, to add a user through [Adobe [!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview), follow Steps 4-7 in the procedure below.

>[!NOTE]
You can login to [Adobe [!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directly or from Brand Portal. Wenn Sie sich direkt anmelden, befolgen Sie die unten beschriebenen Schritte 4 bis 7, um einen Benutzer hinzuzufügen.

1. Klicken Sie in der AEM-Symbolleiste oben auf das Adobe-Logo, um auf Verwaltungswerkzeuge zuzugreifen.

   ![AEM-Logo](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin Tools-Bedienfeld](assets/admin-tools-panel-5.png)

3. In the [!UICONTROL User Roles] page, click the **[!UICONTROL Management]** tab, then click **[!UICONTROL Launch Admin Console]**.

   ![Benutzerrollen zum Starten der Admin-Konsole](assets/launch_admin_console.png)

4. Führen Sie in Admin Console einen der folgenden Schritte aus, um einen neuen Benutzer zu erstellen:

   * Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Überblick]**. In the [!UICONTROL Overview] page, click **[!UICONTROL Assign Users]** from the Brand Portal product card.
   ![Überblick über die Admin-Konsole](assets/admin_console_overviewadduser.png)

   * Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Benutzer]**. In the [!UICONTROL Users] page, [!UICONTROL Users] in the left rail is selected by default. Click **[!UICONTROL Add User]**.
   ![Benutzer der Admin-Konsole hinzufügen](assets/admin_console_adduseruserpage.png)

5. Geben Sie im Dialogfeld „Benutzer hinzufügen“ die E-Mail-Adresse des Benutzers ein, den Sie hinzufügen möchten, oder wählen Sie den Benutzer aus der Liste mit Vorschlägen aus, die erscheint, wenn Sie mit der Eingabe beginnen.

   ![Benutzer zum Markenportal hinzufügen](assets/add_user_to_aem_bp.png)

6. Weisen Sie den Benutzer mindestens einem Produktprofil (ehemals „Produktkonfiguration“) zu, damit der Benutzer auf Brand Portal zugreifen kann. Wählen Sie im Feld **[!UICONTROL Wählen Sie ein Profil für dieses Produkt aus]das entsprechende Produktprofil aus.**
7. Klicken Sie auf **[!UICONTROL Speichern]**. An den hinzugefügten Benutzer wird eine Begrüßungs-E-Mail gesendet. The invited user can access Brand Portal by clicking the link in the welcome email and signing in using an [!UICONTROL Adobe ID]. Weitere Informationen finden Sie unter [Schritte bei der ersten Anmeldung](../using/brand-portal-onboarding.md).

   >[!NOTE]
   If a user is unable to log on to Brand Portal, the Administrator of the organization should visit Adobe [!UICONTROL Admin Console] and check whether the user is present and has been added to at least one product profile.

   Informationen zum Gewähren von Administratorrechten für Benutzer finden Sie unter [Bereitstellen von Administratorrechten für Benutzer](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Hinzufügen von Produktprofilen {#add-a-product-profile}

Product profiles (formerly known as product configurations) in [!UICONTROL Admin Console] are used to create groups in Brand Portal so that you can perform bulk operations such as role management and asset sharing in Brand Portal. **Brand Portal** ist standardmäßig als Produktprofil verfügbar. Sie können weitere Produktprofile erstellen und Benutzer zu den neuen Produktprofilen hinzufügen.

>[!NOTE]
You can login to [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directly or from Brand Portal. If you login to [!UICONTROL Admin Console] directly, follow Steps 4-7 in the procedure below to add a product profile.

1. Klicken Sie in der AEM-Symbolleiste oben auf das Adobe-Logo, um auf Verwaltungswerkzeuge zuzugreifen.

   ![AEM-Logo](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin Tools-Bedienfeld](assets/admin-tools-panel-6.png)

3. In the [!UICONTROL User Roles] page, click the **[!UICONTROL Management]** tab, then click **[!UICONTROL Launch Admin Console]**.

   ![Admin-Konsole starten](assets/launch_admin_console.png)

4. Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Produkte]**.
5. In the [!UICONTROL Products] page, [!UICONTROL Product Profiles] is selected by default. Click **[!UICONTROL New Profile]**.

   ![Neues Produktprofil hinzufügen](assets/admin_console_addproductprofile.png)

6. Geben Sie auf der Seite [!UICONTROL Neues Profil erstellen] Profilname, Anzeigename und Profilbeschreibung ein und wählen Sie aus, ob Benutzer per E-Mail benachrichtigt werden sollen, wenn sie zum Profil hinzugefügt oder daraus entfernt werden.

   ![Produktprofil erstellen](assets/admin_console_addaproductprofilecreatenewprofile.png)

7. Klicken Sie auf **[!UICONTROL Fertig]**. The product configuration group, for example **[!UICONTROL Sales group]**, is added to Brand Portal.

   ![Produktprofile](assets/admin_console_productprofileadded.png)

## Hinzufügen von Benutzern zu Produktprofilen {#add-users-to-a-product-profile}

To add users to a Brand Portal group, add them to the corresponding product profile (formerly known as product configurations) in [!UICONTROL Admin Console]. Sie können Benutzer einzeln oder mehrere Benutzer auf einmal hinzufügen.

>[!NOTE]
You can login to [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directly or from Brand Portal. Wenn Sie sich direkt bei Admin Console anmelden, befolgen Sie die unten beschriebenen Schritte 4 bis 7, um Benutzer zu einem Produktprofil hinzuzufügen.

1. Klicken Sie in der AEM-Symbolleiste oben auf das Adobe-Logo, um auf Verwaltungswerkzeuge zuzugreifen.

   ![AEM-Logo](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin Tools-Bedienfeld](assets/admin-tools-panel-7.png)

3. In the [!UICONTROL User Roles] page, click the **[!UICONTROL Management]** tab, then click **[!UICONTROL Launch Admin Console]**.

   ![Start [!DNL Admin Console]](assets/launch_admin_console.png)

4. Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Produkte]**.
5. In the [!UICONTROL Products] page, [!UICONTROL Product Profiles] is selected by default. Open the product profile to which you want to add a user, for example, [!UICONTROL Sales group].

   ![Produktprofile](assets/admin_console_productprofileadded.png)

6. Gehen Sie wie folgt vor, um einzelne Benutzer zum Produktprofil hinzuzufügen:

   * Click **[!UICONTROL Add User]**.
   ![Gruppe zum Zuordnen des Produktprofils im Markenportal](assets/admin_console_productprofilesalesgroup.png)

   * In the [!UICONTROL Add User to Sales group] page, type the email ID of the user you want to add or select the user from the list of suggestions that appear as you type.
   ![Benutzer zu einer Gruppe hinzufügen](assets/admin_console_addusertosalesgroup.png)

   * Klicken Sie auf **[!UICONTROL Speichern]**.



7. Gehen Sie wie folgt vor, um mehrere Benutzer zum Produktprofil hinzuzufügen:

   * Choose ellipsis (**[!UICONTROL ...) &gt; Add users by CSV]**.
   ![Stapelweises Hinzufügen von Benutzern](assets/admin_console_addbulkusers.png)

   * In the **[!UICONTROL Add Users by CSV]** page, download a CSV template or drag-and-drop a CSV file.
   ![Benutzer durch CSV hinzufügen](assets/admin_console_addbulkuserscsv.png)

   * Klicken Sie auf **[!UICONTROL Hochladen]**.
   Wenn Sie Benutzer dem Standardproduktprofil hinzugefügt haben, also dem Markenportal, wird eine Begrüßungs-E-Email an die E-Email-ID der hinzugefügten Benutzer gesendet. The invited users can access Brand Portal by clicking the link in the welcome email and signing in using an [!UICONTROL Adobe ID]. Weitere Informationen finden Sie unter [Schritte bei der ersten Anmeldung](../using/brand-portal-onboarding.md).

   Benutzer, die zu einem benutzerdefinierten oder neuen Produktprofil hinzugefügt werden, erhalten keine E-Mail-Benachrichtigung.

## Bereitstellen von Administratorrechten für Benutzer {#provide-administrator-privileges-to-users}

Sie können Brand Portal-Benutzern Berechtigungen als Systemadministrator oder Produkt-Administrator gewähren. Do not provide other administrative rights available in [!UICONTROL Admin Console], such as product profile administrator, user group administrator, and support administrator. Weitere Informationen zu diesen Rollen finden Sie unter [Administratorrollen](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
You can login to [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directly or from Brand Portal. If you login to [!UICONTROL Admin Console] directly, follow Steps 4-8 in the procedure below to add a user to a product profile.

1. Klicken Sie in der AEM-Symbolleiste oben auf das Adobe-Logo, um auf Verwaltungswerkzeuge zuzugreifen.

   ![Aemlogo](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin Tools-Bedienfeld](assets/admin-tools-panel-8.png)

3. In the [!UICONTROL User Roles] page, click the **[!UICONTROL Management]** tab, then click **[!UICONTROL Launch Admin Console]**.

   ![Admin-Konsole starten](assets/launch_admin_console.png)

4. Klicken Sie oben in der Symbolleiste auf **[!UICONTROL Benutzer]**.
5. In the [!UICONTROL Users] page, [!UICONTROL Users] in the left rail is selected by default. Klicken Sie auf den Benutzernamen des Benutzers, dem Sie Administratorrechte gewähren möchten.

   ![Benutzer in der Admin-Konsole hinzufügen](assets/admin_console_adduseruserpage.png)

6. In the user profile page, locate the **[!UICONTROL Administrative Rights]** section at the bottom, and choose ellipsis (**[!UICONTROL ... &gt; Edit admin rights]**.
   ![Administratorrechte in der Admin-Konsole](assets/admin_console_editadminrights.png)

7. Wählen Sie auf der Seite [!UICONTROL Administratorrechte bearbeiten] die Option „Systemadministrator“ bzw. „Produkt-Administrator“ aus.

   ![Administratorrechte in der Admin-Konsole bearbeiten](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   Marken Portal unterstützt nur die Rollen Systemadministrator und Produktadministrator.
   Adobe empfiehlt, die Rolle „Systemadministrator“ zu vermeiden, da sie für alle Produkte des jeweiligen Unternehmens unternehmensweite Administratorrechte gewährt. Beispielsweise verfügt ein Systemadministrator einer Organisation, der drei Marketing Cloud-Produkte enthält, über sämtliche Berechtigungen für alle drei Produkte. Nur ein Systemadministrator kann AEM Assets konfigurieren, damit Assets über AEM Assets in Brand Portal veröffentlicht werden können. For more information, see [Configure AEM Assets integration with Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html).
   Im Gegensatz dazu gewährt die Rolle „Produkt-Administrator“ ausschließlich Administratorrechte für ein bestimmtes Produkt. Wenn Sie eine granularere Zugriffssteuerung im Brand Portal erzwingen möchten, verwenden Sie die Rolle "Produktadministrator" und wählen Sie das Produkt als Markenportal aus.

   >[!NOTE]
   Die Administratorrolle „Produktprofil-Administrator“ (ehemals „Konfigurations-Administrator“) wird in Brand Portal nicht unterstützt. Vermeiden Sie die Zuweisung der Administratorrolle „Produktprofil-Administrator“ zu Benutzern.

8. Überprüfen Sie die Auswahl des Administratortyps und klicken Sie auf **[!UICONTROL Speichern]**.

   >[!NOTE]
   Um die Administratorrechte für einen Benutzer zu widerrufen, nehmen Sie auf der Seite [!UICONTROL Administratorrechte bearbeiten] die entsprechenden Änderungen vor und klicken Sie auf **[!UICONTROL Speichern]**.

## Verwalten von Benutzerrollen {#manage-user-roles}

Administratoren können die Rollen für Benutzer in Brand Portal ändern.

Zusätzlich zur Administratorrolle werden in Brand Portal die folgenden Rollen unterstützt:

* [!UICONTROL Betrachter:] Benutzer mit dieser Rolle können Dateien und Ordner anzeigen, die ein Administrator für sie freigegeben hat. Betrachter können auch Assets suchen und herunterladen. However, Viewers cannot share content (files, folders, [!UICONTROL collections]) with other users.
* [!UICONTROL Bearbeiter:] Benutzer mit dieser Rolle verfügen über alle Berechtigungen eines Betrachters. In addition, Editors can share content (folders, [!UICONTROL collections], links) with other users.

1. Klicken Sie in der AEM-Symbolleiste oben auf das Adobe-Logo, um auf Verwaltungswerkzeuge zuzugreifen.

   ![Aemlogo](assets/aemlogo.png)

2. Klicken Sie im Admin Tools-Bereich auf **[!UICONTROL Benutzer]**.

   ![Admin Tools-Bedienfeld](assets/admin-tools-panel-9.png)

3. In the [!UICONTROL User Roles] page, the [!UICONTROL Users] tab is selected by default. For the user whose role you want to change, select **[!UICONTROL Editor]** or **[!UICONTROL Viewer]** from the **[!UICONTROL Role]** drop-down.

   ![Benutzerrollen ändern](assets/modify_user_role.png)

   Wenn Sie gleichzeitig die Rollen mehrerer Benutzer ändern möchten, wählen Sie die entsprechenden Benutzer aus und wählen Sie die gewünschte Rolle in der Dropdown-Liste **[!UICONTROL Rolle]aus.**

   >[!NOTE]
   Bei Administratorbenutzern ist die Liste [!UICONTROL Rolle] deaktiviert. Die Rollen für diese Benutzer können nicht ausgewählt werden.

   >[!NOTE]
   Die Auswahl der Benutzerrolle ist auch dann deaktiviert, wenn der Benutzer zu einer Gruppe mit der Rolle „Bearbeiter“ gehört. Wenn Sie die Bearbeitungsberechtigungen des Benutzers widerrufen möchten, müssen Sie den Benutzer aus der Gruppe mit der Rolle „Bearbeiter“ entfernen oder die Rolle der gesamten Gruppe in „Betrachter“ ändern.

4. Klicken Sie auf **[!UICONTROL Speichern]**. Die Rolle wird für den entsprechenden Benutzer geändert. Wenn Sie mehrere Benutzer ausgewählt haben, werden die Rollen für alle ausgewählten Benutzer gleichzeitig geändert.

   >[!NOTE]
   Changes in user permissions are reflected in the [!UICONTROL User Roles] page only after the users re-login to Brand Portal.

## Verwalten von Gruppenrollen und -berechtigungen {#manage-group-roles-and-privileges}

An Administrator can associate specific privileges with a [group](../using/brand-portal-adding-users.md#main-pars-title-278567577) of users on Brand Portal. The [!UICONTROL Groups] tab on the [!UICONTROL User Roles] page allows administrators to:

* Sie können Benutzergruppen Rollen zuweisen.
* Schränken Sie Benutzergruppen ein, die Original-Ausgabeformate von Bilddateien (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) aus Brand Portal herunterladen können.

>[!NOTE]
Bei über einen Link freigegebenen Assets wird die Zugriffsberechtigung für die Original-Ausgabeformate der Bilddateien basierend auf den Berechtigungen des Benutzers gewährt, der die Assets freigegeben hat.

Führen Sie folgende Schritte aus, um die Rolle und Rechte für den Zugriff auf ursprüngliche Darstellungen für bestimmte Gruppenmitglieder zu ändern:

1. On the [!UICONTROL User Roles] page, navigate to the **[!UICONTROL Groups]** tab.
2. Wählen Sie die Gruppen aus, deren Rollen geändert werden sollen.
3. Wählen Sie die entsprechende Rolle in der Dropdown-Liste [!UICONTROL Rolle] aus.

   To allow the members of a group to have access to original renditions of image files (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) which they download from the portal or shared link, keep the [!UICONTROL Access to  Original] option selected for that group. By default, [!UICONTROL Access to Original] option is selected for all the users. Möchten Sie verhindern, dass eine Benutzergruppe auf Original-Ausgabeformate zugreifen kann, heben Sie die Auswahl der Option für diese Gruppe auf.

   ![Benutzergruppenrollen](assets/access-original-rend.png)

   >[!NOTE]
   Wenn ein Benutzer mehreren Gruppen hinzugefügt wird und eine dieser Gruppen Beschränkungen hat, gelten die Einschränkungen für diesen Benutzer.
   Darüber hinaus gelten Einschränkungen hinsichtlich des Zugriffs auf Original-Ausgabeformate der Bilddateien nicht für Administratoren, auch wenn sie Mitglieder eingeschränkter Gruppen sind.

4. Klicken Sie auf **[!UICONTROL Speichern]**. Die Rolle wird für die entsprechenden Gruppen geändert.

   >[!NOTE]
   Die Benutzer-Gruppen-Zuweisung oder die Gruppenmitgliedschaft eines Benutzers wird alle 8 Stunden mit Brand Portal synchronisiert. Änderungen bei Benutzer- oder Gruppenrollen treten nach Abschluss der nächsten Synchronisation in Kraft.
