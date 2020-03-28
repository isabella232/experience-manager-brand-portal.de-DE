---
title: Konfigurieren von AEM Assets mit Brand Portal
seo-title: Konfigurieren von AEM Assets mit Brand Portal
description: Hier erhalten Sie einen Einblick in die Konfiguration von AEM Assets mit Brand Portal.
seo-description: Hier erhalten Sie einen Einblick in die Konfiguration von AEM Assets mit Brand Portal.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 6b03229b72a1912be57c2bc1b7e47a017d3dca7e

---


# Konfigurieren von AEM Assets mit Brand Portal {#configure-integration}

Adobe Experience Manager (AEM) Assets wird über Adobe I/O in Brand Portal konfiguriert. Dadurch wird ein IMS-Token zur Autorisierung Ihres Brand Portal-Mandanten abgerufen. Die Konfiguration ermöglicht die Veröffentlichung und Verteilung von Assets sowie Asset-Beitragsfunktionen für Brand Portal-Benutzer.

>[!NOTE]
>
>Zuvor wurde Brand Portal über das Legacy-OAuth-Gateway in der klassischen Benutzeroberfläche konfiguriert. Das Gateway ruft mithilfe des JWT-Token-Austauschs ein IMS-Zugriffstoken zur Autorisierung ab.
>
>Die Konfiguration über Legacy OAuth wird ab dem 6. April 2020 nicht mehr unterstützt, sondern erfolgt nun über Adobe I/O.


>[!TIP]
>
>***Nur für bestehende Kunden***
>
>Es wird empfohlen, weiterhin die vorhandene alte OAuth Gateway-Konfiguration zu verwenden. Falls Probleme mit der alten OAuth Gateway-Konfiguration auftreten, löschen Sie die vorhandene Konfiguration und erstellen Sie eine neue Konfiguration über Adobe I/O.


Die Schritte zum Konfigurieren von AEM Assets mit Brand Portal unterscheiden sich je nach Ihrer AEM-Version und davon, ob Sie zum ersten Mal eine Konfiguration durchführen oder die vorhandenen Konfigurationen aktualisieren:

| **AEM-Version** | **Neue Konfiguration** | **Upgrade der Konfiguration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 und höher)** | [Konfiguration erstellen](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgrade der Konfiguration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 und höher)** | [Konfiguration erstellen](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgrade der Konfiguration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 und höher)** | [Konfiguration erstellen](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgrade der Konfiguration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Support kontaktieren | Support kontaktieren |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
