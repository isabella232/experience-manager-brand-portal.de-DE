---
title: Asset-Beschaffung konfigurieren
seo-title: Asset-Beschaffung konfigurieren
description: Hier erhalten Sie einen Einblick in die Konfiguration der Asset-Sourcing-Funktion in AEM Assets.
seo-description: Hier erhalten Sie einen Einblick in die Konfiguration der Asset-Sourcing-Funktion in AEM Assets.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: add4009bd99e5af8ed0c9ffea63647c166b7c75d

---


# Configure Asset Sourcing {#configure-asset-sourcing}

AEM-Administratoren können die **Asset-Beschaffung** aus der AEM-Autoreninstanz konfigurieren. Der Administrator aktiviert die Konfiguration für das Flag "Asset Sourcing"-Feature aus der **AEM Web Console-Konfiguration** und lädt die Liste der aktiven Markenportal-Benutzer in **AEM Assets** hoch.

>[!NOTE]
>
>Bevor Sie mit der Konfiguration beginnen, stellen Sie sicher, dass Ihre AEM Assets-Instanz in das Markenportal integriert ist. Siehe [Konfigurieren der Integration von AEM Assets mit Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html).


Das folgende Video zeigt, wie Sie die Asset-Sourcing in Ihrer AEM-Autoreninstanz konfigurieren:

>[!VIDEO](https://video.tv.adobe.com/v/29771?captions=ger)

## Aktivieren der Asset-Beschaffung {#enable-asset-sourcing}

AEM-Administratoren können die Asset-Beschaffung über die AEM-Web-Konsolen-Konfiguration (auch Configuration Manager genannt) aktivieren.

**Aktivieren der Asset-Beschaffung:**
1. Melden Sie sich bei Ihrer AEM-Autoreninstanz an und öffnen Sie Configuration Manager.
Standard-URL: http:// localhost:4502/system/console/configMgr
1. Suchen Sie nach **Asset-Beschaffung**, um die **[!UICONTROL Konfiguration der Asset-Beschaffungsfunktionskennzeichnung]** zu finden.
1. Klicken Sie auf **[!UICONTROL Konfiguration der Asset-Beschaffungsfunktionskennzeichnung]**, um das Konfigurationsfenster zu öffnen.
1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL feature.flag.active.status]**
1. Klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/enable-asset-sourcing.png)

## Hochladen der Brand Portal-Benutzerliste {#upload-bp-user-list}

AEM-Administratoren können die Datei für die Brand Portal-Benutzerkonfiguration (.csv) hochladen, die eine Liste der aktiven Brand Portal-Benutzer in AEM Assets enthält. Ein Beitragsordner kann nur für die aktiven Brand Portal-Benutzer freigegeben werden, die in der Benutzerliste definiert sind. Administratoren können der Konfigurationsdatei auch neue Benutzer hinzufügen und die geänderte Benutzerliste hochladen.

Administratoren können neue Benutzer in AEM Admin Console hinzufügen. Weitere Informationen finden Sie unter [Benutzer verwalten](brand-portal-adding-users.md). Nachdem Benutzer in Admin Console hinzugefügt wurden, können diese Benutzer der Benutzerkonfigurationsdatei von Brand Portal hinzugefügt werden. Anschließend kann ihnen die Zugriffsberechtigung auf den Beitragsordner zugewiesen werden.

**Hochladen der Brand Portal-Benutzerliste:**
1. Melden Sie sich bei Ihrer AEM-Autoreninstanz an.
Standard-URL: http:// localhost:4502/aem/start.html
1. Navigieren Sie vom Bedienfeld **Werkzeuge** ![](assets/tools.png) zu **[!UICONTROL Assets &gt; Brand Portal-Benutzer]**.
   ![](assets/upload-user-list1.png)
1. Das Fenster zum Hochladen von Beitragenden zu Brand Portal wird geöffnet.
Durchsuchen Sie Ihren lokalen Computer und laden Sie die **Konfigurationsdatei (.csv)** hoch, die die Liste der aktiven Brand Portal-Benutzer enthält.
1. Klicken Sie auf **[!UICONTROL Speichern]**.
   ![](assets/upload-user-list2.png)


Administratoren können über diese Benutzerliste Zugriff auf bestimmte Benutzer/Gruppen gewähren, während sie den Beitragsordner konfigurieren.

Weitere Informationen finden Sie unter [Konfigurieren von Beitragsordnern](brand-portal-contribution-folder.md).
