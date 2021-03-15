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
translation-type: tm+mt
source-git-commit: bfb0c38bf8d5b542caf9d0d20d3168cdcac649b3
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 60%

---


# Konfigurieren von AEM Assets mit Brand Portal {#configure-integration}

Die Konfiguration von Adobe Experience Manager Assets mit dem Markenportal ermöglicht den Benutzern des Markenportals Funktionen zum Veröffentlichen von Assets, zur Asset-Verteilung und zum Asset-Beitrag. Sie ermöglicht es den AEM Assets-Benutzern, Assets zu veröffentlichen und mit den Benutzern des Markenportals zu verteilen. Die Benutzer des Markenportals können auf die freigegebenen Assets zugreifen und einen Beitrag leisten, indem sie neue Assets in die Asset-Beitragsordner hochladen und auf AEM Assets veröffentlichen.

Die Konfiguration von AEM Assets mit dem Markenportal wird unterstützt unter:
* AEM Assets as a Cloud Service
* AEM Assets (Vor-Ort- und Managed Services-Gebäude) 6.3 und höher

AEM Assets als Cloud Service wird automatisch mit dem Markenportal konfiguriert, indem das Markenportal über den Cloud Manager aktiviert wird. Der Arbeitsablauf für die Aktivierung erstellt die erforderlichen Konfigurationen am Backend und aktiviert das Markenportal auf demselben IMS-Format wie das AEM Assets als Cloud Service-Instanz.

Dagegen wird AEM Assets (lokal und Managed Services) manuell mit dem Markenportal mithilfe der Adobe Developer Console konfiguriert, die ein Adobe Identity Management Services (IMS)-Token zur Genehmigung des Markenportal-Mieters abruft.

>[!NOTE]
>
>***Für AEM Assets 6.3 und höher***
>
>Zuvor wurde Brand Portal über das alte OAuth-Gateway in der klassischen Benutzeroberfläche konfiguriert. Das Gateway ruft mithilfe des JSON Web Token (JWT)-Austauschs ein IMS-Token zur Autorisierung ab.
>
>Die Konfiguration über das alte OAuth-Protokoll wird ab dem 6. April 2020 nicht mehr unterstützt, sondern erfolgt nun über Adobe Developer Console.


>[!TIP]
>
>***Nur für Bestandskunden (in Betrieb und Managed Services)***
>
>Die alte OAuth Gateway-Konfiguration funktioniert für bestehende Kunden weiterhin.
>
>Falls Probleme mit der alten OAuth-Gateway-Konfiguration auftreten, löschen Sie die vorhandene Konfiguration und erstellen Sie eine neue Konfiguration über Adobe Developer Console.

Die Schritte zum Konfigurieren von AEM Assets mit Brand Portal unterscheiden sich je nach Ihrer AEM-Version und abhängig davon, ob Sie zum ersten Mal eine Konfiguration durchführen oder die vorhandenen Konfigurationen aktualisieren:

| **AEM-Version** | **Neue Konfiguration** | **Upgrade der Konfiguration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Brand Portal aktivieren](https://docs.adobe.com/content/help/de-DE/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 und höher)** | [Konfiguration erstellen](https://docs.adobe.com/content/help/de-DE/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgrade der Konfiguration](https://docs.adobe.com/content/help/de-DE/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 und höher)** | [Konfiguration erstellen](https://docs.adobe.com/content/help/de-DE/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgrade der Konfiguration](https://docs.adobe.com/content/help/de-DE/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 und höher)** | [Konfiguration erstellen](https://helpx.adobe.com/de/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgrade der Konfiguration](https://helpx.adobe.com/de/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Support kontaktieren | Support kontaktieren |
