---
title: Verwalten allgemeiner Mandantenkonfigurationen
seo-title: Verwalten allgemeiner Mandantenkonfigurationen
description: Konfigurieren Sie Download-Beschleunigung, öffentliches Smart [! UICONTROL Collection] create, public [! UICONTROL-Sammlung] erstellen und Administratoren ermöglichen, Assets auf Mandanten zu löschen.
seo-description: Konfigurieren Sie Download-Beschleunigung, öffentliches Smart [! UICONTROL Collection] create, public [! UICONTROL-Sammlung] erstellen und Administratoren ermöglichen, Assets auf Mandanten zu löschen.
uuid: 3 c 46 cd 7 c-c 38 b -4 bc 7-b 566-93 f 977 bc 8227
contentOwner: mgulati
topic-tags: Administration
content-type: Referenz
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: f 4 c 237 bc-f 6 a 4-4 bc 4-af 56-3 d 9 c 3027 daf 4
translation-type: tm+mt
source-git-commit: ea7fdd2df0696ed309227fa77e3f79d0141bcb58

---


# Verwalten allgemeiner Mandantenkonfigurationen {#administer-general-tenant-configurations}

[!DNL AEM] Mit Assets [!DNL Brand Portal] können Unternehmen die folgenden Funktionen für bestimmte Mandanten konfigurieren:

* das Löschen von Assets durch Administratoren
* Public [!UICONTROL collection] creation by non-admin users
* Public smart [!UICONTROL collection] creation by non-admin users
* die Downloadbeschleunigung
* Sichtbarkeit der übergeordneten Hierarchie von freigegebenen Ordnern für Benutzer ohne Administratorrechte

These configurations have been provided as **General Settings** configurations on the administrative tools panel.

![](assets/general-configs.png)

**Eine** Konfiguration, über die Administratoren Assets löschen [!DNL Brand Portal]können. (Die Option ist standardmäßig aktiviert.)

**B** -Konfiguration, damit Benutzer ohne Administratorrechte öffentliche [!UICONTROL Sammlungen erstellen]können. (Standardeinstellung ist aktiviert)

**C** -Konfiguration, damit Benutzer ohne Administratorrechte öffentliche intelligente [!UICONTROL Sammlungen erstellen]können. (Standardeinstellung ist aktiviert)

**D** -Konfiguration, um die Download-Beschleunigung von Assets zu ermöglichen, die aus dem Portal und aus den freigegebenen Links heruntergeladen wurden. (Die Option ist standardmäßig deaktiviert.)

**E** Konfiguration, die Benutzern ohne Administratorrechte (Bearbeitern, Betrachtern und Gastbenutzern) gestattet, die Ordnerhierarchie (vom Stamm) der freigegebenen Ordner anzuzeigen. (Die Option ist standardmäßig deaktiviert.)

## Aktivieren/Deaktivieren der allgemeinen Konfigurationen {#enable-disable-general-configurations}

So aktivieren/deaktivieren Sie jede dieser Konfigurationen:

1. Melden Sie sich mit Administratorrechten an.
2. Select the [!DNL AEM] logo to access administrative tools, from the toolbar at the top.
3. From the administrative tools panel, select **General** to open the **General Settings** page.
4. Verwenden Sie den entsprechenden Umschalter, um allgemeine Konfigurationen zu aktivieren/deaktivieren.
5. **Speichern Sie die Änderungen.**
6. Melden Sie sich ab, um die Änderungen zu übernehmen.

## Allow admin users to delete assets from [!DNL Brand Portal] {#allow-admin-users-to-delete-assets-from-brand-portal}

**Ermöglichen Sie Benutzern,** die Konfiguration zu löschen, können Unternehmen Benutzer mit Administratorrechten zulassen (oder beschränken), um Assets und Ordner zu löschen [!DNL Brand Portal].

## Zulassen der Erstellung öffentlicher Sammlungen durch Benutzer ohne Administratorrechte {#allow-public-collections-creation-by-non-admins}

[Erstellen Sie die Erstellung öffentlicher [!UICONTROL Sammlungen]] (../using/brand-portal-share-[!UICONTROL collection]. md # main-pars-text -1915052376) Konfigurationssteuert, ob nicht-Administratoren öffentliche [!UICONTROL Sammlungen]erstellen können [!DNL Brand Portal]. Die Konfiguration ist standardmäßig aktiviert. By disabling the configuration organizations can prevent having numerous public [!UICONTROL collection]s on their portal so that system space can be saved.

## Zulassen der Erstellung öffentlicher Smart-Sammlungen durch Benutzer ohne Administratorrechte {#allow-public-smart-collections-creation-by-non-admins}

[Aktivieren Sie die Konfiguration](../using/brand-portal-searching.md#main-pars-header-500620467) öffentlicher intelligenter Sammlungen, unabhängig davon, ob nicht-Administratoren ihre Suchvorgänge als intelligente [!UICONTROL Sammlungen speichern] und für diesen Mandanten öffentlich machen können. Die Konfiguration ist standardmäßig aktiviert. By disabling the configuration organizations can prevent having a huge number of public smart [!UICONTROL collections] created by non-admin users on organization's [!DNL Brand Portal].

## Downloadbeschleunigung aktivieren {#allow-download-acceleration}

Mit der Konfiguration [Downloadbeschleunigung aktivieren](../using/accelerated-download.md)[!DNL Brand Portal] können Unternehmen den beschleunigten Download von Assets aus und über freigegebene Links gestatten. Dies geschieht durch die Integration mit der Anwendung IBM Aspera Connect, die bei Bedarf installiert wird. Die Anwendung nutzt proprietäre Technologie, um TCP-Overheads zu verhindern.

## Ordnerhierarchie aktivieren {#enable-folder-hierarchy}

Mit der Konfiguration [Ordnerhierarchie aktivieren](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) können Administratoren steuern, wie Benutzer ohne Administratorrechte (Bearbeiter, Betrachter und Gastbenutzer) die freigegebenen Ordner nach der Anmeldung sehen.
