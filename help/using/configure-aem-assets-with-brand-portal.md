---
title: Konfigurieren von AEM Assets mit Brand Portal
seo-title: Konfigurieren von AEM Assets mit Brand Portal
description: Hier erhalten Sie einen Einblick in die Konfiguration von AEM Assets mit Brand Portal.
seo-description: Hier erhalten Sie einen Einblick in die Konfiguration von AEM Assets mit Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: ht
source-git-commit: ba8a1f09573766643f6a5013a8d181f0f0dbb4f2
workflow-type: ht
source-wordcount: '335'
ht-degree: 100%

---


# Konfigurieren von AEM Assets mit Brand Portal {#configure-integration}

Adobe Experience Manager (AEM) Assets wird über Adobe Developer Console mit Brand Portal konfiguriert. Dadurch wird ein IMS-Token zur Autorisierung Ihres Brand Portal-Mandanten abgerufen. Brand Portal wird jetzt von AEM Assets Cloud Service, AEM Assets 6.3 und hher unterstützt.

Durch die Konfiguration von AEM Assets Cloud Service mit Brand Portal können Sie Assets veröffentlichen und an Benutzer von Brand Portal verteilen. Die Konfiguration von Brand Portal unter AEM 6.3 (und höher) wiederum bietet den Benutzern von Brand Portal Funktionen zu Asset-Veröffentlichung, Asset-Verteilung und Mitarbeit an Assets.

>[!NOTE]
>
>***Für AEM Assets 6.3 und höher***
>
>Zuvor wurde Brand Portal über das alte OAuth-Gateway in der klassischen Benutzeroberfläche konfiguriert. Das Gateway ruft mithilfe des JWT-Token-Austauschs ein IMS-Zugriffstoken zur Autorisierung ab.
>
>Die Konfiguration über das alte OAuth-Protokoll wird ab dem 6. April 2020 nicht mehr unterstützt, sondern erfolgt nun über Adobe Developer Console.


>[!TIP]
>
>***Nur für Bestandskunden***
>
>Die alte OAuth Gateway-Konfiguration funktioniert für bestehende Kunden weiterhin.
>
>Falls Probleme mit der alten OAuth-Gateway-Konfiguration auftreten, löschen Sie die vorhandene Konfiguration und erstellen Sie eine neue Konfiguration über Adobe Developer Console.


Die Schritte zum Konfigurieren von AEM Assets mit Brand Portal unterscheiden sich je nach Ihrer AEM-Version und davon, ob Sie zum ersten Mal eine Konfiguration durchführen oder die vorhandenen Konfigurationen aktualisieren:

| **AEM-Version** | **Neue Konfiguration** | **Upgrade der Konfiguration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Konfiguration erstellen](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 und höher)** | [Konfiguration erstellen](https://docs.adobe.com/content/help/de-DE/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.translate.html) | [Upgrade der Konfiguration](https://docs.adobe.com/content/help/de-DE/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.translate.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 und höher)** | [Konfiguration erstellen](https://docs.adobe.com/content/help/de-DE/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgrade der Konfiguration](https://docs.adobe.com/content/help/de-DE/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 und höher)** | [Konfiguration erstellen](https://helpx.adobe.com/de/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgrade der Konfiguration](https://helpx.adobe.com/de/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Support kontaktieren | Support kontaktieren |


