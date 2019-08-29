---
title: Überblick über AEM Assets Brand Portal
seo-title: Überblick über AEM Assets Brand Portal
description: Mit AEM Assets Brand Portal können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen.
seo-description: Mit AEM Assets Brand Portal können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen.
uuid: b 1 e 54 d 03-eb 2 e -488 e-af 4 d-bae 817 dd 135 a
content-type: Referenz
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: Einführung
discoiquuid: 6 aefa 298-4728-4 b 8 e-a 85 b-e 419 ee 37 f 2 f 4
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Überblick über AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

Als Vermarkter müssen Sie manchmal mit Kanalpartnern und internen Geschäftsbenutzern zusammenarbeiten, um schnell relevante digitale Inhalte für Kunden zu erstellen, zu verwalten und bereitzustellen. Die zeitnahe Bereitstellung relevanter Inhalte für die gesamte Customer Journey ist ein wichtiger Faktor für Nachfragegenerierung, Konversionen, Interaktionen und Kundenloyalität.

Die Entwicklung von Lösungen, die die effiziente und sichere Freigabe genehmigter Marken-Logos, Richtlinien, Kampagnen-Assets oder Produktfotos für erweiterte interne Teams, Partner und Reseller unterstützen, ist jedoch eine Herausforderung.

**[!DNL Adobe Experience Manager (AEM) Assets Brand Portal]** Mit können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen. Brand Portal ermöglicht effizientere Asset-Freigabe, schnellere Time-to-Market für Assets sowie verringerte Risiken von Nicht-Compliance und unbefugten Zugriff.

Mit der browserbasierten Portalumgebung können Sie Assets mühelos hochladen, durchsuchen, suchen, in einer Vorschau anzeigen und in genehmigte Formate exportieren.

## Benutzerrollen im Markenportal {#Personas}

[!DNL Brand Portal] unterstützt die folgenden Benutzerrollen:

* Gastbenutzer
* Betrachter
* Bearbeiter
* Administrator

Die folgende Tabelle enthält die Aufgaben, die Benutzer mit diesen Rollen ausführen können:

|  | **Durchsuchen** | **Suchen** | **Download** | **Ordner freigeben** | **Sammlungen freigeben** | **Assets als Link freigeben** | **Zugriff auf Admin Tools** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Gastbenutzer** | ✓* | ✓* | ✓* | x | x | x | x |
| **Betrachter** | ✓ | ✓ | ✓ | x | x | x | x |
| **Bearbeiter** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Administrator** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* Gastbenutzer können nur Assets durchsuchen, auf Assets zugreifen oder nach Assets suchen, die sich in öffentlichen Ordnern und Sammlungen befinden.

### Gastbenutzer {#guest-user}

Any user having limited access to assets on [!DNL Brand Portal] without undergoing authentication is a guest user. Über die Gastsitzung können Benutzer auf öffentliche Ordner und Sammlungen zugreifen. Als Gastbenutzer können Sie durch die Asset-Details navigieren und die vollständige Asset-Ansicht der Mitglieder öffentlicher Ordner und Sammlungen haben. You can search, download, and add public assets to [!UICONTROL lightbox collection].

In einer Gastsitzung können Sie jedoch keine Sammlungen und gespeicherten Suchen erstellen und sie weiter freigeben. Benutzer in einer Gastsitzung können nicht auf Einstellungen für Ordner und Sammlungen zugreifen und keine Assets als Link. Diese Aufgaben kann ein Gastbenutzer ausführen:

[Öffentliche Assets durchsuchen und darauf zugreifen](browse-assets-brand-portal.md)

[Nach öffentlichen Assets suchen](brand-portal-searching.md)

[Öffentliche Assets herunterladen](brand-portal-download-users.md)

