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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Gastzugang für Brand Portal {#guest-access-to-brand-portal}

[!DNL AEM Brand portal] ermöglicht den Gastzugriff auf das Portal. Ein Gastbenutzer braucht keine Anmeldeinformationen, um das Portal aufzurufen, und hat Zugriff auf die öffentlichen Assets (und Sammlungen) des Portals. Users in the guest session can add assets to their lightbox (private collection) and download the same until their session lasts, which is 2 hours from the beginning of the session unless the guest user chooses to [End Session](#exit-guest-session).

Guest access functionality enables organizations to [quickly share approved assets](../using/brand-portal-sharing-folders.md#how-to-share-folders) with the intended audience at scale without having to onboard them. [!DNL Brand Portal]Ab Version 6.4.2 unterstützt mehrere gleichzeitige Gastbenutzer. Die Anzahl entspricht 10 % des Gesamtbenutzerkontingents pro Organisation. Allowing guest access saves time to manage and on-board scores of users who need to use limited functionalities on [!DNL Brand Portal].\
Organisationen können über die Option "Gastzugriff [!DNL Brand Portal]**zulassen" über die Option" Gastzugriff** zulassen" im **Bereich "Zugriffsrechte** " den Gastzugriff auf die Organisation aktivieren (oder deaktivieren).

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Starten einer Gastsitzung {#begin-guest-session}

Um Brand Portal anonym aufzurufen, wählen Sie die Option **[!UICONTROL Hier klicken]** aus, die dem Link **Gastzugang?** auf dem [!DNL Brand Portal] Startbildschirm. Users need not seek access and wait for the administrator to authenticate them to grant access to use the [!DNL Brand Portal].

![](assets/bp-login-screen.png)

## Dauer der Gastsitzung {#guest-session-duration}

Eine Gastbenutzersitzung bleibt für 2 Stunden aktiv. This means that the state of the [!UICONTROL lightbox] is preserved until 1 hour from the session start time, and after 2 hours the current guest session restarts so the lightbox state is lost.\
For example, a guest user logs in to the [!DNL Brand Portal] at 1500 hours and adds assets to lightbox for download at 16:50 hours. If the user doesn't download the [!UICONTROL lightbox collection] (or its assets) before 17:00 hours, the [!UICONTROL lightbox] will become empty as the user will have to restart the session at the end of 1 hour (that is 1700 hours).

## Gleichzeitige Gastsitzungen zulässig {#concurrent-guest-sessions-allowed}

Die Anzahl gleichzeitiger Gastsitzungen ist auf 10% der Gesamtbenutzerquoten pro Organisation beschränkt. Dies bedeutet, dass für eine Organisation mit Benutzerkontingent von 200 maximal 20 Gäste gleichzeitig arbeiten können. Dem 21. Benutzer wird der Zugriff verweigert und er kann nur als Gast zugreifen, wenn die Sitzung einer der 20 aktiven Gäste beendet wird.

## Gastbenutzerinteraktion mit Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigation in der Gast-Benutzeroberfläche

On entering the [!DNL Brand Portal] as the guest, users are able to see all the [assets and folders shared](../using/brand-portal-sharing-folders.md#sharefolders) publicly or with guest users exclusively. Bei dieser Ansicht handelt es sich um die Ansicht „Nur Inhalte“, in der Assets in einem Karten-, Listen- oder Spaltenlayout angezeigt werden.

![](assets/disabled-folder-hierarchy1.png)

However, Guest Users see the folder tree (starting from the root folder) and the shared folders arranged within their respective parent folders on logging in to the [!DNL Brand Portal], if administrators have enabled [Enable Folder Hierarchy](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) configuration.

Diese übergeordneten Ordner sind virtuelle Ordner und für sie können keine Aktionen durchgeführt werden. Sie können diese virtuellen Ordner an einem Schlosssymbol erkennen.

Im Gegensatz zu freigegebenen Ordnern sind keine Aktionsaufgaben zu sehen, wenn Sie den Mauszeiger auf die Ordner bewegen oder sie in der Kartenansicht auswählen. Die Schaltfläche „Überblick“ wird angezeigt, wenn Sie einen virtuellen Ordner in der Spaltenansicht und Listenansicht auswählen.

>[!NOTE]
>
>Beachten Sie, dass das Standardminiaturbild der virtuellen Ordner das Miniaturbild des ersten freigegebenen Ordners ist.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

Über die Option Anzeigeeinstellungen können die Gastbenutzer die Kartengrößen in der Kartenansicht oder die in der Listenansicht anzuzeigenden Spalten festlegen.

![](assets/nav-guest-user.png)

Mit der Inhaltsstruktur können Sie die Asset-Hierarchie durchlaufen.

![](assets/guest-login-ui.png)

[!DNL Brand Portal] bietet **Übersichtsoption** für Gäste, um Asset-Eigenschaften der ausgewählten Assets/Ordner anzuzeigen. Die Option „Überblick“ finden Sie an folgenden Stellen:

1. In der Symbolleiste am oberen Rand des ausgewählten Assets/Ordners
2. in der Dropdown-Liste des ausgewählten Leistenselektors

Bei Auswahl der Option „Überblick“ bei ausgewähltem Asset/Ordner können die Benutzer den Titel, den Pfad und den Zeitpunkt der Asset-Erstellung sehen. Wohingegen die Benutzer bei Auswahl der Option „Überblick“ auf der Asset-Detailseite die Metadaten des Assets sehen können.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL Die Navigationsoption]** in der linken Leiste ermöglicht das Navigieren von Dateien zu [!UICONTROL Sammlungen] und zurück in der Gastsitzung, damit Benutzer Assets in Dateien oder [!UICONTROL Sammlungen durchsuchen]können.

**Mit** der Filteroption können Gastbenutzer Asset-Dateien und -ordner mithilfe von vom Administrator festgelegten Suchvorhersagen filtern.

### Funktionen der Gastbenutzer

Guest users can access public assets on [!DNL Brand Portal], and also have few restrictions as discussed further.

Gastbenutzer können Folgendes tun:

* access all the public folders and [!UICONTROL collections] meant for all the [!DNL Brand Portal] users.
* browse members, detail page, and have full asset view of the members of all the public folders and [!UICONTROL collections].
* search assets across public folders and [!UICONTROL collections].
* add assets to lightbox [!UICONTROL collection]. These changes to the [!UICONTROL collection] persist during the session.
* download assets directly or through lightbox [!UICONTROL collection].

Gastbenutzer können Folgendes nicht tun:

* [!UICONTROL Sammlungen] und gespeicherte Suchen erstellen oder sie weiter freigeben.
* access folder and [!UICONTROL collections] settings.
* Assets als Links freigeben

### Herunterladen von Assets in Gastsitzungen

Guest users can directly download assets shared publically or exclusively with guest users on [!DNL Brand Portal]. Guest users can also add assets to [!UICONTROL Lightbox] (public [!UICONTROL collection]), and download the [!UICONTROL lightbox collection] before their session expires.

To download assets and [!UICONTROL collections], use the download icon from:

* quick action thumbnails, which appear on hovering over the asset or [!UICONTROL collection]
* the toolbar at the top, which appears on selecting the asset or [!UICONTROL collection]

![](assets/download-on-guest.png)

Mit der Option **Downloadbeschleunigung aktivieren** im Dialogfeld „Download“ können Sie die [Download-Zeit verkürzen](../using/accelerated-download.md).

## Beenden einer Gastsitzung {#exit-guest-session}

To exit a guest session, use **End Session** from the options available in the header. Wenn jedoch die für die Gastsitzung verwendete Browserregisterkarte inaktiv ist, läuft die Sitzung nach zwei Stunden Inaktivität automatisch ab.

![](assets/end-guest-session.png)

## Überwachen von Gastbenutzeraktivitäten {#monitoring-guest-user-activities}

Administrators can monitor guest user interaction with the [!DNL Brand Portal]. Reports generated in [!DNL Brand Portal] can provide key insights into guest user activities. So können Sie beispielsweise mithilfe des Berichts **Download** die Anzahl an Assets nachverfolgen, die vom Gastbenutzer heruntergeladen wurden. **Der** Bericht zu Benutzeranmeldungen kann darüber informiert werden, wann der Gastbenutzer zuletzt beim Portal angemeldet ist und die Häufigkeit der Anmeldungen in einer festgelegten Dauer.
