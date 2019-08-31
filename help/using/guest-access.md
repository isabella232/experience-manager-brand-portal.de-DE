---
title: Gastzugang für Brand Portal
seo-title: Gastzugang für Brand Portal
description: Lassen Sie Gastzugänge zu und speichern Sie diese Einstellung, um zahlreiche Benutzer zu integrieren, die nicht authentifiziert werden müssen.
seo-description: Lassen Sie Gastzugänge zu und speichern Sie diese Einstellung, um zahlreiche Benutzer zu integrieren, die nicht authentifiziert werden müssen.
uuid: edb 3378 d -1710-44 a 2-97 a 6-594 d 99 f 62 fff
contentOwner: mgulati
topic-tags: Einführung
content-type: Referenz
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: b 9 e 9 fe 7 b -0373-42 d 1-851 b -7 c 76 b 47657 c 2
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Gastzugang für Brand Portal {#guest-access-to-brand-portal}

AEM Brand Portal gestattet den Gastzugang für das Portal. Ein Gastbenutzer braucht keine Anmeldeinformationen, um das Portal aufzurufen, und hat Zugriff auf die öffentlichen Assets (und Sammlungen) des Portals. Users in the guest session can add assets to their lightbox (private collection) and download the same until their session lasts, which is 2 hours from the beginning of the session unless the guest user chooses to [[!UICONTROL End Session]](#exit-guest-session).

Guest access functionality enables organizations to [quickly share approved assets](../using/brand-portal-sharing-folders.md#how-to-share-folders) with the intended audience at scale without having to onboard them. Ab Version 6.4.2 unterstützt Brand Portal mehrere gleichzeitige Gastbenutzer. Die Anzahl entspricht 10 % des Gesamtbenutzerkontingents pro Organisation. Durch Zulassen des Gastzugriffs sparen Sie Zeit zur Verwaltung und Onlineauswertung von Benutzern, die eingeschränkte Funktionen im Brand Portal verwenden müssen.\
Organisationen können Gastzugriff auf das Markenportal-Konto des Unternehmens aktivieren (oder deaktivieren), indem **[!UICONTROL Sie die Option Gastzugriff]** zulassen aus **[!UICONTROL den Zugriffseinstellungen]** im Bereich für die Verwaltung der Verwaltungswerkzeuge verwenden.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Starten einer Gastsitzung {#begin-guest-session}

Um Brand Portal anonym aufzurufen, wählen Sie die Option **[!UICONTROL Hier klicken]** aus, die dem Link **Gastzugang?** auf dem Marken-Portal-Startbildschirm. Benutzer müssen keinen Zugriff anfordern und warten, bis sie vom Administrator authentifiziert werden, damit sie auf Brand Portal zugreifen können.

![](assets/bp-login-screen.png)

## Dauer der Gastsitzung {#guest-session-duration}

Eine Gastbenutzersitzung bleibt für 2 Stunden aktiv. This means that the state of the [!UICONTROL Lightbox] is preserved until 1 hour from the session start time, and after 2 hours the current guest session restarts so the Lightbox state is lost.\
Ein Gastbenutzer meldet sich beispielsweise beim Brand Portal mit 1500 Stunden an und fügt Lightbox zum Download um 16:50 Stunden hinzu. If the user doesn't download the [!UICONTROL Lightbox] collection (or its assets) before 17:00 hours, the [!UICONTROL Lightbox] will become empty as the user will have to restart the session at the end of 1 hour (that is 1700 hours).

## Gleichzeitige Gastsitzungen zulässig {#concurrent-guest-sessions-allowed}

Die Anzahl gleichzeitiger Gastsitzungen ist auf 10% der Gesamtbenutzerquoten pro Organisation beschränkt. Dies bedeutet, dass für eine Organisation mit Benutzerkontingent von 200 maximal 20 Gäste gleichzeitig arbeiten können. Dem 21. Benutzer wird der Zugriff verweigert und er kann nur als Gast zugreifen, wenn die Sitzung einer der 20 aktiven Gastbenutzer endet.

## Gastbenutzerinteraktion mit Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigation in der Gast-Benutzeroberfläche

On entering the Brand Portal as the guest, users can see all the [assets and folders shared](../using/brand-portal-sharing-folders.md#sharefolders) publicly or with guest users exclusively. Bei dieser Ansicht handelt es sich um die Ansicht „Nur Inhalte“, in der Assets in einem Karten-, Listen- oder Spaltenlayout angezeigt werden.

![](assets/disabled-folder-hierarchy1.png)

However, the guest users see the folder tree (starting from the root folder) and the shared folders arranged within their respective parent folders on logging in to the Brand Portal, if administrators have enabled [Enable Folder Hierarchy](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) configuration.

Diese übergeordneten Ordner sind virtuelle Ordner und für sie können keine Aktionen durchgeführt werden. Sie können diese virtuellen Ordner an einem Schlosssymbol erkennen.

No action tasks are visible on hovering or selecting them in [!UICONTROL Card View], unlike the shared folders. [!UICONTROL Die Schaltfläche "Übersicht] " wird angezeigt, wenn Sie einen virtuellen Ordner in der [!UICONTROL Spaltenansicht] und Listenansicht [!UICONTROL auswählen].

>[!NOTE]
>
>Beachten Sie, dass das Standardminiaturbild der virtuellen Ordner das Miniaturbild des ersten freigegebenen Ordners ist.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

[!UICONTROL Mit der Option "Einstellungen] anzeigen" können die Gastbenutzer Kartengrößen in der [!UICONTROL Kartenansicht] oder in Spalten anpassen, die in [!UICONTROL der Listenansicht angezeigt]werden.

![](assets/nav-guest-user.png)

The [!UICONTROL Content tree] lets you move through assets hierarchy.

![](assets/guest-login-ui.png)

Brand Portal provides [!UICONTROL Overview] option to guest users to view [!UICONTROL Asset Properties] of selected assets/folders. The [!UICONTROL Overview] option is visible:

* In der Symbolleiste am oberen Rand des ausgewählten Assets/Ordners
* in der Dropdown-Liste des ausgewählten Leistenselektors

On selecting the [!UICONTROL Overview] option while an asset/folder is selected, users can see the title, path, and time of asset creation. Whereas, on asset detail page selecting [!UICONTROL Overview] option lets the users see metadata of the asset.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL Die Navigationsoption]** in der linken Leiste ermöglicht das Navigieren von Dateien zu Sammlungen und zurück in der Gastsitzung, damit Benutzer Assets in Dateien oder Sammlungen durchsuchen können.

**[!UICONTROL Mit]** der Filteroption können Gastbenutzer Asset-Dateien und -ordner mithilfe von vom Administrator festgelegten Suchvorhersagen filtern.

### Funktionen der Gastbenutzer

Gastbenutzer können auf öffentliche Assets in Brand Portal zugreifen, haben jedoch auch einige Einschränkungen, die nachfolgend näher beschrieben werden.

Gastbenutzer können Folgendes tun:

* Auf alle öffentlichen Ordner und Sammlungen, die für sämtliche Brand Portal-Benutzer freigegeben sind, zugreifen
* Mitglieder und die Detailseite durchsuchen und alle Assets der Mitglieder sämtlicher öffentlicher Ordner und Sammlungen anzeigen
* Assets in allen öffentlichen Ordnern und Sammlungen durchsuchen
* Assets zur Lightbox-Sammlung hinzufügen Diese Änderungen an der Sammlung bleiben für die Dauer der Sitzung bestehen.
* Assets direkt oder über die Lightbox-Sammlung herunterladen

Gastbenutzer können Folgendes nicht tun:

* Sammlungen und gespeicherte Suchen erstellen oder diese weiter freigeben
* Auf Einstellungen für Ordner und Sammlungen zugreifen
* Assets als Links freigeben

### Herunterladen von Assets in Gastsitzungen

Gastbenutzer können öffentlich oder ausschließlich für Gastbenutzer freigegebene Assets in Brand Portal herunterladen. Guest users can also add assets to [!UICONTROL Lightbox] (public collection), and download the [!UICONTROL Lightbox] collection before their session expires.

Verwenden Sie zum Herunterladen von Assets und Sammlungen das „Download“-Symbol der:

* Miniaturansichten von Aktionen, die beim Mausfahren über das Asset oder die Sammlung angezeigt werden
* die Symbolleiste oben, die beim Auswählen des Assets oder der Sammlung angezeigt wird

![](assets/download-on-guest.png)

Mit der Option **[!UICONTROL Downloadbeschleunigung aktivieren]**[!UICONTROL  im Dialogfeld „Download“ können Sie die ]Download-Zeit verkürzen[.](../using/accelerated-download.md)

## Beenden einer Gastsitzung {#exit-guest-session}

To exit a guest session, use **[!UICONTROL End Session]** from the options available in the header. Wenn jedoch die für die Gastsitzung verwendete Browserregisterkarte inaktiv ist, läuft die Sitzung nach zwei Stunden Inaktivität automatisch ab.

![](assets/end-guest-session.png)

## Überwachen von Gastbenutzeraktivitäten {#monitoring-guest-user-activities}

Administratoren können die Gastbenutzerinteraktion mit Brand Portal überwachen. Die in Brand Portal erstellten Berichte können wichtige Einblicke in die Gastbenutzeraktivitäten liefern. So können Sie beispielsweise mithilfe des Berichts **[!UICONTROL Download]die Anzahl an Assets nachverfolgen, die vom Gastbenutzer heruntergeladen wurden.** **[!UICONTROL Der]** Bericht zu Benutzeranmeldungen kann darüber informiert werden, wann der Gastbenutzer zuletzt beim Portal angemeldet ist und die Häufigkeit der Anmeldungen in einer festgelegten Dauer.
