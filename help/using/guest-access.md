---
title: Gastzugang für Brand Portal
seo-title: Gastzugang für Brand Portal
description: Lassen Sie Gastzugänge zu und speichern Sie diese Einstellung, um zahlreiche Benutzer zu integrieren, die nicht authentifiziert werden müssen.
seo-description: Lassen Sie Gastzugänge zu und speichern Sie diese Einstellung, um zahlreiche Benutzer zu integrieren, die nicht authentifiziert werden müssen.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: mgulati
topic-tags: Einführung
content-type: Referenz
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: 9763a57a83db22cd6686701dcbd8fcde16bcbb31

---


# Gastzugang für Brand Portal {#guest-access-to-brand-portal}

AEM Brand Portal gestattet den Gastzugang für das Portal. Ein Gastbenutzer braucht keine Anmeldeinformationen, um das Portal aufzurufen, und hat Zugriff auf die öffentlichen Assets (und Sammlungen) des Portals. Users in the guest session can add assets to their lightbox (private collection) and download the same until their session lasts, which is 2 hours from the beginning of the session unless the guest user chooses to [[!UICONTROL End Session]](#exit-guest-session).

Die Gastzugangsfunktion bietet Organisationen die Möglichkeit, schnell und skaliert [genehmigte Assets für die gewünschte Zielgruppe freizugeben](../using/brand-portal-sharing-folders.md#how-to-share-folders), ohne dass sie integriert werden müssen. Ab Version 6.4.2 unterstützt Brand Portal mehrere gleichzeitige Gastbenutzer. Die Anzahl entspricht 10 % des Gesamtbenutzerkontingents pro Organisation. Allowing guest access saves time to manage and on-board scores of users who need to use limited functionalities on Brand Portal.\
Organizations can enable (or disable) guest access on Brand Portal account of the organization using **[!UICONTROL Allow Guest Access]** option from **[!UICONTROL Access]** settings in the administrative tools panel.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Starten einer Gastsitzung {#begin-guest-session}

Um Brand Portal anonym aufzurufen, wählen Sie die Option **[!UICONTROL Hier klicken]** neben dem Link **Gastzugang?** im Willkommensbildschirm des Markenportals. Benutzer müssen keinen Zugriff anfordern und warten, bis sie vom Administrator authentifiziert werden, damit sie auf Brand Portal zugreifen können.

![](assets/bp-login-screen.png)

## Dauer der Gastsitzung {#guest-session-duration}

Eine Gastbenutzersitzung bleibt für 2 Stunden aktiv. This means that the state of the [!UICONTROL Lightbox] is preserved until 1 hour from the session start time, and after 2 hours the current guest session restarts so the Lightbox state is lost.\
Ein Gast-Benutzer meldet sich beispielsweise 1500 Stunden beim Markenportal an und fügt Assets zur Lightbox zum Download um 16:50 Uhr hinzu. If the user doesn't download the [!UICONTROL Lightbox] collection (or its assets) before 17:00 hours, the [!UICONTROL Lightbox] will become empty as the user will have to restart the session at the end of 1 hour (that is 1700 hours).

## Gleichzeitige Gastsitzungen zulässig {#concurrent-guest-sessions-allowed}

Die Zahl der gleichzeitigen Gastsitzungen ist auf 10 % des Gesamtbenutzerkontingents pro Organisation beschränkt. Das bedeutet für eine Organisation mit einem Benutzerkontingent von 200, dass maximal 20 Gastbenutzer gleichzeitig arbeiten können. Dem 21. Benutzer wird der Zugriff verweigert und er kann nur als Gast zugreifen, wenn die Sitzung eines der 20 aktiven Gastbenutzer beendet wird.

## Gastbenutzerinteraktion mit Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigation in der Gast-Benutzeroberfläche

On entering the Brand Portal as the guest, users can see all the [assets and folders shared](../using/brand-portal-sharing-folders.md#sharefolders) publicly or with guest users exclusively. Bei dieser Ansicht handelt es sich um die Ansicht „Nur Inhalte“, in der Assets in einem Karten-, Listen- oder Spaltenlayout angezeigt werden.

![](assets/disabled-folder-hierarchy1.png)

However, the guest users see the folder tree (starting from the root folder) and the shared folders arranged within their respective parent folders on logging in to the Brand Portal, if administrators have enabled [Enable Folder Hierarchy](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) configuration.

Diese übergeordneten Ordner sind virtuelle Ordner und für sie können keine Aktionen durchgeführt werden. Sie können diese virtuellen Ordner an einem Schlosssymbol erkennen.

No action tasks are visible on hovering or selecting them in [!UICONTROL Card View], unlike the shared folders. [!UICONTROL Overview] button is shown on selecting a virtual folder in [!UICONTROL Column View] and [!UICONTROL List View].

>[!NOTE]
>
>Beachten Sie, dass das Standardminiaturbild der virtuellen Ordner das Miniaturbild des ersten freigegebenen Ordners ist.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

[!UICONTROL View Settings] option allows the guest users to adjust card sizes in [!UICONTROL Card View] or columns to display in [!UICONTROL List View].

![](assets/nav-guest-user.png)

The [!UICONTROL Content tree] lets you move through assets hierarchy.

![](assets/guest-login-ui.png)

Brand Portal provides [!UICONTROL Overview] option to guest users to view [!UICONTROL Asset Properties] of selected assets/folders. The [!UICONTROL Overview] option is visible:

* In der Symbolleiste am oberen Rand des ausgewählten Assets/Ordners
* In der Dropdown-Liste des ausgewählten Leistenselektors

On selecting the [!UICONTROL Overview] option while an asset/folder is selected, users can see the title, path, and time of asset creation. Whereas, on asset detail page selecting [!UICONTROL Overview] option lets the users see metadata of the asset.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)<br />

Die Option **[!UICONTROL Navigation]** in der linken Seitenschiene ermöglicht die Navigation von Dateien zu Sammlungen und zurück zur Gastsitzung, damit Benutzer durch Assets in Dateien oder Sammlungen navigieren können.

**[!UICONTROL Über die Option Filter]** können Gastbenutzer Asset-Dateien und Ordner nach den vom Administrator festgelegten Sucheigenschaften filtern.

### Funktionen der Gastbenutzer

Gastbenutzer können auf öffentliche Assets in Brand Portal zugreifen, haben jedoch auch einige Einschränkungen, die nachfolgend näher beschrieben werden.

Gastbenutzer können Folgendes tun:

* Auf alle öffentlichen Ordner und Sammlungen, die für sämtliche Brand Portal-Benutzer freigegeben sind, zugreifen
* Mitglieder oder die Detailseite durchsuchen; sie haben eine vollständige Asset-Ansicht der Mitglieder aller öffentlichen Ordner und Sammlungen.
* Assets in allen öffentlichen Ordnern und Sammlungen durchsuchen.
* Assets zur Lightbox-Sammlung hinzufügen. Diese Änderungen an der Sammlung bleiben für die Dauer der Sitzung bestehen.
* Assets direkt oder über die Lightbox-Sammlung herunterladen.

Gastbenutzer können Folgendes nicht tun:

* Sammlungen und gespeicherte Suchen erstellen oder diese weiter freigeben.
* Auf Einstellungen für Ordner und Sammlungen zugreifen.
* Assets als Links freigeben

### Herunterladen von Assets in Gastsitzungen

Gastbenutzer können öffentlich oder ausschließlich für Gastbenutzer freigegebene Assets in Brand Portal herunterladen. Guest users can also add assets to [!UICONTROL Lightbox] (public collection), and download the [!UICONTROL Lightbox] collection before their session expires.

Verwenden Sie zum Herunterladen von Assets und Sammlungen das Symbol „Download“:

* Schnellzugriff-Miniaturansichten, die beim Bewegen des Mauszeigers über das Asset bzw. die Sammlung angezeigt werden
* Die Symbolleiste am oberen Rand, die bei Auswahl des Assets bzw. der Sammlung angezeigt wird

![](assets/download-on-guest.png)

Mit der Option **[!UICONTROL Downloadbeschleunigung aktivieren]**[!UICONTROL  im Dialogfeld „Download“ können Sie die ]Download-Zeit verkürzen[.](../using/accelerated-download.md)

## Beenden einer Gastsitzung {#exit-guest-session}

Beenden Sie die Gastsitzung durch Auswahl von **[!UICONTROL Sitzung beenden]aus den in der Kopfzeile verfügbaren Optionen.** Ist die für die Gastsitzung verwendete Browser-Registerkarte inaktiv, läuft die Sitzung automatisch nach 2 Stunden Inaktivität ab.

![](assets/end-guest-session.png)

## Überwachen von Gastbenutzeraktivitäten {#monitoring-guest-user-activities}

Administratoren können die Gastbenutzerinteraktion mit Brand Portal überwachen. Die in Brand Portal erstellten Berichte können wichtige Einblicke in die Gastbenutzeraktivitäten liefern. So können Sie beispielsweise mithilfe des Berichts **[!UICONTROL Download]die Anzahl an Assets nachverfolgen, die vom Gastbenutzer heruntergeladen wurden.** **[!UICONTROL Der Bericht Benutzeranmeldungen]** kann darüber informieren, wann sich der Gastbenutzer zuletzt im Portal angemeldet hat und wie oft er sich in einer bestimmten Zeit angemeldet hat.
