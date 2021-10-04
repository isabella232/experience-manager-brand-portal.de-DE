---
title: Konfigurieren von Experience Manager Assets mit Brand Portal
seo-title: Configure Experience Manager Assets with Brand Portal
description: Hier erhalten Sie einen Einblick in die Konfiguration von Experience Manager Assets mit Brand Portal.
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 49%

---

# Konfigurieren von Experience Manager Assets mit Brand Portal {#configure-integration}

Die Konfiguration von Adobe Experience Manager Assets mit Brand Portal bietet Benutzern von Brand Portal Funktionen zur Asset-Veröffentlichung, Asset-Verteilung und Mitarbeit an Assets. Dadurch können Experience Manager-Assets-Benutzer Assets veröffentlichen und an die Brand Portal-Benutzer verteilen. Die Brand Portal-Benutzer können auf die freigegebenen Assets zugreifen und Beiträge hinzufügen, indem sie neue Assets in die Asset-Beitragsordner hochladen und sie wieder in Experience Manager-Assets veröffentlichen.

Die Konfiguration von Experience Manager Assets mit Brand Portal wird unterstützt unter:

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets (On-Premise und Managed Service) 6.3 und höher

Experience Manager Assets as a Cloud Service wird automatisch mit Brand Portal konfiguriert, indem Brand Portal über Cloud Manager aktiviert wird. Der Aktivierungs-Workflow erstellt die erforderlichen Konfigurationen im Backend und aktiviert Brand Portal auf derselben IMS-Organisation wie die Experience Manager Assets als Cloud Service-Instanz.

Im Gegensatz dazu wird Experience Manager Assets (On-Premise und verwalteter Dienst) mithilfe der Adobe Developer Console manuell mit Brand Portal konfiguriert. Dadurch wird ein Adobe Identity Management Services (IMS)-Token zur Autorisierung des Brand Portal-Mandanten abgerufen.

>[!NOTE]
>
>***Für Experience Manager Assets 6.3 und höher***
>
>Zuvor wurde Brand Portal über das alte OAuth-Gateway in der klassischen Benutzeroberfläche konfiguriert. Das Gateway ruft mithilfe des JSON Web Token (JWT)-Austauschs ein IMS-Token zur Autorisierung ab.
>
>Die Konfiguration über das alte OAuth-Protokoll wird ab dem 6. April 2020 nicht mehr unterstützt, sondern erfolgt nun über Adobe Developer Console.


>[!TIP]
>
>***Nur für Bestandskunden (On-Premise und Managed Service)***
>
>Die alte OAuth Gateway-Konfiguration funktioniert für bestehende Kunden weiterhin.
>
>Falls Probleme mit der alten OAuth-Gateway-Konfiguration auftreten, löschen Sie die vorhandene Konfiguration und erstellen Sie eine neue Konfiguration über Adobe Developer Console.

Die Schritte zum Konfigurieren von AEM Assets mit Brand Portal unterscheiden sich je nach Ihrer AEM-Version und abhängig davon, ob Sie zum ersten Mal eine Konfiguration durchführen oder die vorhandenen Konfigurationen aktualisieren:

| **AEM-Version** | **Neue Konfiguration** | **Upgrade der Konfiguration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Brand Portal aktivieren](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 und höher)** | [Konfiguration erstellen](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgrade der Konfiguration](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 und höher)** | [Konfiguration erstellen](https://experienceleague.adobe.com/docs/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgrade der Konfiguration](https://experienceleague.adobe.com/docs/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 und höher)** | [Konfiguration erstellen](https://helpx.adobe.com/de/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgrade der Konfiguration](https://helpx.adobe.com/de/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Support kontaktieren | Support kontaktieren |
