---
title: Versionshinweise
seo-title: Versionshinweise
description: Hier erhalten Sie nützliche Informationen zu Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 6.4.6.
seo-description: Hier erhalten Sie nützliche Informationen zu Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 6.4.6.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: a357879f921ac88f89d1bc11bff379f1d0d3e681

---


# Versionshinweise {#release-notes}

Hier erhalten Sie nützliche Informationen zu neuen Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 6.4.6.

## Versionshinweise {#release-information}

| Produkt | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 6.4.6 |
| Datum | &amp;#x200B;. März 2020 |

## Überblick {#overview}

Mit Adobe Experience Manager (AEM) Assets Brand Portal können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen. Brand Portal ermöglicht eine effizientere Asset-Freigabe, schnellere Time-to-Market für Assets sowie verringerte Risiken von Nicht-Compliance und unbefugtem Zugriff. Brand Portal bietet Benutzern die Möglichkeit, Assets jederzeit und überall zu durchsuchen, zu suchen, als Vorschau anzuzeigen, herunterzuladen und in Formate zu exportieren, die vom Unternehmen genehmigt wurden.

## Neue Funktionen in Version 6.4.6 {#what-s-new-in-646}

### Neue Funktionen {#new-feature}

Diese Version umfasst die folgenden neuen Funktionen:

* Captcha für die Gast-Anmeldung bei Brand Portal. Weitere Informationen finden Sie unter [Gast-Zugriff auf Brand Portal](../using/guest-access.md).

* Markenportal wird jetzt mit dem AEM Assets-Cloud-Dienst unterstützt. Sie können AEM Assets könnte mit dem Brand Portal Dienst für die Freigabe und Verteilung von Assets für die Benutzer des Markenportals einrichten.
For more information, see [Configure AEM Assets cloud service with Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brandportal/configure-aem-assets-with-brand-portal.html).

### Verbesserungen {#enhancements-646}

Diese Version von Brand Portal umfasst die folgenden Verbesserungen:

* In AEM 6.3 und höher wird der Kanal für die Autorisierung zwischen AEM Assets und Brand Portal geändert. AEM Assets wird jetzt über Adobe I/O in Brand Portal konfiguriert. Die Konsole ruft das IMS-Token zur Authentifizierung Ihres Brand Portal-Mandanten ab.

   >[!NOTE]
   >
   >Die Konfiguration über Legacy OAuth wird ab dem 6. April 2020 nicht mehr unterstützt, sondern erfolgt nun über Adobe I/O.


>[!TIP]
>
>***Nur für bestehende Kunden***
>
>Es wird empfohlen, weiterhin die vorhandene alte OAuth Gateway-Konfiguration zu verwenden. Falls Probleme mit der alten OAuth Gateway-Konfiguration auftreten, löschen Sie die vorhandene Konfiguration und erstellen Sie eine neue Konfiguration über Adobe I/O.


Weitere Informationen finden Sie unter [Konfigurieren von AEM Assets mit Brand Portal](configure-aem-assets-with-brand-portal.md).

### Behobene kritische Probleme {#critical-issues-fixed}

Diese Version umfasst Behebungen für die folgenden kritischen Probleme:

* Dropdown-Werte für Metadatenschemas werden in den Asset-Eigenschaften nicht angezeigt.

* Metadaten-Unterschema zeigt keine Registerkarten basierend auf dem MIME-Typ in den Asset-Eigenschaften an.

* Beim Rückgängigmachen der Veröffentlichung des Metadatenschemas wird eine Fehlermeldung angezeigt, obwohl das Schema im Backend entfernt wurde.

* Für ein veröffentlichtes Asset wird kein Vorschaubild angezeigt.

* Benutzer können Assets, die ein einzelnes Anführungszeichen im Namen enthalten, nicht veröffentlichen oder die Veröffentlichung rückgängig machen.

* Die Geschäftsbedingungen werden beim Herunterladen mehrerer Assets nicht angezeigt.

* Geringfügige Sicherheitslücken wurden behoben.

### Bekannte Probleme {#known-issues}

Dieses Release weist die folgenden bekannten Probleme auf:

* Benutzer von Markenportalen können beim Aktualisieren auf Adobe I/O auf AEM 6.5.4 keine Beitragsordnerelemente in AEM Assets veröffentlichen.

   Dieses Problem wird im nächsten Service Pack 6.5.5 behoben.

   Für eine sofortige Fehlerbehebung in AEM 6.5.4 wird empfohlen, den Hotfix [](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) herunterzuladen und auf Ihrer Autoreninstanz zu installieren.

* Die Option &quot;Systemwiedergaben ausschließen&quot;funktioniert beim Herunterladen eines Assets nicht ordnungsgemäß.


## Sprachen {#languages}

Die Brand Portal-Benutzeroberfläche ist in den folgenden Sprachen verfügbar:

* Englisch
* Deutsch
* Französisch
* Spanisch
* Italienisch
* Brasilianisches   Portugiesisch
* Japanisch
* Vereinfachtes Chinesisch
* Koreanisch

## Zertifizierte Plattformen    {#certified-platforms}

Informationen dazu, welche Plattformen für diese Version von Brand Portal zertifiziert sind, finden Sie in der Spalte **Unterstützung für Touch-optimierte Benutzeroberfläche** in der Tabelle im Bereich **Unterstützte Browser für die Autoren-Benutzeroberfläche** unter [Technische Anforderungen ](https://helpx.adobe.com/de/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Links {#links}

* [Adobe Experience Manager-Produktseite unter adobe.com](http://www.adobe.com/de/marketing-cloud/experience-manager.html)
* [Assets Brand Portal-Dokumentation](https://helpx.adobe.com/de/experience-manager/brand-portal/user-guide.html)

## Produktzugriff und Support (Websites mit Zugriffsbeschränkung) {#product-access-and-support-restricted-sites}

Diese Sites sind nur für Kunden verfügbar. Wenn Sie Kunde sind und Zugriff benötigen, wenden Sie sich an Ihren Adobe-Kundenbetreuer.

* [](https://daycare.day.com) [Produktzugriff](https://login.marketing.adobe.com)

* [Adobe-Kundendienst](https://helpx.adobe.com/de/contact.html)
