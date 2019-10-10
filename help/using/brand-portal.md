---
title: Überblick über AEM Assets Brand Portal
seo-title: Überblick über AEM Assets Brand Portal
description: Mit AEM Assets Brand Portal können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen.
seo-description: Mit AEM Assets Brand Portal können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen.
uuid: b1e54d03-eb2e-48e-af4d-bae817dd135a
content-type: Referenz
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: Einführung
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee 37f2f4
translation-type: tm+mt
source-git-commit: 96d915ba146189ccddb7eb798c86c92fd55fbe3b

---


# Überblick über AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

Als Marketingexperte müssen Sie gelegentlich mit Channel-Partnern und unternehmensinternen Nutzern zusammenarbeiten, um schnell relevante Inhalte für Kunden erstellen, verwalten und liefern zu können. Die zeitnahe Bereitstellung relevanter Inhalte für die gesamte Customer Journey ist ein wichtiger Faktor für Nachfragegenerierung, Konversionen, Interaktionen und Kundenloyalität.

Die Entwicklung von Lösungen, die die effiziente und sichere Freigabe genehmigter Marken-Logos, Richtlinien, Kampagnen-Assets oder Produktfotos für erweiterte interne Teams, Partner und Reseller unterstützen, ist jedoch eine Herausforderung.

**Das Adobe Experience Manager (AEM) Asset Brand Portal** konzentriert sich auf die Notwendigkeit, effektiv mit den global verteilten Markenportalen zusammenzuarbeiten, indem es Asset-Distributions- und Asset-Beitragsfunktionen bereitstellt.

Mit der Asset-Verteilung können Sie genehmigte kreative Elemente mühelos erwerben, steuern und sicher an externe und interne Geschäftsbenutzer verteilen. Der Asset-Beitrag ermöglicht es den Benutzern des Markenportals, Assets in das Markenportal hochzuladen und in AEM Assets zu veröffentlichen, ohne Zugriff auf die Autorenumgebung zu benötigen. Die Beitragsfunktion wird als **Asset-Sourcing im Markenportal**bezeichnet. Außerdem verbessert sie die allgemeine Erfahrung des Markenportals bei der Asset-Verteilung und dem Beitrag der Markenportal-Benutzer (externe Agenturen/Teams), beschleunigt die Markteinführung von Assets und verringert das Risiko von Nichteinhaltung und unbefugtem Zugriff.
Siehe [Asset-Beschaffung im Markenportal](brand-portal-asset-sourcing.md).

Die Browser-basierte Portalumgebung erlaubt es Ihnen, Assets einfach hochzuladen, zu durchsuchen, zu suchen, in einer Vorschau anzuzeigen und in genehmigten Formaten zu exportieren.

## Benutzerrollen in Brand Portal {#Personas}

Markenportal unterstützt die folgenden Benutzerrollen:

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

Jeder Benutzer mit eingeschränktem Zugriff auf Assets in Brand Portal, der nicht authentifiziert wird, ist ein Gastbenutzer. In der Gastsitzung können Benutzer auf öffentliche Ordner und Sammlungen zugreifen. Als Gastbenutzer haben Sie die Möglichkeit, Asset-Details zu durchsuchen und Assets der Mitglieder von öffentlichen Ordnern und Sammlungen vollständig anzuzeigen. You can search, download, and add public assets to [!UICONTROL Lightbox] collection.

In einer Gastsitzung können Sie jedoch keine Sammlungen und gespeicherten Suchen erstellen und sie weiter freigeben. Benutzer in einer Gastsitzung können nicht auf Einstellungen für Ordner und Sammlungen zugreifen und keine Assets als Link. Diese Aufgaben kann ein Gastbenutzer ausführen:

[Öffentliche Assets durchsuchen und darauf zugreifen](browse-assets-brand-portal.md)

[Nach öffentlichen Assets suchen](brand-portal-searching.md)

[Öffentliche Assets herunterladen](brand-portal-download-users.md)

