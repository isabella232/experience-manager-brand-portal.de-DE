---
title: Versionshinweise
seo-title: Versionshinweise
description: Hier erhalten Sie nützliche Informationen zu Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 2021.02.0.
seo-description: Hier erhalten Sie nützliche Informationen zu Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 2021.02.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: d70817274ac7be84528778352f34934a0d4a60fc
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 54%

---


# Versionshinweise {#release-notes}

Hier erhalten Sie nützliche Informationen zu neuen Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 2021.02.0.

## Versionshinweise {#release-information}

| Produkt | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 2021,02,0 |
| Datum | Februar 2021 |

## Überblick {#overview}

Mit Adobe Experience Manager (AEM) Assets Brand Portal können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen. Brand Portal ermöglicht eine effizientere Asset-Freigabe, schnellere Time-to-Market für Assets sowie verringerte Risiken von Nicht-Compliance und unbefugtem Zugriff. Brand Portal bietet Benutzern die Möglichkeit, Assets jederzeit und überall zu durchsuchen, zu suchen, als Vorschau anzuzeigen, herunterzuladen und in Formate zu exportieren, die vom Unternehmen genehmigt wurden.

## Neue Funktionen in Version 2021.02.0 {#whats-new-in-2021.02.0}

### Neue Funktionen {#new-features}

Diese Version umfasst die folgenden neuen Funktionen:

* Die Asset-Sourcing-Funktion ist jetzt auf AEM Assets als Cloud Service verfügbar. Dadurch können Benutzer des Markenportals Assets in die zulässigen Beitragsordner hochladen und den Beitragsordner vom Markenportal nach AEM Assets als Cloud Service veröffentlichen.

* Unter **[!UICONTROL Download-Einstellungen]** wurde eine zusätzliche Einstellung für **[!UICONTROL Asset-Download]** eingeführt. Beim Herunterladen der Ordner, Sammlungen oder beim Herunterladen von Assets wird für jedes Asset ein separater Ordner erstellt. Siehe [Download-Einstellungen](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download).

<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

### Verbesserungen {#enhancements}

Diese Version umfasst die folgenden Verbesserungen:

* Beim Herunterladen von Ordnern wird für jedes Asset unabhängig von den **[!UICONTROL Download-Einstellungen]** ein separater Ordner über den Link &quot;Teilen&quot;erstellt.
* Das Markenportal **[!UICONTROL Gebrauchsbericht]** wurde geändert, um nur die aktiven Markenportalbenutzer wiederzugeben.

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Behobene kritische Probleme {#critical-issues-fixed}

Diese Version umfasst Behebungen für die folgenden kritischen Probleme:

* Wenn nur die ursprünglichen Assets heruntergeladen werden, spiegelt das Asset seine eigene Erweiterung wider und wird erst geöffnet, wenn die Erweiterung manuell in ZIP geändert wird.
* Die Benutzeroberfläche des Sammlungsordners reagiert nicht, wenn auf den Navigationspfeil geklickt wird.
* **[!UICONTROL Die]** Option &quot;Erstellen&quot;ist auch dann in der  **** Spaltenansicht sichtbar, wenn die Ordner leer sind.
* **[!UICONTROL Die Omni-]** Suche schlägt mit einer 414-Fehlermeldung fehl (Anforderung-URI zu lang), wenn der Dispatcher beim Zugriff auf die Brand Portal-Instanz umgangen wird.
* Ein leerer ZIP-Ordner wird heruntergeladen, wenn das Asset im Dateinamen ein Komma (`,`) enthält.
* Die Viewer-Benutzer erhalten die Möglichkeit, Benutzer zur erstellten Sammlung hinzuzufügen.
* Inkonsistentes Verhalten tritt auf, wenn ein Asset (Miniaturansicht oder Webdarstellung) über einen Freigabelink heruntergeladen wird.

Siehe [Neue Funktionen im Markenportal 2021.02.0](whats-new.md).


### Bekannte Probleme {#known-issues}

Diese Version enthält die folgenden bekannten Probleme:

* Die Benutzer erhalten keine E-Mail-Benachrichtigungen für den Asset Sourcing-Workflows.

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


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
* Brasilianisches Portugiesisch
* Japanisch
* Vereinfachtes Chinesisch
* Koreanisch

## Zertifizierte Plattformen {#certified-platforms}

Informationen dazu, welche Plattformen für diese Version von Brand Portal zertifiziert sind, finden Sie in der Spalte **Unterstützung für Touch-optimierte Benutzeroberfläche** in der Tabelle im Bereich **Unterstützte Browser für die Autoren-Benutzeroberfläche** unter [Technische Anforderungen](https://helpx.adobe.com/de/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

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
