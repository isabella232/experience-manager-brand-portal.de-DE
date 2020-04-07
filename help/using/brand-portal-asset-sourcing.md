---
title: Asset-Beschaffung in Brand Portal
seo-title: Asset-Beschaffung in Brand Portal
description: Hier erhalten Sie einen Einblick in die Asset-Beschaffungsfunktion, die in Adobe Experience Manager Assets Brand Portal veröffentlicht wurde.
seo-description: Hier erhalten Sie einen Einblick in die Asset-Beschaffungsfunktion, die in Adobe Experience Manager Assets Brand Portal veröffentlicht wurde.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: Assets
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: ca71b51ea51a92f23fc4c7d6682f73c4c204a5f2

---


# Überblick über die Asset-Beschaffung {#overview-asset-sourcing-in-bp}

Mit der **Asset-Beschaffung** können AEM-Benutzer (Administratoren/Benutzer ohne Administratorrechte) neue Ordner mit der zusätzlichen Eigenschaft **Asset-Beitrag** erstellen, um sicherzustellen, dass die neu erstellten Ordner von Brand Portal-Benutzern für die Übermittlung von Assets nutzbar sind. Dadurch wird automatisch ein Workflow ausgelöst, mit dem zwei weitere Unterordner namens **SHARED** und **NEW** im neu erstellten **Beitragsordner** erstellt werden. Der AEM-Administrator definiert dann die Anforderung, indem er eine Kurzbeschreibung der Asset-Typen, die zum Beitragsordner hinzugefügt werden sollen, sowie eine Reihe von Grundlinien-Assets in den Ordner **SHARED** hochlädt, um sicherzustellen, dass Brand Portal-Benutzer über die benötigten Referenzinformationen verfügen. Der Administrator kann aktiven Brand Portal-Benutzern anschließend Zugriff auf den Beitragsordner gewähren, bevor der neu erstellte **Beitragsordner** in Brand Portal veröffentlicht wird. Nachdem die Benutzer Inhalte zum Ordner **NEW** hinzugefügt haben, können sie den Beitragsordner wieder in der AEM-Autorenumgebung veröffentlichen. Bitte beachten Sie, dass es einige Minuten dauern kann, bis der Import abgeschlossen ist und die neu veröffentlichten Inhalte in AEM Assets angezeigt werden.

Darüber hinaus bleiben alle vorhandenen Funktionen unverändert. Brand Portal-Benutzer können Assets aus dem Beitragsordner sowie aus anderen Ordnern anzeigen, suchen und herunterladen, für die sie über entsprechende Berechtigungen verfügen. Administratoren können außerdem den Beitragsordner freigeben, Eigenschaften ändern und Assets zu Sammlungen hinzufügen.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

>[!NOTE]
>
>Die Asset-Beschaffung in Brand Portal wird ab AEM 6.5.2.0 unterstützt.
>
>Die Funktion wird in früheren Versionen – AEM 6.3 und AEM 6.4 – nicht unterstützt.
>
>Wenden Sie sich an den Adobe-Support, um Ihre AEM-Instanz auf die aktuelle unterstützte AEM-Version zu aktualisieren.

![Beschaffung von Brand Portal-Assets](assets/asset-sourcing.png)


>[!NOTE]
>
>Wenn Sie AEM 6.5.4-Benutzer sind, funktioniert die Asset-Sourcing-Funktion weiterhin mit der &quot;Legacy-OAuth-Integration&quot;.
>
>Brand Portal-Benutzer können jedoch keine Beitragsordnerelemente für AEM Assets veröffentlichen, wenn sie auf Adobe I/O auf AEM 6.5.4 aktualisieren.
>
>Dieses Problem wird im nächsten Service Pack AEM 6.5.5 behoben.
>
>Für eine sofortige Fehlerbehebung in AEM 6.5.4 wird empfohlen, den Hotfix [](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) herunterzuladen und auf Ihrer Autoreninstanz zu installieren.


## Voraussetzungen {#prerequisites}

* AEM 6.5.0.2 oder höher.
* Stellen Sie sicher, dass Ihre AEM Assets-Instanz mit Brand Portal konfiguriert ist. Siehe [Konfigurieren von AEM Assets mit Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Siehe auch {#reference-articles}

**Für Administratoren**

* [Konfigurieren der Asset-Beschaffung in AEM](brand-portal-configure-asset-sourcing.md)
* [Hochladen der Brand Portal-Benutzerliste](brand-portal-configure-asset-sourcing.md)
* [Konfigurieren von Beitragsordnern](brand-portal-contribution-folder.md)
* [Hochladen von Grundlinien-Assets in den Beitragsordner](brand-portal-upload-baseline-assets.md)
* [Veröffentlichen von Beitragsordnern in Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Für Brand Portal-Benutzer**

* [Herunterladen von Asset-Anforderungen](brand-portal-download-asset-requirements.md)
* [Hochladen von neuen Assets in den Beitragsordner](brand-portal-upload-assets-to-contribution-folder.md)
* [Veröffentlichen von Beitragsordnern in AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
