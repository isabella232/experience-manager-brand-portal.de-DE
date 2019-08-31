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
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Verwalten allgemeiner Mandantenkonfigurationen {#administer-general-tenant-configurations}

In AEM Assets Brand Portal können Unternehmen die folgenden Funktionen für bestimmte Mandanten konfigurieren:

* das Löschen von Assets durch Administratoren
* die Erstellung öffentlicher Sammlungen von Benutzern ohne Administratorrechte
* die Erstellung öffentlicher Smart-Sammlungen von Benutzern ohne Administratorrechte
* die Downloadbeschleunigung
* Sichtbarkeit der übergeordneten Hierarchie von freigegebenen Ordnern für Benutzer ohne Administratorrechte

These configurations have been provided as **[!UICONTROL General Settings]** configurations on the administrative tools panel.

![](assets/general-configs.png)

**Eine** Konfiguration, damit Administratoren Assets aus dem Brand Portal löschen können. (Die Option ist standardmäßig aktiviert.)

**B** -Konfiguration, damit Benutzer ohne Administratorrechte öffentliche Sammlungen erstellen können. (Die Option ist standardmäßig aktiviert.)

**C** Konfiguration, die es Benutzern ohne Adminstratorrechte gestattet, öffentliche Smart-Sammlungen zu erstellen. (Die Option ist standardmäßig aktiviert.)

**D** -Konfiguration, um die Download-Beschleunigung von Assets zu ermöglichen, die aus dem Portal und aus den freigegebenen Links heruntergeladen wurden. (Die Option ist standardmäßig deaktiviert.)

**E** Konfiguration, die Benutzern ohne Administratorrechte (Bearbeitern, Betrachtern und Gastbenutzern) gestattet, die Ordnerhierarchie (vom Stamm) der freigegebenen Ordner anzuzeigen. (Die Option ist standardmäßig deaktiviert.)

## Aktivieren/Deaktivieren der allgemeinen Konfigurationen {#enable-disable-general-configurations}

So aktivieren/deaktivieren Sie jede dieser Konfigurationen:

1. Melden Sie sich mit Administratorrechten an.
2. Wählen Sie in der Symbolleiste am oberen Rand das AEM-Logo aus, um die Admin Tools aufzurufen.
3. From the administrative tools panel, select **[!UICONTROL General]** to open the **[!UICONTROL General Settings]** page.
4. Verwenden Sie den entsprechenden Umschalter, um allgemeine Konfigurationen zu aktivieren/deaktivieren.
5. **[!UICONTROL Speichern Sie die Änderungen.]**
6. Melden Sie sich ab, um die Änderungen zu übernehmen.

## Löschen von Assets in Brand Portal durch Administratoren zulassen {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Erlauben Sie Benutzern,]** die Konfiguration zu aktivieren, damit Unternehmen Benutzer mit Administratorrechten zulassen (oder einschränken) können, Assets und Ordner aus dem Brand Portal zu löschen.

## Zulassen der Erstellung öffentlicher Sammlungen durch Benutzer ohne Administratorrechte {#allow-public-collections-creation-by-non-admins}

[[! UICONTROL Zulassen der Erstellung öffentlicher Sammlungen]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) Konfigurationen steuern, ob nicht-Administratoren öffentliche Sammlungen im Brand Portal erstellen können. Die Konfiguration ist standardmäßig aktiviert. Unternehmen können die Konfiguration deaktivieren, um zu verhindern, dass sich in ihrem Portal zahlreiche öffentliche Sammlungen befinden. Auf diese Weise wird Systemspeicherplatz eingespart.

## Zulassen der Erstellung öffentlicher Smart-Sammlungen durch Benutzer ohne Administratorrechte {#allow-public-smart-collections-creation-by-non-admins}

[[! UICONTROL Zulassen der Erstellung öffentlicher intelligenter Sammlungen]](../using/brand-portal-searching.md#main-pars-header-500620467) Konfiguration steuert, ob nicht-Administratoren ihre Suchvorgänge als intelligente Sammlungen speichern und für diesen Mandant öffentlich machen können. Die Konfiguration ist standardmäßig aktiviert. Unternehmen können die Konfiguration deaktivieren, um zu verhindern, dass Benutzer ohne Administratorrechte eine große Anzahl öffentlicher Smart-Sammlungen im Portal der Organisation erstellen.

## Downloadbeschleunigung aktivieren {#allow-download-acceleration}

[[! UICONTROL Allow Download Acceleration]](../using/accelerated-download.md) Konfiguration ermöglicht es Unternehmen, beschleunigte Downloads von Assets aus Markenportal und freigegebenen Links zuzulassen, indem sie eine Integration in IBM Aspera Connect durchführen, die eine Installationsanwendung ist. Die Anwendung nutzt proprietäre Technologie, um TCP-Overheads zu verhindern.

## Ordnerhierarchie aktivieren {#enable-folder-hierarchy}

[[! UICONTROL Enable Folder-Hierarchiekonfiguration ermöglicht](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) die Konfiguration der Administratoren steuern, wie die Nicht-Admin-Benutzer (Editors, Viewer und Gastbenutzer) die freigegebenen Ordner nach der Anmeldung sehen.
