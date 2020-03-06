---
title: Konfigurieren der von AEM Assets mit Brand Portal
seo-title: Konfigurieren der von AEM Assets mit Brand Portal
description: Hier erhalten Sie einen Einblick in die Konfiguration von AEM Assets mit dem Markenportal.
seo-description: Hier erhalten Sie einen Einblick in die Konfiguration von AEM Assets mit dem Markenportal.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 58110f1635a9e74340d4a8901e86c0c6a99cf4e2

---


# Konfigurieren der von AEM Assets mit Brand Portal {#configure-integration}

Adobe Experience Manager (AEM)-Assets werden über die Adobe-ID/O mit dem Markenportal konfiguriert. Dadurch wird ein IMS-Token zur Autorisierung Ihres Markenportal-Mandanten beschafft. Die Konfiguration ermöglicht die Veröffentlichung von Assets, die Verteilung von Assets und Asset-Beitragsfunktionen für die Benutzer des Markenportals.

>[!NOTE]
>
>Zuvor wurde Brand Portal über das Legacy-OAuth-Gateway in der klassischen Benutzeroberfläche konfiguriert. Das Gateway ruft mithilfe des JWT-Token-Austauschs ein IMS-Zugriffstoken zur Autorisierung ab.
>
>Die Konfiguration über Legacy-OAuth wird ab dem 6. April 2020 nicht mehr unterstützt. Die Konfiguration erfolgt nun über Adobe I/O.
>
>Wenn Sie ein bestehender Brand Portal-Benutzer mit einer Konfiguration auf dem alten OAuth Gateway sind, sollten Sie die vorhandenen Konfigurationen löschen und eine neue Konfiguration auf der Adobe-E/A-Datei erstellen.
>
>Die vorhandene Konfiguration funktioniert jedoch weiterhin, wenn Sie die Konfigurationen nicht ändern.

Die Schritte zum Konfigurieren von AEM Assets mit dem Markenportal unterscheiden sich je nach Ihrer AEM-Version und ob Sie zum ersten Mal konfigurieren oder die vorhandenen Konfigurationen aktualisieren:

| **AEM-Version** | **Neue Konfiguration** | **Konfiguration aktualisieren** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 und höher)** | [Konfiguration erstellen](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Konfiguration aktualisieren](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 und höher)** | [Konfiguration erstellen](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Konfiguration aktualisieren](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 und höher)** | [Konfiguration erstellen](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Konfiguration aktualisieren](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Support kontaktieren | Support kontaktieren |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