[Fügen Sie Assets zu [! UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Betrachter {#viewer}

A standard user in [!DNL Brand Portal] is typically a user with the role of Viewer. Ein Benutzer mit dieser Rolle kann auf erlaubte Ordner, Sammlungen und Assets zugreifen. Der Benutzer kann außerdem Assets durchsuchen, als Vorschau anzeigen, herunterladen und exportieren (ursprüngliche oder bestimmte Ausgabeformate), Kontoeinstellungen konfigurieren sowie Assets suchen. Diese Aufgaben kann ein Betrachter ausführen:

[Assets durchsuchen](browse-assets-brand-portal.md)

[Suchen nach Assets](brand-portal-searching.md)

[Herunterladen von Assets](brand-portal-download-users.md)

### Bearbeiter {#editor}

Ein Benutzer mit der Rolle Bearbeiter kann alle Aufgaben ausführen, die einem Betrachter zur Verfügung stehen. Zusätzlich kann ein Bearbeiter die Dateien und Ordner anzeigen, die ein Administrator freigegeben hat. Ein Benutzer mit der Rolle Bearbeiter kann außerdem Inhalte (Dateien, Ordner und Sammlungen) für andere Benutzer freigeben.

Neben den Aufgaben, die ein Betrachter ausführen kann, stehen dem Bearbeiter folgende Aufgaben zur Verfügung:

[Ordner freigeben](brand-portal-sharing-folders.md)

[Sammlungen freigeben](brand-portal-share-collection.md)

[Assets als Link freigeben](brand-portal-link-share.md)

### Administrator {#administrator}

An administrator includes a user marked as system administrator or [!DNL Brand Portal] product administrator in [!UICONTROL Admin Console]. Administratoren können Systemadministratoren und Benutzer hinzufügen und entfernen, Vorgaben definieren, E-Mails an Benutzer senden sowie Portalnutzung und Speicherberichte anzeigen.

Administratoren können alle Aufgaben ausführen, die ein Bearbeiter ausführen kann. Außerdem stehen ihnen folgende Aufgaben zur Verfügung:

[Verwalten von Benutzern, Gruppen und Benutzerrollen](brand-portal-adding-users.md)

[Anpassen von Hintergrund, Seitenkopfzeilen und E-Mails](brand-portal-branding.md)

[Verwenden benutzerdefinierter Suchfacetten](brand-portal-search-facets.md)

[Verwenden von Metadatenschema-Formularen](brand-portal-metadata-schemas.md)

[Anwenden von Bildvorgaben oder dynamischen Ausgabeformaten](brand-portal-image-presets.md)

[Arbeiten mit Berichten](brand-portal-reports.md)

In addition to the above tasks, an Author in [!DNL AEM Assets] can perform the following tasks:

[Konfigurieren [! DNL AEM Assets] Integration mit [DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[Veröffentlichen Sie Ordner auf [! DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Veröffentlichen Sie Sammlungen auf [! DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alternativer Alias für Brand Portal-URL {#tenant-alias-for-portal-url}

[!DNL Brand Portal] Ab 6.4.3 können Organisationen eine alternative (Alias) URL für die vorhandene URL ihres [!DNL Brand Portal] Mandanten haben. Die Alias-URL kann durch ein alternatives Präfix in der URL erstellt werden.\
Note that only the prefix of the [!DNL Brand Portal] URL can be customized and not the entire URL. For example, an organization with existing domain **[!UICONTROL geomettrix.brand-portal.adobe.com]** can get **[!UICONTROL geomettrixinc.brand-portal.adobe.com]** created on request.

However, **[!DNL AEM] Author instance can be [configured](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) only with the tenant id URL and not with tenant alias (alternate) URL.

>[!NOTE]
>
>To get an alias for tenant name in existing portal URL, organizations need to contact **[!DNL Adobe support] with a new tenant alias creation request. Bei der Bearbeitung dieses Antrags wird zuerst geprüft, ob der Alias verfügbar ist. Trifft dies zu, wird der Alias erstellt.
>
>Um den alten Alias zu ersetzen oder zu löschen, muss der gleiche Prozess befolgt werden.

## Anfordern von Zugriff auf Brand Portal {#request-access-to-brand-portal}

Users can request access to [!DNL Brand Portal] from the login screen. These requests are sent to [!DNL Brand Portal] administrators, who grant access to users through the Adobe Admin Console. Sobald der Zugriff gewährt wurde, erhalten die Benutzer eine Benachrichtigungs-E-Mail.

Gehen Sie wie folgt vor, um Zugriff anzufragen:

1. From the [!DNL Brand Portal] login page, select the **Click here** corresponding to **Need Access?**. However, to enter the guest session, select the **Click here** corresponding to **Guest Access?**.

   ![Bildschirm "Marken-Portal-Anmeldung «](assets/bp-login-requestaccess.png)

   Die Seite **Zugriff anfragen** wird geöffnet.

2. To be able to request access to an organization’s [!DNL Brand Portal], you must have a valid [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], or [!UICONTROL Federated ID].

   In the **Request Access** page, sign in using your ID (scenario 1) or create an [!UICONTROL Adobe ID] (scenario 2):
   ![Zugriff anfordern](assets/bplogin_request_access_2.png)

   **Szenario 1**
   1. If you have an [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], or [!UICONTROL Federated ID], click **Sign In**.
The **Sign in** page opens.
   2. Provide your [!UICONTROL Adobe ID] credentials and click **Sign in**.
      ![Adobe-Anmeldung](assets/bplogin_request_access_3.png)
   You are redirected to the **Request Access** page.
   **Szenario 2**
   1. If you do not have an [!UICONTROL Adobe ID], to create one, click **Get an Adobe ID** from the **Request Access** page.
The **Sign in** page opens.
   2. Click **Get an Adobe ID**.
The **Sign up** page opens.
   3. Geben Sie Ihren Vornamen und Nachnamen, die E-Mail-Adresse und ein Kennwort ein. Click **Sign up**.
      ![](assets/bplogin_request_access_5.png)
   You are redirected to the **Request Access** page.

3. Auf der nächsten Seite werden Ihr Name und Ihre E-Email-ID zum Anfordern des Zugriffs angezeigt. Geben Sie einen Kommentar für den Administrator ein und klicken Sie dann auf **Übermitteln**.

   ![](assets/bplogin-request-access.png)

## Produktadministratoren gewähren Zugriff {#grant-access-to-brand-portal}

[!DNL Brand Portal] Produktadministratoren erhalten im [!DNL Brand Portal] Benachrichtigungsbereich und per E-Mail im Posteingang Zugriffsanforderungen.

![Zugriff auf angeforderte Benachrichtigungen](assets/bplogin_request_access_7.png)

Um Zugriff zu gewähren, müssen Produktadministratoren auf die relevante Benachrichtigung im [!DNL Brand Portal] Benachrichtigungsbereich klicken und dann auf Zugriff **gewähren**klicken.
Alternatively, product administrators can follow the link provided in the access request email to visit [!DNL Adobe Admin Console] and add the user to the relevant product configuration.
![](assets/bplogin_request_access_8.png)

You are redirected to the [[!DNL Adobe Admin Console]](https://adminconsole.adobe.com/enterprise/overview) home page. Use [!DNL Adobe Admin Console] to create users and assign them to product profiles (formerly known as product configurations), which show as groups in [!DNL Brand Portal]. For more information about adding users in [!DNL Admin Console], see [Add a user](brand-portal-adding-users.md#add-a-user) (follow Steps 4-7 in the procedure to add a user).

## Wartungsbenachrichtigung in Brand Portal {#brand-portal-maintenance-notification}

Before [!DNL Brand Portal] is scheduled to go down for maintenance, a notification is displayed as a banner after you log in to [!DNL Brand Portal]. Beispiel für eine Benachrichtigung:

![](assets/bp_maintenance_notification.png)

You can dismiss this notification and continue using [!DNL Brand Portal]. Diese Benachrichtigung wird in jeder neuen Sitzung angezeigt.

## Versions- und Systeminformationen {#release-and-system-information}

<!--* [What's new](../using/whats-new.md)-->
* [Versionshinweise](brand-portal-release-notes.md)
* [Unterstützte Dateiformate](brand-portal-supported-formats.md)

## Verwandte Ressourcen {#related-resources}

* [Adobe-Kundendienst](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [AEM-Foren](https://www.adobe.com/go/aod_forums_en)