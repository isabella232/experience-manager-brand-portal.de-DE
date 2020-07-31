---
title: Versionshinweise
seo-title: Versionshinweise
description: Hier erhalten Sie nützliche Informationen zu Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 6.4.6.2.
seo-description: Hier erhalten Sie nützliche Informationen zu Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 6.4.6.2.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: ht
source-git-commit: 70640f9fa605d56160f01fde577ee699cfaac08d
workflow-type: ht
source-wordcount: '813'
ht-degree: 100%

---


# Versionshinweise {#release-notes}

Hier erhalten Sie nützliche Informationen zu neuen Funktionen, Verbesserungen, behobenen kritischen Problemen sowie bekannten Problemen in Adobe Experience Manager Assets Brand Portal 6.4.6.2.

## Versionshinweise {#release-information}

| Produkt | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 6.4.6.2 |
| Datum | Juni 2020 |

## Überblick {#overview}

Mit Adobe Experience Manager (AEM) Assets Brand Portal können Sie problemlos genehmigte Kreativ-Assets abrufen, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer auf allen Geräten verteilen. Brand Portal ermöglicht eine effizientere Asset-Freigabe, schnellere Time-to-Market für Assets sowie verringerte Risiken von Nicht-Compliance und unbefugtem Zugriff. Brand Portal bietet Benutzern die Möglichkeit, Assets jederzeit und überall zu durchsuchen, zu suchen, als Vorschau anzuzeigen, herunterzuladen und in Formate zu exportieren, die vom Unternehmen genehmigt wurden.

## Neue Funktionen in Version 6.4.6.2 {#what-s-new-in-6462}

### Behobene kritische Probleme {#critical-issues-fixed-6462}

Diese Version umfasst Behebungen für die folgenden kritischen Probleme:

* Wenn Sie ein veröffentlichtes Metadatenschema aus Brand Portal entfernen, wird ein Fehler ausgegeben.

* Wenn der Administrator Experience Manager Assets 6.5.4 mit Brand Portal über Adobe Developer Console konfiguriert, können Brand Portal-Benutzer die Assets des Beitragsordners nicht von Brand Portal in Experience Manager veröffentlichen.

* Doppelte Replikation der übergeordneten Ordner, die Konflikte verursachen.

* Benutzer kann den Bericht zur Linkfreigabe nicht erstellen.

* Benutzer können MAC-Geheimnisse für einen Brand Portal-Endpunkt mit dem Befehl „copyPage“ kopieren.

* cqTags verursachen eine Neuindizierung des VA5-Klons.


### Bekannte Probleme {#known-issues-6462}

Dieses Release weist die folgenden bekannten Probleme auf:

* Benutzer mit der Rolle „Beobachter“ dürfen keine Links für Sammlungen freigeben, die Option zum Freigeben ist für sie jedoch in der Produktoberfläche sichtbar.

* Wenn ein Ordner in der Hierarchie von AEM Assets umbenannt wird und der verschachtelte Ordner, der ein Asset enthält, in Brand Portal veröffentlicht wird, wird der Titel des Ordners in Brand Portal erst dann aktualisiert, wenn der Stammordner erneut veröffentlicht wird.


## Neue Funktionen in Version 6.4.6 {#what-s-new-in-646}

### Neue Funktionen {#new-feature}

Diese Version umfasst die folgenden neuen Funktionen:

* Captcha für die Gast-Anmeldung bei Brand Portal. Weitere Informationen finden Sie unter [Gast-Zugriff auf Brand Portal](../using/guest-access.md).

* Brand Portal wird jetzt von AEM Assets Cloud Service unterstützt. Sie können AEM Assets Cloud Service mit Brand Portal konfigurieren, um Assets für Benutzer von Brand Portal freizugeben und zu verteilen.
Weitere Informationen finden Sie unter [Konfigurieren von AEM Assets Cloud Service mit Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html).

### Verbesserungen {#enhancements-646}

Diese Version von Brand Portal umfasst die folgenden Verbesserungen:

* In AEM 6.3 und höher wurde der Autorisierungskanal zwischen AEM Assets und Brand Portal geändert. AEM Assets wird jetzt mit Brand Portal über Adobe Devloper Console konfiguriert, die ein IMS-Token zur Authentifizierung Ihres Brand Portal-Mandanten abruft.

>[!NOTE]
>
>Die Konfiguration über das alte OAuth-Protokoll wird ab dem 6. April 2020 nicht mehr unterstützt, sondern erfolgt nun über Adobe Developer Console.

>[!TIP]
>
>***Nur für Bestandskunden***
>
>Die alte OAuth Gateway-Konfiguration funktioniert für bestehende Kunden weiterhin.
>
>Falls Probleme mit der alten OAuth-Gateway-Konfiguration auftreten, löschen Sie die vorhandene Konfiguration und erstellen Sie eine neue Konfiguration über Adobe Developer Console.

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

* Brand Portal-Benutzer können beim Aktualisieren auf Adobe Developer Console unter AEM 6.5.4 keine Beitragsordner-Assets in AEM Assets veröffentlichen.

   Dieses Problem wird mit dem nächsten Service Pack für AEM 6.5.5 behoben.

   Zur sofortigen Fehlerbehebung unter AEM 6.5.4 wird empfohlen, [den Hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) herunterzuladen und auf Ihrer Autoreninstanz zu installieren.

* Die Option „Systemausgaben ausschließen“ funktioniert beim Herunterladen eines Assets nicht ordnungsgemäß.


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

## Zertifizierte Plattformen            {#certified-platforms}

Informationen dazu, welche Plattformen für diese Version von Brand Portal zertifiziert sind, finden Sie in der Spalte **Unterstützung für Touch-optimierte Benutzeroberfläche** in der Tabelle im Bereich **Unterstützte Browser für die Autoren-Benutzeroberfläche** unter [Technische Anforderungen ](https://helpx.adobe.com/de/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Links {#links}

* [Adobe Experience Manager-Produktseite unter adobe.com](http://www.adobe.com/de/marketing-cloud/experience-manager.html)
* [Assets Brand Portal-Dokumentation](https://helpx.adobe.com/de/experience-manager/brand-portal/user-guide.html)

## Produktzugriff und Support (Websites mit Zugriffsbeschränkung) {#product-access-and-support-restricted-sites}

Diese Sites sind nur für Kunden verfügbar. Wenn Sie Kunde sind und Zugriff benötigen, wenden Sie sich an Ihren Adobe-Kundenbetreuer.

* [https://daycare.day.com](https://daycare.day.com)

* [Produktzugriff](https://login.marketing.adobe.com)

* [Adobe-Kundenunterstützung](https://helpx.adobe.com/de/contact.html)
