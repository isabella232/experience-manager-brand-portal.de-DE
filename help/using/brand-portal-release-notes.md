---
title: Versionshinweise
seo-title: Versionshinweise
description: Hier erhalten Sie nützliche Informationen zu Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 2020.10.0.
seo-description: Hier erhalten Sie nützliche Informationen zu Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 2020.10.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 4774d8a78657c89081d229ce596a3bd404ae1bc8
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 50%

---


# Versionshinweise {#release-notes}

Hier erhalten Sie nützliche Informationen zu neuen Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 2020.10.0.

## Versionshinweise {#release-information}

| Produkt | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 2020.10.0 |
| Datum            | Oktober 2020 |

## Überblick {#overview}

Mit Adobe Experience Manager (AEM) Assets Brand Portal können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen. Brand Portal ermöglicht eine effizientere Asset-Freigabe, schnellere Time-to-Market für Assets sowie verringerte Risiken von Nicht-Compliance und unbefugtem Zugriff. Brand Portal bietet Benutzern die Möglichkeit, Assets jederzeit und überall zu durchsuchen, zu suchen, als Vorschau anzuzeigen, herunterzuladen und in Formate zu exportieren, die vom Unternehmen genehmigt wurden.

## Neue Funktionen in Version 2020.10.0 {#whats-new-in-2020.10.0}

### Neue Funktionen {#new-features}

Diese Version umfasst die folgenden neuen Funktionen:

* Das Dialogfeld &quot; **[!UICONTROL Herunterladen]** &quot;wird in einer Liste-Ansicht mit zusätzlichen Optionen zum Ausschließen nicht erforderlicher Darstellungen, zum Anwenden desselben Regelsatzes für ähnliche Asset-Typen und zum Herunterladen der ausgewählten Asset-Darstellungen überarbeitet. Siehe [Schritte zum Herunterladen von Assets aus dem Markenportal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* Die Navigation zu den **[!UICONTROL Dateien]**, **[!UICONTROL Sammlungen]** und **[!UICONTROL freigegebenen Links]** ist jetzt von allen Seiten des Markenportals mit einem Klick möglich.

* Das Bedienfeld &quot; **[!UICONTROL Darstellungen]** &quot;auf der Seite mit den Asset-Details ermöglicht es den Benutzern des Markenportals nun, das ursprüngliche Asset und (oder) bestimmte Asset-Darstellungen auszuwählen und sie direkt aus dem Bedienfeld &quot; **[!UICONTROL Darstellungen]** &quot;herunterzuladen, ohne das Dialogfeld &quot; **[!UICONTROL Herunterladen]** &quot;öffnen zu müssen. Siehe Seite [zum Herunterladen von Assets aus den Asset-Details](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* Zusätzlich zu den vorhandenen **[!UICONTROL Download]** -Konfigurationen können die Markenportal-Administratoren auch Berechtigungen für verschiedene Benutzergruppen [für die Ansicht](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) konfigurieren und (oder) das Originalasset und dessen Darstellungen von der Seite mit den Asset-Details herunterladen. Diese Konfigurationen definieren, wer auf die Asset-Darstellungen zugreifen und (oder) sie herunterladen kann.

### Verbesserungen {#enhancements}

Diese Version umfasst die folgenden Verbesserungen:

* Der Schwellenwert für die Sitzungs-Timeout für die Gastbenutzer wurde von 2 Stunden auf 15 Minuten verringert.
* Die Option &quot;Zusätzliche **[!UICONTROL Ansichten]** &quot;wurde für mehrseitige PDFs entfernt, da der Benutzer die PDF-Seiten jetzt aus dem Adobe Document Cloud Viewer Ansicht haben kann.


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### Bekannte Probleme {#known-issues}

Diese Version enthält das folgende bekannte Problem:

* Die Suche in den **[!UICONTROL Asset-Berichten]** zeigt die Verarbeitung auf der Produktoberfläche ohne Suchergebnis an.
* Die Video-DM-Kodierungen sind für Benutzer, die keine Administratoren sind, auf der Seite mit den Asset-Details nicht sichtbar.
* Die Ausrichtung der Größe einzelner Asset-Darstellungen und der maximalen Downloadgröße wird im Dialogfeld &quot;Herunterladen&quot;verzerrt.



<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## Sprachen {#languages}

Die Brand Portal-Benutzeroberfläche ist in den folgenden Sprachen verfügbar:

* Englisch
* Deutsch
* Französisch
* Spanisch
* Italienisch
* Brasilianisches       Portugiesisch
* Japanisch
* Vereinfachtes Chinesisch
* Koreanisch

## Zertifizierte Plattformen                {#certified-platforms}

Informationen dazu, welche Plattformen für diese Version von Brand Portal zertifiziert sind, finden Sie in der Spalte **Unterstützung für Touch-optimierte Benutzeroberfläche** in der Tabelle im Bereich **Unterstützte Browser für die Autoren-Benutzeroberfläche** unter [Technische Anforderungen ](https://helpx.adobe.com/de/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Links {#links}

* [Adobe Experience Manager-Produktseite unter adobe.com](http://www.adobe.com/de/marketing-cloud/experience-manager.html)
* [Assets Brand Portal-Dokumentation](https://helpx.adobe.com/de/experience-manager/brand-portal/user-guide.html)

## Produktzugriff und Support (Websites mit Zugriffsbeschränkung) {#product-access-and-support-restricted-sites}

Diese Sites sind nur für Kunden verfügbar. Wenn Sie Kunde sind und Zugriff benötigen, wenden Sie sich an Ihren Adobe-Kundenbetreuer.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Produktzugriff](https://login.marketing.adobe.com)

* [Adobe-Kundenunterstützung](https://helpx.adobe.com/de/contact.html)
