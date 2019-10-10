---
title: Asset-Beschaffung im Markenportal
seo-title: Asset-Beschaffung im Markenportal
description: Hier erhalten Sie einen Einblick in die Asset-Sourcing-Funktion, die im Adobe Experience Manager Assets Brand Portal veröffentlicht wurde.
seo-description: Hier erhalten Sie einen Einblick in die Asset-Sourcing-Funktion, die im Adobe Experience Manager Assets Brand Portal veröffentlicht wurde.
uuid: null
content-type: Referenz
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Übersicht über die Asset-Beschaffung {#overview-asset-sourcing-in-bp}

**Mit der Asset-Beschaffung** können AEM-Benutzer (Administratoren/Nicht-Admin-Benutzer) neue Ordner mit einer zusätzlichen **Asset Contribution** -Eigenschaft erstellen, um sicherzustellen, dass der neue Ordner für die Asset-Übermittlung durch Brand Portal-Benutzer geöffnet ist. Dadurch wird automatisch ein Workflow ausgelöst, der zwei weitere Unterordner im neu erstellten Ordner " **Contribution** "erstellt, die als **SHARED** und **NEW** bezeichnet werden. Der AEM-Administrator definiert die Anforderung dann, indem er eine kurze Beschreibung der Asset-Typen, die dem Beitragsordner hinzugefügt werden sollen, sowie eine Reihe von Basiselementen in den **SHARED** -Ordner hochlädt, um sicherzustellen, dass BP-Benutzer über die benötigten Referenzinformationen verfügen. Der Administrator kann Benutzern des aktiven Markenportals dann Zugriff auf den Beitragsordner gewähren, bevor der neu erstellte **Beitragsordner** im Markenportal veröffentlicht wird. Nachdem der Benutzer den Inhalt im Ordner " **NEW** "hinzugefügt hat, kann er den Beitragsordner wieder in der AEM-Autorenumgebung veröffentlichen. Bitte beachten Sie, dass es einige Minuten dauern kann, bis der Import abgeschlossen ist und die neu veröffentlichten Inhalte in AEM Assets wiedergegeben werden.

Darüber hinaus bleiben alle vorhandenen Funktionen unverändert. Markenportal-Benutzer können Assets aus dem Beitragsordner sowie aus anderen zulässigen Ordnern anzeigen, suchen und herunterladen. Administratoren können außerdem den Beitragsordner freigeben, Eigenschaften ändern und Assets zu Sammlungen hinzufügen.

>[!NOTE]
>
>Die Asset-Beschaffung im Markenportal wird auf AEM 6.5.2.0 und höher unterstützt.
>
>Die Funktion wird in früheren Versionen - AEM 6.3 und AEM 6.4 - nicht unterstützt.
>
>Wenden Sie sich an den Adobe-Support, um Ihre AEM-Instanz auf die neueste unterstützte AEM-Version zu aktualisieren.

![](assets/asset-sourcing.png)

## Siehe auch {#reference-articles}

**Für Administratoren**
* [Asset-Sourcing in AEM konfigurieren](brand-portal-enable-asset-sourcing.md)
* [Liste der Markenportal-Benutzer hochladen](brand-portal-upload-user-list.md)
* [Beitragsordner konfigurieren](brand-portal-contribution-folder.md)
* [Hochladen von Grundlagenelementen in den Beitragsordner](brand-portal-upload-baseline-assets.md)
* [Veröffentlichen des Beitragsordners im Markenportal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Für Benutzer des Markenportals**
* [Asset-Anforderungen herunterladen](brand-portal-download-asset-requirements.md)
* [Neue Assets in den Beitragsordner hochladen](brand-portal-upload-assets-to-contribution-folder.md)
* [Veröffentlichen des Beitragsordners in AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
