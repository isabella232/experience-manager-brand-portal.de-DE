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
source-git-commit: 5a61c42762e111b824163ce7d054d413a4da56bc
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 62%

---


# Überblick über die Asset-Beschaffung {#overview-asset-sourcing-in-bp}

Mit der **Asset-Beschaffung** können AEM-Benutzer (Administratoren/Benutzer ohne Administratorrechte) neue Ordner mit der zusätzlichen Eigenschaft **Asset-Beitrag** erstellen, um sicherzustellen, dass die neu erstellten Ordner von Brand Portal-Benutzern für die Übermittlung von Assets nutzbar sind. Dadurch wird automatisch ein Workflow ausgelöst, mit dem zwei weitere Unterordner namens **SHARED** und **NEW** im neu erstellten **Beitragsordner** erstellt werden. Der AEM-Administrator definiert dann die Anforderung, indem er eine Kurzbeschreibung der Asset-Typen, die zum Beitragsordner hinzugefügt werden sollen, sowie eine Reihe von Grundlinien-Assets in den Ordner **SHARED** hochlädt, um sicherzustellen, dass Brand Portal-Benutzer über die benötigten Referenzinformationen verfügen. Der Administrator kann aktiven Brand Portal-Benutzern anschließend Zugriff auf den Beitragsordner gewähren, bevor der neu erstellte **Beitragsordner** in Brand Portal veröffentlicht wird. Nachdem die Benutzer Inhalte zum Ordner **NEU** hinzugefügt haben, können sie den Beitragsordner wieder in der AEM-Autorenumgebung veröffentlichen. Bitte beachten Sie, dass es einige Minuten dauern kann, bis der Import abgeschlossen ist und die neu veröffentlichten Inhalte in AEM Assets angezeigt werden.

Darüber hinaus bleiben alle vorhandenen Funktionen unverändert. Brand Portal-Benutzer können Assets aus dem Beitragsordner sowie aus anderen Ordnern anzeigen, suchen und herunterladen, für die sie über entsprechende Berechtigungen verfügen. Administratoren können außerdem den Beitragsordner freigeben, Eigenschaften ändern und Assets zu Sammlungen hinzufügen.

## Voraussetzungen {#prerequisites}

* AEM Assets als Cloud Service-Instanz, AEM Assets 6.5.2 oder höher.
* Stellen Sie sicher, dass Ihre AEM Assets-Instanz mit Brand Portal konfiguriert ist. Siehe [Konfigurieren von AEM Assets mit Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Stellen Sie sicher, dass Ihr Brand Portal-Mandant mit einer AEM Assets-Autoreninstanz konfiguriert ist.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Asset-Beschaffung in Brand Portal](assets/asset-sourcing.png)