[Hinzufügen von Assets zu [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Betrachter {#viewer}

Ein Brand Portal-Standardbenutzer ist meist ein Benutzer mit der Rolle Betrachter. Ein Benutzer mit dieser Rolle kann auf erlaubte Ordner, Sammlungen und Assets zugreifen. Der Benutzer kann außerdem Assets durchsuchen, als Vorschau anzeigen, herunterladen und exportieren (ursprüngliche oder bestimmte Ausgabeformate), Kontoeinstellungen konfigurieren sowie Assets suchen. Diese Aufgaben kann ein Betrachter ausführen:

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

An administrator includes a user marked as system administrator or Brand Portal product administrator in [!UICONTROL Admin Console]. Administratoren können Systemadministratoren und Benutzer hinzufügen und entfernen, Vorgaben definieren, E-Mails an Benutzer senden sowie Portalnutzung und Speicherberichte anzeigen.

Ein Administrator kann alle Aufgaben ausführen, die ein Editor für die folgenden zusätzlichen Aufgaben ausführen kann:

[Verwalten von Benutzern, Gruppen und Benutzerrollen](brand-portal-adding-users.md)

[Anpassen von Hintergrund, Seitenkopfzeilen und E-Mails](brand-portal-branding.md)

[Verwenden benutzerdefinierter Suchfacetten](brand-portal-search-facets.md)

[Verwenden von Metadatenschema-Formularen](brand-portal-metadata-schemas.md)

[Anwenden von Bildvorgaben oder dynamischen Wiedergaben](brand-portal-image-presets.md)

[Arbeiten mit Berichten](brand-portal-reports.md)

Zusätzlich zu den oben genannten Aufgaben stehen AEM Assets-Autoren folgende Aufgaben zur Verfügung:

[Konfigurieren der Integration von AEM Assets mit Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[Veröffentlichen von Ordnern in Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Veröffentlichen von Sammlungen in Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alternativer Alias für Brand Portal-URL {#tenant-alias-for-portal-url}

Ab Brand Portal 6.4.3 können Unternehmen eine alternative URL (Alias) für die vorhandene URL ihres Markenportal-Mandanten haben. Die Alias-URL kann erstellt werden, indem ein alternatives Präfix in die URL eingefügt wird.\
Beachten Sie, dass nur das Präfix der Brand Portal-URL angepasst werden kann und nicht die gesamte URL. Für eine Organisation mit der vorhandenen Domäne **[!UICONTROL geomettrix.brand-portal.adobe.com]** kann beispielsweise auf Anfrage die Domäne **[!UICONTROL geomettrixinc.brand-portal.adobe.com]** erstellt werden.

Eine AEM-Autoreninstanz kann jedoch nur mit der Mandanten-ID-URL [konfiguriert](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) werden und nicht mit einer (alternativen) Mandantenalias-URL.

>[!NOTE]
>
>Um einen Alias für einen Mandantennamen in einer vorhandenen Portal-URL zu erhalten, müssen sich Organisationen an den Adobe-Support wenden und das Erstellen eines neuen Mandantenalias anfordern. Bei der Bearbeitung dieses Antrags wird zuerst geprüft, ob der Alias verfügbar ist. Trifft dies zu, wird der Alias erstellt.
>
>Um den alten Alias zu ersetzen oder zu löschen, muss der gleiche Prozess befolgt werden.

## Anfordern von Zugriff auf Brand Portal {#request-access-to-brand-portal}

Benutzer können über den Anmeldebildschirm Zugriff auf Brand Portal anfragen. These requests are sent to Brand Portal administrators, who grant access to users through the Adobe [!UICONTROL Admin Console]. Sobald der Zugriff gewährt wurde, erhalten die Benutzer eine Benachrichtigungs-E-Mail.

Gehen Sie wie folgt vor, um Zugriff anzufragen:

1. From the Brand Portal login page, select **[!UICONTROL Click here]** corresponding to **[!UICONTROL Need Access?]**. Um jedoch einer Gastsitzung beizutreten, wählen Sie **[!UICONTROL Hier klicken]** neben **[!UICONTROL Gastzugang?]**.

   ![Brand Portal-Anmeldebildschirm](assets/bp-login-requestaccess.png)

   Die Seite [!UICONTROL Zugriff anfragen] wird geöffnet.

1. To request access to an organization’s Brand Portal, you must have a valid [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], or [!UICONTROL Federated ID].

   Melden Sie sich auf der Seite [!UICONTROL Zugriff anfordern] mit Ihrer ID an (Szenario 1) oder erstellen Sie eine [!UICONTROL Adobe ID] (Szenario 2):<br />
   ![[!UICONTROL Zugriff anfordern]](assets/bplogin_request_access_2.png)

   **Szenario 1**
   1. If you have an [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], or [!UICONTROL Federated ID], click **[!UICONTROL Sign In]**.
Die Seite [!UICONTROL Anmelden] wird geöffnet.
   1. Geben Sie Ihre [!UICONTROL Adobe ID]-Anmeldedaten ein und klicken Sie auf **[!UICONTROL Anmelden]**.<br />
   ![Adobe-Anmeldung](assets/bplogin_request_access_3.png)

   Sie werden zur Seite [!UICONTROL Zugriff anfordern] weitergeleitet.<br />
   **Szenario 2**
   1. Wenn Sie noch keine [!UICONTROL Adobe ID] haben, erstellen Sie die ID, indem Sie auf der Seite **[!UICONTROL Zugriff anfordern]** auf [!UICONTROL Adobe ID anfordern] klicken.

Die Seite [!UICONTROL Anmelden] wird geöffnet.
   1. Click **[!UICONTROL Get an Adobe ID]**.
Die Seite [!UICONTROL Registrieren] wird geöffnet.
   1. Geben Sie Ihren Vornamen und Nachnamen, die E-Mail-Adresse und ein Kennwort ein.
   1. Wählen Sie **[!UICONTROL Anmelden]**.<br />
   ![](assets/bplogin_request_access_5.png)

   Sie werden zur Seite [!UICONTROL Zugriff anfordern] weitergeleitet.

1. Auf der nächsten Seite werden der Name des aktuellen Benutzers und die E-Mail-Adresse angezeigt, die zum Anfordern des Zugriffs genutzt werden. Geben Sie einen Kommentar für den Administrator ein und klicken Sie dann auf **[!UICONTROL Übermitteln]**.<br />

   ![](assets/bplogin-request-access.png)

## Produktadministratoren gewähren Zugriff {#grant-access-to-brand-portal}

Produktadministratoren des Markenportals erhalten Zugriffsanfragen in ihrem Markenportal-Benachrichtigungsbereich und per E-Mail in ihrem Posteingang.

![Zugriff auf die angeforderte Benachrichtigungen](assets/bplogin_request_access_7.png)

To grant access, product administrators need to click the relevant notification in Brand Portal notification area and then click **[!UICONTROL Grant Access]**.
Alternatively, product administrators can follow the link provided in the access request email to visit Adobe [!UICONTROL Admin Console] and add the user to the relevant product configuration.

You are redirected to the [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) home page. Use Adobe [!UICONTROL Admin Console] to create users and assign them to product profiles (formerly known as product configurations), which show as groups in Brand Portal. For more information about adding users in [!UICONTROL Admin Console], see [Add a user](brand-portal-adding-users.md#add-a-user) (follow Steps 4-7 in the procedure to add a user).

## Markenportal-Sprachen {#brand-portal-language}

Sie können die Sprache des Markenportals in den Adobe [!UICONTROL Experience Cloud-Einstellungen]ändern.

![Zugriff auf die angeforderte Benachrichtigungen](assets/BPLang.png)

So ändern Sie die Sprache:

1. Wählen Sie [!UICONTROL Benutzer] &gt; Profilbearbeiten aus dem oberen Menü.<br />
   ![Profil bearbeiten](assets/EditBPProfile.png)

1. Wählen Sie auf der Seite [!UICONTROL Experience Cloud-Einstellungen] eine Sprache aus dem Dropdownmenü [!UICONTROL Sprache] .

## Wartungsbenachrichtigung in Brand Portal {#brand-portal-maintenance-notification}

Bevor Brand Portal planmäßig zur Wartung heruntergefahren wird, wird nach dem Anmelden bei Brand Portal eine Benachrichtigung als Banner angezeigt. Beispiel für eine Benachrichtigung:

![](assets/bp_maintenance_notification.png)

Sie können diese Benachrichtigung schließen und Brand Portal weiterhin verwenden. Diese Benachrichtigung erscheint bei jeder neuen Sitzung.

## Versions- und Systeminformationen {#release-and-system-information}

* [Neuerungen](whats-new.md)
* [Versionshinweise](brand-portal-release-notes.md)
* [Unterstützte Dateiformate](brand-portal-supported-formats.md)

## Verwandte Ressourcen {#related-resources}

* [Adobe-Kundendienst](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [AEM-Foren](https://www.adobe.com/go/aod_forums_en)