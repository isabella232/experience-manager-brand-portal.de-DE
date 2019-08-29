---
title: Anpassen von Hintergrund, Kopfzeilen und E-Mail-Nachrichten
seo-title: Anpassen von Hintergrund, Kopfzeilen und E-Mail-Nachrichten
description: Brand Portal-Administratoren können einige Aspekte der Benutzeroberfläche für Benutzer anpassen. Sie können ein bestimmtes Hintergrundbild (Bildschirmhintergrund) für die Brand Portal-Anmeldeseite auswählen, ein Kopfzeilenbild hinzufügen und die Asset-Freigabe-E-Mails an die Marke des Kunden anpassen.
seo-description: Brand Portal-Administratoren können einige Aspekte der Benutzeroberfläche für Benutzer anpassen. Sie können ein bestimmtes Hintergrundbild (Bildschirmhintergrund) für die Brand Portal-Anmeldeseite auswählen, ein Kopfzeilenbild hinzufügen und die Asset-Freigabe-E-Mails an die Marke des Kunden anpassen.
uuid: e 078 d 0 b 9-18 b 5-467 a-ae 90-7 f 0 b 9 fd 0 d 414
content-type: Referenz
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: Administration
discoiquuid: 7 b 773 a 4 f -2 d 4 e -48 d 6-b 259-436 d 0 cfbdce 9
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Anpassen von Hintergrund, Kopfzeilen und E-Mail-Nachrichten {#customize-wallpaper-header-and-email-message}

[!DNL Brand Portal] Administratoren können die für Benutzer angezeigte Benutzeroberfläche eingeschränkte Anpassungen vornehmen. You can choose a specific background image (wallpaper) for the [!DNL Brand Portal] login page. ein Kopfzeilenbild hinzufügen und die Asset-Freigabe-E-Mails an die Marke des Kunden anpassen.

## Anpassen des Hintergrundbilds für den Anmeldebildschirm {#customize-the-login-screen-wallpaper}

Wenn kein benutzerdefiniertes Hintergrundbild mit der Unternehmensmarke definiert ist, wird auf der Anmeldeseite ein Standard-Hintergrundbild verwendet.

1. From the [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Branding**.

   ![](assets/admin-tools-panel-10.png)

3. On the left rail of the **Configure Branding** page, **Wallpaper** is selected by default. Das Standard-Hintergrundbild der Anmeldeseite wird angezeigt.

   ![](assets/default_wallpaper.png)

4. To add a new background image, click the **Choose Image** icon from the toolbar at the top.

   ![](assets/choose_wallpaperimage.png)

   Führen Sie einen der folgenden Schritte aus:

   * To upload an image from your computer, click **Upload**. Navigieren Sie zum erforderlichen Bild und laden Sie es hoch.
   * To use an existing Brand Portal image, click **Select from existing**. Wählen Sie mit der Asset-Auswahl ein Bild aus.
   ![](assets/asset-picker.png)

5. Geben Sie den Kopfzeilentext und eine Beschreibung für das Hintergrundbild an. To save the changes, click **Save** from the toolbar at the top.

6. From the toolbar at the top, click the **Preview** icon to generate a preview of the Brand Portal interface with the image.

   ![](assets/chlimage_1.png)

   ![](assets/custom-wallpaper-preview.png)

7. To activate or deactivate the default wallpaper, do the following in the **Configure Branding** &gt; **Wallpaper** page:

   * To display the default wallpaper image on the Brand Portal login page, click **Deactivate Wallpaper** from the toolbar at the top. Eine Meldung bestätigt, dass das Standardbild deaktiviert wurde.
   ![](assets/chlimage_1-1.png)

   * Um das benutzerdefinierte Bild auf der Brand Portal-Anmeldeseite wiederherzustellen, klicken Sie in der Symbolleiste auf **Hintergrund aktivieren.** Eine Meldung bestätigt, dass das Bild wiederhergestellt wurde.
   ![](assets/chlimage_1-2.png)

   * Klicken Sie auf **Speichern**, um die Änderungen zu speichern.



## Anpassen der Kopfzeile {#customize-the-header}

Die Kopfzeile wird auf verschiedenen Marken Portal-Seiten angezeigt, nachdem Sie sich bei Brand Portal angemeldet haben.

1. Klicken Sie in der AEM-Symbolleiste oben auf das Adobe-Logo, um auf Verwaltungswerkzeuge zuzugreifen.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Branding**.

   ![](assets/admin-tools-panel-11.png)

3. To customize the page header for the Brand Portal interface, on the **Configure Branding** page, select **Header Image** from the left rail. Das Standard-Kopfzeilenbild wird angezeigt.

   ![](assets/default-header.png)

4. To upload a header image, click the **Choose Image** icon and choose **Upload**.

   To use an existing  [!DNL Brand Portal] image, choose **Select from existing**.

   ![](assets/choose_wallpaperimage-1.png)

   Wählen Sie mit der Asset-Auswahl ein Bild aus.

   ![](assets/asset-picker-header.png)

5. Um eine URL im Kopfzeilenbild einzubeziehen, geben Sie sie im Feld **Bild-URL** an. Sie können externe oder interne urls angeben. Interne Links können auch relative Links sein, z. B.
   `/mediaportal.html/content/dam/mac/tenant_id/tags`.
Dieser Link leitet Benutzer zum Tags-Ordner weiter.
To save the changes, click **Save** from the toolbar at the top.

   ![](assets/configure_brandingheaderimageurl.png)

6. From the toolbar at the top, click the **Preview** icon to generate a preview of the  [!DNL Brand Portal] interface with the header image.

   ![](assets/chlimage_1-3.png)
   ![](assets/custom_header_preview.png)

7. To activate or deactivate the header image, do the following in the **Configure Branding** &gt; **Header Image** page:

   * To prevent a header image from appearing on  [!DNL Brand Portal] pages, click **Deactivate Header** from the toolbar at the top. Eine Meldung bestätigt, dass das Bild deaktiviert wurde.
   ![](assets/chlimage_1-4.png)

   * To make the header image reappear on  [!DNL Brand Portal] pages, click **Activate Header** from the toolbar at the top. Eine Meldung bestätigt, dass das Bild aktiviert wurde.
   ![](assets/chlimage_1-5.png)

   * Klicken Sie auf **Speichern**, um die Änderungen zu speichern.



## Anpassen der E-Mail-Nachrichten {#customize-the-email-messaging}

Wenn Assets als Link freigegeben werden, erhalten Benutzer eine E-Mail mit dem Link. Administratoren können diese Nachrichten, d. h. das Logo, die Beschreibung und die Fußzeile dieser E-Mails, anpassen.

1. From the  [!DNL AEM] toolbar at the top, click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

2. From the administrative tools panel, click **Branding**.

   ![](assets/admin-tools-panel-12.png)

3. When assets are shared as links or downloaded through emails, and when  [!UICONTROL collections] are shared, email notifications are sent to users. To customize the email message, on the **Configure Branding** page, select **Email Message** from the left rail.

   ![](assets/configure-branding-page-email.png)

4. Um für ausgehende E-Mails ein Logo hinzuzufügen, klicken Sie oben in der Symbolleiste auf **Hochladen.**

5. Geben Sie im Bereich **Beschreibung** die E-Mail-Kopfzeile und den Fußzeilentext an. To save the changes, click **Save** from the toolbar at the top.

   >[!NOTE]
   >
   >Wenn Sie die empfohlene Größe für das Logo nicht verwenden oder wenn der Kopf- und Fußzeilentext die empfohlene Wortanzahl überschreitet, wird der Inhalt in der E-Mail möglicherweise beschädigt.