>[!NOTE]
>
>Es gibt ein bekanntes Problem in AEM Assets 6.5.4. Markenportal-Benutzer können die Assets des Beitragsordners bei einem Upgrade auf die Adobe Developer Console nicht auf AEM Assets veröffentlichen.
>
>Das Problem wurde in AEM 6.5.5 behoben. Sie können Ihre AEM Assets-Instanz auf das neueste Service Pack AEM 6.5.5 aktualisieren und Ihre Konfigurationen [in Adobe Developer Console](https://docs.adobe.com/content/help/de-DE/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.translate.html#upgrade-integration-65) aktualisieren.
>
>Zur sofortigen Fehlerbehebung unter AEM 6.5.4 wird empfohlen, [den Hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) herunterzuladen und auf der Autoreninstanz zu installieren.

## Konfigurieren der Asset-Beschaffung {#configure-asset-sourcing}

**Asset** Sourcingkonfiguration erfolgt über die AEM Assets-Autoreninstanz. Die Administratoren können die Konfiguration des Asset Sourcing-Feature-Flag über die AEM **Web-Konsolenkonfiguration** aktivieren und die aktive Markenportal-Liste unter **AEM Assets** hochladen.

>[!NOTE]
>
>Die Asset-Beschaffung ist auf AEM Assets als Cloud Service standardmäßig aktiviert. Der AEM-Administrator kann die aktiven Markenportal-Benutzer direkt hochladen, um ihnen den Zugriff auf die Asset-Sourcing-Funktion zu ermöglichen.

>[!NOTE]
>
>Bevor Sie mit der Konfiguration beginnen, stellen Sie sicher, dass Ihre AEM Assets-Instanz in Brand Portal konfiguriert ist. Siehe [Konfigurieren von AEM Assets mit Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

Das folgende Video zeigt, wie Sie die Asset-Beschaffung in Ihrer AEM Assets-Autoreninstanz konfigurieren:

>[!VIDEO](https://video.tv.adobe.com/v/29771)

### Aktivieren der Asset-Beschaffung {#enable-asset-sourcing}

AEM Administratoren können das Flag für die Asset-Sourcing-Funktion in der AEM Web-Konsolenkonfiguration (auch Configuration Manager genannt) aktivieren.

>[!NOTE]
>
>Dieser Schritt gilt nicht für AEM Assets als Cloud Service.


**Aktivieren der Asset-Beschaffung:**
1. Melden Sie sich bei Ihrer AEM Assets-Autoreninstanz an und öffnen Sie Configuration Manager.
Standard-URL: http:// localhost:4502/system/console/configMgr.
1. Suchen Sie mithilfe des Suchbegriffs **Asset Sourcing**, um **[!UICONTROL Konfiguration der Asset-Sourcing-Funktion]** zu finden.
1. Klicken Sie auf **[!UICONTROL Konfiguration der Asset-Sourcing-Funktion]**, um das Konfigurationsfenster zu öffnen.
1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL feature.flag.active.status]**.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/enable-asset-sourcing.png)

### Hochladen der Brand Portal-Benutzerliste {#upload-bp-user-list}

AEM-Administratoren können die Datei für die Brand Portal-Benutzerkonfiguration (.csv) hochladen, die eine Liste der aktiven Brand Portal-Benutzer in AEM Assets enthält. Ein Beitragsordner kann nur für die aktiven Brand Portal-Benutzer freigegeben werden, die in der Benutzerliste definiert sind. Der Administrator kann der Konfigurationsdatei auch neue Benutzer hinzufügen und die geänderte Liste hochladen.

>[!NOTE]
>
>Das Format der CSV-Datei entspricht dem Format, das in der Admin Console für den Massenimport von Benutzern unterstützt wird. E-Mail-Adresse, Vorname und Nachname sind obligatorisch.

Die Administratoren können neue Benutzer in AEM Admin Console hinzufügen. Detaillierte Informationen finden Sie unter [Benutzer verwalten](brand-portal-adding-users.md). Nachdem Benutzer in Admin Console hinzugefügt wurden, können diese Benutzer der Benutzerkonfigurationsdatei von Brand Portal hinzugefügt werden. Anschließend kann ihnen die Zugriffsberechtigung auf den Beitragsordner zugewiesen werden.

**Hochladen der Brand Portal-Benutzerliste:**
1. Melden Sie sich bei Ihrer AEM Assets-Instanz an.
1. Navigieren Sie im Bedienfeld **Tools** zu **[!UICONTROL Assets]** > **[!UICONTROL Markenportal-Benutzer]**.

1. Das Fenster zum Hochladen von Beitragenden zu Brand Portal wird geöffnet.
Durchsuchen Sie Ihren lokalen Computer und laden Sie die **Konfigurationsdatei (.csv)** hoch, die die Liste der aktiven Brand Portal-Benutzer enthält.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/upload-user-list2.png)


Administratoren können bestimmten Benutzern über diese Liste Zugriff gewähren, während sie einen Beitragsordner konfigurieren. Nur die Benutzer, die einem Beitragsordner zugewiesen sind, haben Zugriff auf den Beitragsordner und veröffentlichen Assets vom Markenportal nach AEM Assets.

## Siehe auch {#reference-articles}

* [Konfigurieren und Veröffentlichen des Beitragsordners für das Markenportal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Veröffentlichen von Beitragsordnern in AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
