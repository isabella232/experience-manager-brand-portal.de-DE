---
title: Neue Funktionen in AEM Assets Brand Portal
seo-title: Neue Funktionen in AEM Assets Brand Portal
description: Informieren Sie sich über die neuen Funktionen und Verbesserungen in Version 6.4.4.
seo-description: Informieren Sie sich über die neuen Funktionen und Verbesserungen in Version 6.4.4.
uuid: 2 c 59 d 738-9 b 53-4 f 25-a 205-13 bf 75 c 80 b 77
contentOwner: bdhar
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: Referenz
topic-tags: Einführung
discoiquuid: fec 32 ca 3-142 b -4 a 11-9 b 92-5113 fc 27277 a
translation-type: tm+mt
source-git-commit: cbb64eb8a79480a1ccedbe5131a38ddf6eaec88d

---


# Neue Funktionen in AEM Assets Brand Portal {#what-s-new-in-aem-assets-brand-portal}

Mit Adobe Experience Manager (AEM) Assets Brand Portal können Sie mühelos kreative Assets erwerben, kontrollieren und sicher an externe Parteien und interne Geschäftsbenutzer geräteübergreifend verteilen. Brand Portal ermöglicht eine effizientere Asset-Freigabe, schnellere Time-to-Market für Assets sowie verringerte Risiken von Nicht-Compliance und unbefugten Zugriff. Adobe arbeitet an der Verbesserung des allgemeinen Brand Portal-Erlebnisses. Nachfolgend erfahren Sie, welche Funktionen und Erweiterungen eingeführt werden.

## Änderungen in 6.4.4 {#what-is-changing-in}

Version 6.4.4 von Brand Portal konzentriert sich auf Verbesserungen der Textsuche und von Kunden häufig gewünschte Funktionen. Siehe Aktuelle [Marken-Versionshinweise](brand-portal-release-notes.md).

### Verbesserungen der Suche {#search-enhancements}

Ab Version 6.4.4 unterstützt Brand Portal die Suche nach Textteilen über das Eigenschaftsprädikat im Filterbereich. To allow partial text search you need to enable **Partial Search** in Property Predicate in the search form.

Lesen Sie weiter, um mehr über die Suche nach Textteilen und Suche mit Platzhalter zu erfahren.

#### Suche nach Satzteilen {#partial-phrase-search}

Sie können nach Assets suchen, indem Sie nur einen Teil – d. h. ein oder zwei Wörter – des gesuchten Satzes in den Filterbereich eingeben.

**Anwendungsfall**
Die partielle Wortsuche ist hilfreich, wenn Sie nicht sicher sind, welche Kombination aus Wörtern in der gesuchten Wortgruppe aufgetreten ist.

Beispiel: Wenn Ihr Suchformular in Brand Portal das Eigenschaftsprädikat für Teilsuche nach einem Asset-Titel anwendet, werden nach Angabe des Begriffs **Lager** alle Assets mit dem Wort Lager im Titelsatz zurückgegeben.

![](assets/partialphrasesearch.png)

#### Suche mit Platzhalter {#wildcard-search}

Das Markenportal ermöglicht das Verwenden des Sternchens (*) in der Suchabfrage sowie einen Teil des Wortes in der gesuchten Wortgruppe.

**Anwendungsfall**
Wenn Sie sich nicht sicher sind, wie genau die Wörter in der gesuchten Wortgruppe sind, können Sie die Lücken in Ihrer Suchabfrage mit einer Platzhaltersuche ausfüllen.

For example, specifying **climb*** returns all the assets having words beginning with the characters **climb** in their title phrase if search form in Brand Portal uses Property Predicate for partial search on assets title.

![](assets/wildcard-prop.png)

Auch gilt Folgendes:

* *** skaliert** alle Assets, die mit Zeichen enden, die mit Zeichen **enden, in** deren Titelleiste.

* *** climb *** gibt alle Assets zurück, die die Zeichen mit **den** Zeichen aus der Titelleiste zusammenführen.

>[!NOTE]
>
>Nach Aktivierung des Kontrollkästchens **Teilsuche** wird **Groß-/Kleinschreibung ignorieren** standardmäßig aktiviert.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## Änderungen in 6.4.3 {#what-changed-in}

Version 6.4.3 von Brand Portal bietet Unternehmen neben der Mandanten-ID einen alternativen Alias für die Brand Portal-Zugriffs-URL, eine neue Ordnerhierarchiekonfiguration, Verbesserungen bei der Videounterstützung, die geplante Veröffentlichung aus der AEM-Autoreninstanz in Brand Portal, betriebliche Verbesserungen und die Umsetzung von Kundenwünschen.

### Ordnerhierarchienavigation für Benutzer ohne Administratorrechte

Administratoren können jetzt konfigurieren, wie Ordner für Benutzer ohne Administratorrechte (Bearbeiter, Betrachter und Gastbenutzer) bei der Anmeldung angezeigt werden. [Die Konfiguration der Ordnerhierarchie](../using/brand-portal-general-configuration.md) wird in **den allgemeinen Einstellungen** im Bereich admin tools hinzugefügt. Wenn die Konfiguration:

* **aktiviert** ist, ist die Ordnerstruktur ab dem Stammordner für Nicht-Administratoren sichtbar. Sie können also genauso wie Administratoren navigieren.
* **deaktiviert** sind, werden nur die freigegebenen Ordner auf der Einstiegsseite angezeigt.

![](assets/enable-folder-hierarchy.png)
**Der Anwendungsfall**

The [Enable Folder Hierarchy](../using/brand-portal-general-configuration.md) functionality (when enabled) helps you differentiate the folders with the same names shared from different hierarchies. Bei der Anmeldung sehen Nicht-Administratoren nun die virtuellen übergeordneten (und untergeordneten) Ordner der freigegebenen Ordner.
![](assets/disabled-folder-hierarchy1-2.png) ![](assets/enabled-hierarchy1-2.png)

Die freigegebenen Ordner werden innerhalb der jeweiligen Verzeichnisse in virtuellen Ordnern angeordnet. Sie können diese virtuellen Ordner an einem Schlosssymbol erkennen.

Beachten Sie, dass das Standardminiaturbild der virtuellen Ordner das Miniaturbild des ersten freigegebenen Ordners ist.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### Suche in einer bestimmten Ordnerhierarchie oder in einem bestimmten Ordnerpfad

**Das Pfadbrowser** -Prädikatzeichen wird im Suchformular eingeführt, um die Suche nach Assets in einem bestimmten Verzeichnis zuzulassen. The default search path of search predicate for Path Browser is */content/dam/mac/&lt;tenant-id&gt;/*, which can be configured by editing the default search form.

* Administratoren können über den Pfadbrowser zu einem beliebigen Verzeichnis in Brand Portal navigieren.
* Benutzer ohne Administratorrechte können mithilfe des Pfadbrowsers nur zu den Ordnern navigieren (und zurück zu den übergeordneten Ordnern navigieren), die für sie freigegeben wurden.
Beispielsweise wird */content/dam/mac/ &lt; tenant-id &gt;/foldera/folderc/folderc* für einen Benutzer ohne Administratorrechte freigegeben. Der Benutzer kann mithilfe des Pfadbrowsers innerhalb von folderc nach Assets suchen. Dieser Benutzer kann auch zu folderb und foldera navigieren (da es sich um Vorgänger des Ordners handelt, der für den Benutzer freigegeben ist).

![](assets/edit-search-form.png)

**Der Anwendungsfall**

Sie können die Asset-Suche nun in einem bestimmten Ordner einschränken, zu dem Sie navigiert sind, anstatt die Einschränkung angefangen beim Stammordner anzuwenden.

Beachten Sie, dass die Suche in diesen Ordnern nur Suchergebnisse aus Assets zurückgibt, die für den Benutzer freigegeben wurden.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Unterstützung von Dynamic Media-Videowiedergaben

Benutzer, deren AEM-Autoreninstanz sich im Hybrid-Hybrid-Hybrid-Modus befindet, können die dynamischen Medienwiedergaben zusätzlich zu den ursprünglichen Videodateien in der Vorschau anzeigen und herunterladen.

To allow preview and download of dynamic media renditions on specific tenant accounts, administrators need to specify **Dynamic Media Configuration** (video service URL (DM-Gateway URL) and registration ID to fetch the dynamic video) in **Video** configuration from admin tools panel.

**Die Anwendungsfälle**
dynamischer Medien können in der Vorschau angezeigt werden:

* Asset-Detailseite
* Asset-Kartenansicht
* Linkfreigabe-Vorschauseite

Dynamic Media-Videokodierungen können heruntergeladen werden über:

* Brand Portal
* Freigegebenen Link

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Geplante Veröffentlichung in Brand Portal

Assets (and folders) publish workflow from [AEM (6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) Author instance to Brand Portal can be scheduled for a later date, time.

Entsprechend können veröffentlichte Assets zu einem späteren Zeitpunkt aus dem Portal entfernt werden, indem der Workflow zum Rückgängigmachen der Veröffentlichung in Brand Portal geplant wird.

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Konfigurierbarer Mandantenalias in URL

Unternehmen können ihre Portal-URL mit einem alternativen Präfix in der URL anpassen. Um einen Alias für einen Mandantenamen in der vorhandenen Portal-URL zu erhalten, müssen Unternehmen sich mit dem Adobe-Support in Verbindung setzen.

Beachten Sie, dass nur das Präfix der Brand Portal-URL angepasst werden kann und nicht die gesamte URL.\
For example, an organization with existing domain **geomettrix.brand-portal.adobe.com** can get **geomettrixinc.brand-portal.adobe.com** created on request.

Eine AEM-Autoreninstanz kann jedoch nur mit der Mandanten-ID-URL [konfiguriert](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) werden und nicht mit einer (alternativen) Mandantenalias-URL.

**Der Anwendungsfall**
Unternehmen können ihre Branding-Anforderungen erfüllen, indem sie ihre Portal-URL anpassen, anstatt die von Adobe bereitgestellte URL beizubehalten.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Optimierter Download

In Adobe Experience Manager Assets Brand Portal 6.4.3 wurde der Download vereinfacht, sodass in den folgenden Situationen weniger Klicks notwendig sind und weniger Warnungen angezeigt werden:

* Entscheidung, dass nur die Wiedergaben heruntergeladen werden (und nicht die Original-Assets).
* Herunterladen der Assets, wenn der Zugriff auf die Originalwiedergaben eingeschränkt ist.

## Änderungen in 6.4.2 {#what-changed-in-1}

Die Markenversion von Brand Portal 6.4.2 bietet eine Reihe von Funktionen, die den Anforderungen an die Verteilung von Assets gerecht werden und ihnen helfen, eine große Anzahl an Benutzern zu erreichen, die global über den Gastriffzugriff und die optimale Nutzung mit beschleunigten Downloads verteilt sind. Darüber hinaus bietet Brand Portal Organisationen durch neue Konfigurationsoptionen für Administratoren, einen neu hinzugefügten Bericht und bessere Berücksichtigung von Kundenanforderungen eine größere Kontrolle.

### Gastzugang

![](assets/bp-login-screen-1.png)

AEM Brand Portal gestattet den Gastzugang für das Portal. Ein Gastbenutzer benötigt keine Anmeldeinformationen, um das Portal aufzurufen, und kann auf sämtliche öffentliche Ordner und Sammlungen zugreifen und diese herunterladen. Gastbenutzer können Assets zu ihrer Lightbox (private Sammlung) hinzufügen und diese herunterladen. Sie können Smart-Tag-basierte Suchen und Sucheigenschaften, die von Administratoren festgelegt wurden, anzeigen. Die Gastsitzung gestattet es Benutzern jedoch nicht, Sammlungen und gespeicherte Suchen zu erstellen oder weiter freizugeben, auf die Einstellungen für Ordner und Sammlungen zuzugreifen und Assets als Links freizugeben.

In einer Organisation sind mehrere gleichzeitige Gastsitzungen zulässig, deren Zahl ist jedoch auf 10 % des Gesamtbenutzerkontingents pro Organisation beschränkt.

Eine Gastsitzung bleibt für 2 Stunden aktiv. Infolgedessen wird der Status der Lightbox auch bis 2 Stunden nach Beginn der Sitzung beibehalten. Nach 2 Stunden muss die Gastsitzung neu gestartet werden, d. h. der Lightbox-Status geht verloren.

### Beschleunigte Downloads

Brand Portal-Benutzer können mit der IBM Aspera Connect-basierten Downloadbeschleunigung – unabhängig von ihrem globalen Standort – bis zu 25-mal höhere Geschwindigkeiten und eine unterbrechungsfreie Download-Performance erzielen. Um Assets schneller aus Brand Portal oder über den freigegebenen Link herunterzuladen, müssen Benutzer die Option **Downloadbeschleunigung aktivieren** im Dialogfeld „Herunterladen“ auswählen, sofern die Downloadbeschleunigung im Unternehmen aktiviert ist.

![](assets/donload-assets-dialog-2.png)

To enable IBM Aspera based accelerated download for the organization, administrators **Enable Download Acceleration** option (which is disabled by default) from [General Settings](brand-portal-general-configuration.md#allow-download-acceleration) in the administrative tools panel. Weitere Informationen zu den Voraussetzungen und den Schritten zur Fehlerbehebung bei Problemen mit dem schnelleren Download von Asset-Dateien von Brand Portal und über freigegebene Links finden Sie unter [Anleitung zum Beschleunigen von Downloads von Brand Portal](../using/accelerated-download.md#main-pars-header).

### Bericht „Benutzeranmeldungen“

Es wurde ein neuer Bericht zum Nachverfolgen von Benutzeranmeldungen eingeführt. Der Bericht **Benutzeranmeldungen** bietet Organisationen die Möglichkeit, die delegierten Administratoren und andere Benutzer von Brand Portal zu überwachen und zu kontrollieren.

Der Bericht protokolliert Anzeigenamen, E-Email-IDs, Mitarbeiter (Admin, Viewer, Editor, Gast), Gruppen, letzte Anmeldung, Aktivitätsstatus und Anmeldenählungen der einzelnen Benutzer aus der Markenoberfläche von Brand Portal 6.4.2 bis zum Zeitpunkt der Berichtgenerierung. Administratoren können den Bericht als .csv-Datei exportieren. Der Bericht „Benutzeranmeldungen“ gestattet in Verbindung mit anderen Berichten eine genauere Überwachung der Benutzerinteraktionen mit den genehmigten Brand-Ressourcen und gewährleistet so die Einhaltung von Vorschriften der Corporate Compliance Offices.

![](assets/user-logins-1.png)

### Zugriff auf die Original-Ausgabeformate

Administratoren können den Zugriff auf die Original-Bilddateien (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) einschränken und Zugriff auf Wiedergaben mit einer niedrigen Auflösung erteilen, die aus Brand Portal oder über einen freigegebenen Link heruntergeladen werden. Dieser Zugriff kann auf Benutzergruppenebene über die Registerkarte „Gruppen“ auf der Seite „Benutzerrollen“ im Admin Tools-Bereich gesteuert werden.

![](assets/access-original-rend-1.png)

* Standardmäßig können alle Benutzer Originaldarstellungen herunterladen, da der Zugriff auf Original für alle aktiviert ist.
* Administratoren müssen die Auswahl der entsprechenden Kontrollkästchen deaktivieren, um zu verhindern, dass eine Gruppe von Benutzern auf Original-Ausgabeformate zugreift.
* Falls ein Benutzer Mitglied mehrerer Gruppen ist, eine dieser Gruppen aber über Einschränkungen verfügt, gelten die Einschränkungen für diesen Benutzer.
* Die Einschränkungen gelten nicht für Administratoren, auch wenn sie Mitglieder von eingeschränkten Gruppen sind.
* Berechtigungen der Benutzer, die Assets gemeinsam verwenden, gelten für Benutzer, die Assets mit freigegebenen Links herunterladen.

### Ordnerhierarchiepfad in Karten- und Listenansichten

Karten von Ordnern in der Kartenansicht zeigen jetzt Ordnerhierarchieinformationen an nicht-admin-Benutzer (Editor, Viewer und Gastbenutzer) an. Mit dieser Funktion können die Benutzer den Speicherort der Ordner kennen und auf die übergeordnete Hierarchie zugreifen.

Ordnerhierarchieinformationen sind besonders hilfreich, um die Ordner zu unterscheiden, deren Namen anderen Ordnern ähnlich sind, die in einer anderen Ordnerhierarchie freigegeben wurden. Wenn Benutzer ohne Administratorrechte nicht die Ordnerstruktur der für sie freigegebenen Assets berücksichtigen, können Assets bzw. Ordner mit denselben Namen für Verwirrung sorgen.

* Die auf den jeweiligen Karten angezeigten Pfade werden abgeschnitten, um sie an die Kartengrößen anzupassen. Benutzer können den vollständigen Pfad jedoch als quickinfo beim Bewegen des Mauszeigers über den abgeschnittenen Pfad sehen.

![](assets/folder-hierarchy1-1.png)

In der Listenansicht wird der Ordnerpfad der Assets in einer Spalte für alle Benutzer von Brand Portal angezeigt.

![](assets/list-view-1.png)

### Option „Überblick“ zur Anzeige der Asset-Eigenschaften

Brand Portal stellt Benutzern ohne Administratorrechte (Bearbeitern, Betrachtern, Gastbenutzern) mit der Option Überblick eine Funktion zum Anzeigen von Asset-Eigenschaften von ausgewählten Assets/Ordnern bereit. Die Option „Überblick“ finden Sie an folgenden Stellen:

1. In der Symbolleiste am oberen Rand des ausgewählten Assets/Ordners
2. in der Dropdown-Liste des ausgewählten Leistenselektors

Bei Auswahl der Option „Überblick“ bei ausgewähltem Asset/Ordner können die Benutzer den Titel, den Pfad und den Zeitpunkt der Asset-Erstellung sehen. Wohingegen die Benutzer bei Auswahl der Option „Überblick“ auf der Asset-Detailseite die Metadaten des Assets sehen können.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## Neue Konfigurationen

Es wurden sechs neue Konfigurationen hinzugefügt, damit Administratoren folgende Funktionen für bestimmte Mandanten aktivieren bzw. deaktivieren können:

* Gastzugang zulassen
* Zugriffsanfrage für Brand Portal durch Benutzer erlauben
* Löschen von Assets von Brand Portal durch Administratoren zulassen
* Erstellung öffentlicher Sammlungen zulassen
* Erstellung öffentlicher Smart-Sammlungen zulassen
* Downloadbeschleunigung aktivieren

Die zuvor genannten Konfigurationen sind unter Zugriffseinstellungen und Allgemeine Einstellungen im Admin Tools-Bereich verfügbar.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Adobe.io hostet die Benutzeroberfläche zum Konfigurieren von oAuth-Integrationen

Brand Portal 6.4.2 onwards uses Adobe.io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) interface to create JWT application, which enables configuring oAuth integrations to allow AEM Assets integration with Brand Portal. Previously, the UI for configuring OAuth integrations was hosted in [https://marketing.adobe.com/developer/](https://marketing.adobe.com/developer/). To know more about integrating AEM Assets with Brand Portal for publishing assets and collections to Brand Portal refer [Configure AEM Assets integration with Brand Portal](https://helpx.adobe.com/in/experience-manager/6-4/assets/using/brand-portal-configuring-integration.html).

## Verbesserungen der Suche

Administratoren können die Eigenschaft für die Nichtgroß-/Kleinschreibung anhand der aktualisierten Eigenschaftsprädikate verwenden, die eine Prüfung auf Schreibweise ignorieren hat. Die Option ist für Eigenschaftsprädikat und für Eigenschaftsprädikat mit mehreren Werten verfügbar.\
Eine Suche, bei der nicht zwischen Groß- und Kleinschreibung unterschieden wird, ist vergleichsweise langsamer als die Standardsuche nach Eigenschaftsprädikat. Wenn im Suchfilter zu viele nichtgroß-/kleinschreibung berücksichtigt werden, kann die Suche verlangsamt werden. Daher ist es ratsam, Suchen, bei denen nicht zwischen Groß- und Kleinschreibung unterschieden wird, umsichtig zu verwenden.

## Änderungen in 6.4.1 {#what-changed-in-2}

Brand Portal 6.4.1 ist eine Plattform-Upgrade-Version, die mehrere neue Funktionen und wichtige Erweiterungen bei den Funktionen zum Durchsuchen und Suchen sowie Performancesteigerungen mit sich bringt, um die Bereitstellung herausragender Kundenerlebnisse zu ermöglichen.

### Erweiterte Funktionen zum Durchsuchen

* Neue Inhaltsstrukturleiste zur schnellen Navigation in Asset-Hierarchien.

![](assets/contenttree-2.png)

* Introduced new keyboard shortcuts, for example _(p)_ for navigation to properties page, _(e)_ for Edit, and _(ctrl+c)_ for copy operations.
* Verbesserte Scrollfunktion, Lazy-Loading-Erlebnis in der Karten- und Listenansicht beim Durchsuchen einer großen Anzahl von Elementen.
* Erweiterte Kartenansicht mit Unterstützung für unterschiedlich große Karten basierend auf der Anzeigeeinstellung.

![](assets/cardviewsettings-1.png)

* Kartenansicht zeigt jetzt beim Bewegen des Mauszeigers über der Datumsangabe einen Datums-/Zeitstempel an.

* Enhanced Column view with **More Details** under the asset snapshot, which lets you navigate to details page of an asset.

![](assets/columnmoredetail.png)

* Die Listenansicht zeigt jetzt Dateinamen der Assets in der ersten Spalte standardmäßig zusätzlich zu Gebietsschema, Asset-Typ, Dimensionen, Größe, Bewertung und Veröffentlichungsinformationen an. New **View Settings** can be used to configure the amount of detail to display in List view.

* Verbessertes Asset-Detailerlebnis mit der Möglichkeit, mit neuen Navigationsschaltflächen zwischen Assets vor und zurück zu wechseln, und mit Anzeige der Asset-Anzahl.

![](assets/navbtn.png)

* Neue Möglichkeit zur Vorschau von Audio-Dateien, die aus AEM hochgeladen wurden, in der Detailseite des jeweiligen Assets.
* Neue Funktion „Zugehörige Assets“ auf der Seite „Asset-Eigenschaften“. Assets, die mit anderen Quell-/abgeleiteten Assets auf AEM im Zusammenhang stehen und auf dem Markenportal veröffentlicht werden, haben jetzt die Beziehung in Brand Portal mit Verknüpfungen zu den zugehörigen Assets auf der Eigenschaftenseite.
* Neue Konfiguration verhindert, dass Nicht-Administrator-Benutzer öffentliche Sammlungen erstellen können. Organisationen können mit dem Adobe Support Team zusammenarbeiten, um diese Funktion für bestimmte Konten zu konfigurieren.

### Verbesserungen der Suche

* Die Fähigkeit, nach dem Navigieren zu einem Suchelement zu der gleichen Position in den Suchergebnissen zurückzukehren, ohne die Suchabfrage erneut auszuführen.
* Neuer Zähler für Suchergebnisse, um die Anzahl der Suchergebnisse anzuzeigen.
* Verbesserter Suchfilter für Dateitypen mit der Möglichkeit, Suchergebnisse basierend auf differenzierten MIME-Typen wie .jpg, .png und .psd zu filtern, anstatt die bisherigen Optionen wie Bilder, Dokumente, Multimedia zu verwenden.
* Erweiterter Suchfilter für Sammlungen mit genauen Zeitstempeln anstelle der bisherigen Zeitschiebereglerfunktion.
* Neue Filter für Zugriffstyp zum Suchen nach öffentlichen bzw. nicht-öffentlichen Sammlungen.

![](assets/accesstypefilter.png)

### Download-Optimierungen

* Eine einzelne große Datei wird direkt heruntergeladen, ohne dass die ZIP-Datei erstellt wird, wodurch die Geschwindigkeit und der Durchsatz verbessert werden.
* Die maximale Größe für ZIP-Downloads bei der Linkfreigabe wurde von 1 GB auf 5 GB erhöht.

* Benutzer können beim Herunterladen von Assets aus Brand Portal oder über freigegebene Links jetzt auswählen, ob sie nur die benutzerdefinierten oder die ursprünglichen Dateien, und vermeiden Sie vordefinierte Darstellungen, während Sie Assets aus dem Markenportal oder über die Funktion für freigegebene Links herunterladen.

![](assets/excludeautorendition.png)

### Performancesteigerung

* Bis zu 100 % höhere Asset-Downloadgeschwindigkeit
* Bis zu 40 % schnellere Reaktion bei der Asset-Suche
* Bis zu 40 % bessere Browser-Leistung

**Hinweis:** Die genannten Verbesserungen wurden bei Tests in einem Labor gemessen.

### Erweiterte Berichterstellungsfunktionen

**Neuer Bericht zur Linkfreigabe**
Ein neuer Bericht wurde eingeführt, der Informationen zu freigegebenen Links bereitstellt. Der Bericht zur Linkfreigabe führt alle URLs zu Assets auf, die für interne und externe Benutzer im Unternehmen innerhalb des festgelegten Zeitrahmens freigegeben wurden. Zusätzlich enthält der Bericht Informationen zum Zeitpunkt der Linkfreigabe und zu dessen Ablaufdatum sowie dazu, wer den Link freigegeben hat.

![](assets/navigatereport.png)

**Einstiegspunkt für den Zugriff auf den Verwendungsbericht geändert**
Der Verwendungsbericht wurde jetzt mit anderen Berichten konsolidiert und kann von der Konsole „Asset-Berichte“ angezeigt werden. To reach Asset Reports console, navigate to **Create/Manage Reports** from administrative tools panel.

![](assets/accessassetreport.png)

**Verbesserte Benutzererfahrung mit**der Berichterstellungsschnittstelle
auf dem Markenportal wurde intuitiver und übersichtlicher. Administratoren können nicht mehr nur verschiedene Berichte erstellen, sondern auch zuvor generierte Berichte erneut aufrufen und diese herunterladen oder löschen, da sie in Brand Portal gespeichert sind.

Alle Berichte können durch das Hinzufügen oder Entfernen standardmäßiger Spalten angepasst werden. Zudem können für die Berichte „Download“, „Ablauf“ und „Veröffentlichen“ benutzerdefinierte Spalten hinzugefügt werden, um den Detailgrad anzupassen.

### Verbesserte Admin Tools

Verbesserte Eigenschaftenauswahl in den Admin Tools für Metadaten, Suche und Berichte mit Vervollständigungs- und Suchfunktion, um die Abläufe für Administratoren zu vereinfachen

### Weitere Verbesserungen

* Assets, die in Brand Portal über AEM 6.3.2.1 und 6.4 veröffentlicht wurden, können jetzt für allgemeine Benutzer von Brand Portal veröffentlicht werden, indem Sie das Kontrollkästchen "Veröffentlichen des öffentlichen Ordners" im Dialogfeld" Replizierungsverfahren für AEM Assets Brand Portal" markieren.

![](assets/public-folder-publish.png)

* Wenn Benutzer Zugriff auf Brand Portal anfragen, erhalten Administratoren zusätzlich zur Benachrichtigung im Brand Portal-Benachrichtigungsbereich eine E-Mail über die Zugriffsanforderung.

## Änderungen in 6.3.2 {#what-changed-in-3}

Brand Portal 6.3.2 enthält neue und erweiterte Funktionen, die die wichtigsten Kundenanfragen erfüllen und eine allgemeine Performancesteigerung bringen.

### Anfordern von Zugriff auf Brand Portal {#request-access-to-brand-portal}

Benutzer können jetzt den Zugriff auf Brand Portal über die neue**** erforderliche Zugriffsberechtigung anfordern, die auf dem Anmeldebildschirm von Brand Portal verfügbar ist.

![](assets/bplogin_request_access.png)

Je nachdem, ob die Benutzer bereits eine Adobe ID haben oder zuerst eine Adobe ID erstellen müssen, können die Benutzer den entsprechenden Arbeitsablauf für die Anfrage befolgen. Brand Portal-Produkt-Administratoren werden in ihrem Benachrichtigungsbereich über diese Anfragen informiert und gewähren den Zugriff über Adobe Admin Console.

Weitere Informationen finden Sie unter [Anfordern von Zugriff auf Brand Portal](../using/brand-portal.md#requestaccesstobrandportal).

### Erweiterung des Berichts über heruntergeladene Assets {#enhancement-in-the-assets-downloaded-report}

Der Bericht über heruntergeladene Assets zeigt jetzt an, wie viele Assets die einzelnen Benutzer innerhalb eines bestimmten Zeitraums heruntergeladen haben. Benutzer können diesen Bericht im CSV-Format herunterladen und Daten zur Gesamtanzahl der Downloads für ein lizenziertes Asset zusammenstellen.

![](assets/reports_download_downloaded_by.png)

Weitere Informationen finden Sie in Schritt 3 und 6 unter [Erstellen und Verwalten weiterer Berichte](../using/brand-portal-reports.md#createandmanageadditionalreports).

### Wartungsbenachrichtigung in Brand Portal {#brand-portal-maintenance-notification}

Brand Portal zeigt jetzt einige Tage vor geplanten Wartungsaktivitäten ein entsprechendes Benachrichtigungsbanner an. Beispiel für eine Benachrichtigung:

![](assets/bp_maintenance_notification-1.png)

For more information, see [Brand Portal maintenance notification](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification).

### Erweiterungen für lizenzierte Assets, die über die Funktion „Asset-Freigabe“ freigegeben werden {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

Beim Herunterladen lizenzierter Assets mit der Funktion „Asset-Freigabe“ werden Sie jetzt aufgefordert, der Lizenzvereinbarung für diese Assets zuzustimmen.

![](assets/copyright_management.png)

For more information, see Step 12 in [Share assets as a link](../using/brand-portal-link-share.md#shareassetsasalink).

### Erweiterung der Funktion zur Benutzerauswahl {#user-picker-enhancement}

Die Funktion zur Benutzerauswahl wurde jetzt verbessert, um den Anforderungen von Kunden mit großen Benutzerzahlen gerecht zu werden.

### Änderungen beim Experience Cloud-Branding {#experience-cloud-branding-changes}

Brand Portal ist jetzt mit dem neuen Adobe Experience Cloud-Branding konform.

![](assets/bp_solution_switcher.png)

## Änderungen in 6.3.1 {#what-changed-in-4}

Brand Portal 6.3.1 enthält neue und erweiterte Funktionen, die die Abstimmung von Brand Portal mit AEM verbessern.

### Aktualisierte Benutzeroberfläche {#upgraded-user-interface}

Um das Brand Portal-Benutzererlebnis an AEM anzupassen, vollzieht Adobe einen Übergang zur Coral 3-Benutzeroberfläche. Durch diese Änderung wird die allgemeine Benutzerfreundlichkeit, einschließlich Navigation und Darstellung, verbessert.

#### Erweiterte Funktionen für die Navigation {#enhanced-navigational-experience}

* Schnellzugriff auf Admin Tools über das neue Adobe-Logo:

![](assets/aemlogo-3.png)

* Produktnavigation mithilfe einer Überlagerung:

![](assets/overlay_navigation.png)

* Schnellnavigation zu übergeordneten Ordnern:

![](assets/navigationparentfolders.png)

* Schnellsuche und Navigation zu erforderlichen Inhalten und Tools:

![](assets/omnisearchicon.png)

### Erweiterte Funktionen zum Durchsuchen {#enhanced-browsing-experience}

* Neue Spaltenansicht zum Durchsuchen verschachtelter Ordner:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* In der Liste der Assets in einem Ordner wird das zuletzt hochgeladene Asset oben angezeigt.

### Erweiterte Funktionen zum Suchen {#enhanced-search-experience}

* Die neue Omni-Suchfunktion ermöglicht mithilfe automatischer Vorschläge beim Eingeben der Suchschlüsselwörter den schnellen Zugriff auf relevante Inhalte, Funktionen oder Tags. Die Omni-Suche ist für alle Suchfunktionen verfügbar:

![](assets/omnisearch_whatsnew.png)

* Sie können außerdem Suchfilter zur Omni-Suche hinzufügen, um die Suche weiter einzugrenzen und zu beschleunigen.

![](assets/omnisearch_withfilters.png)

* Dank der neuen auf Asset-Bewertungen basierenden Suche können Sie anhand der in AEM Assets veröffentlichten Bewertungen (sofern verfügbar) nach Assets suchen.
* Die neue Suchfunktion für mehrere Werte akzeptiert die Eingabe mehrerer Suchbegriffe mit dem Operator UND, um die Suche zu beschleunigen.
* Durch die neue Suchoptimierungsfunktion können Sie die Relevanz der Suchergebnisse verbessern, sodass bestimmte Assets in den Suchergebnissen oben angezeigt werden.
* Die neue pfadbasierte Suche ermöglicht die Angabe eines Pfads zu einem verschachtelten Ordner, damit Sie nach Assets in diesem Ordner suchen können.

#### Neue Smart-Tag-basierte Suche {#new-smart-tags-based-search}

Wenn Bilder mit Smart-Tags aus AEM Assets in Brand Portal veröffentlicht werden, können Sie in Brand Portal anhand der Smart-Tag-Namen als Suchschlüsselwörter nach diesen Bildern suchen. Diese Funktion ist nur für Dateien verfügbar.

### Erweiterte Funktionen für Downloads {#enhanced-downloading-experience}

Nach dem Herunterladen eines verschachtelten Ordners können Sie die ursprüngliche Ordnerhierarchie beibehalten. Die Assets in einem verschachtelten Ordner können in einem Ordner heruntergeladen werden. Das Heruntergeladen in separaten Ordnern ist nicht mehr erforderlich.

### Verbesserte Leistung {#improved-performance}

Die Erweiterungen der Funktionen zum Durchsuchen, Suchen und Herunterladen verbessern die Brand Portal-Leistung erheblich.

### Neues Digital Rights Management für Assets {#new-digital-rights-management-for-assets}

Administratoren können vor der Freigabe von Assets Datum und Uhrzeit als Ablaufdatum festlegen. Abgelaufene Assets sind für Betrachter und Bearbeiter sichtbar, können aber nicht mehr heruntergeladen werden. Administratoren erhalten eine Benachrichtigung über abgelaufene Assets.

### Erweiterte Asset-Sortierung {#enhanced-asset-sorting}

Die Asset-Sortierung in einem Ordner in der Listenansicht ist nicht mehr auf die Anzahl der Assets auf der ersten Seite beschränkt. Stattdessen werden alle Assets sortiert, unabhängig davon, ob sie auf der ersten Seite angezeigt werden.

### Erweiterte Berichterstellung {#reporting-capabilities}

Administratoren können drei Berichtstypen erstellen und verwalten – zu heruntergeladenen, abgelaufenen und veröffentlichten Assets. Zudem können die Spalten im Bericht konfiguriert und die Berichte als CSV-Datei exportiert werden.

![](assets/newreport.png)

### Zusätzliche Metadaten {#additional-metadata}

Brand Portal 6.3.1 führt zusätzliche Metadaten ein, die auch in AEM Assets 6.3 enthalten sind. Die Metadaten, die auf der Seite „Asset-Eigenschaften“ angezeigt werden, können mit dem Metadatenschema-Editor festlegt werden. Asset-Metadaten sind nicht für Benutzer sichtbar, die Assets als Freigabe über einen externen Link erhalten und die Assets nur mithilfe der Linkfreigabe-URL in der Vorschau anzeigen sowie herunterladen können.

![](assets/additionsinmetadata.png)

### Weitere Funktionen für Administratoren {#additional-capabilities-for-administrators}

* Vor dem Abschließen der Anpassungen für den Anmeldebildschirm-Hintergrund können Administratoren die Änderungen in der Vorschau anzeigen.

![](assets/wallpaperpreview.png)

* Wenn ein Administrator neue Benutzer zum Brand Portal-Konto hinzugefügt hat, müssen diese keine Einladungen annehmen, um zu Brand Portal hinzugefügt zu werden. Das Hinzufügen erfolgt automatisch.

### Neue Veröffentlichungsfunktionen in AEM Assets 6.3 {#new-publishing-capabilities-in-aem-assets}

* AEM-Administratoren können mithilfe von AEM 6.3 SP 1-CFP 1 (6.3.1.1) (ab 4. Quartal 2017 verfügbar) Metadatenschemata aus AEM Assets in Brand Portal veröffentlichen.

![](assets/publish_metadataschemaaemassets.png)

* AEM-Administratoren können alle Tags aus AEM Assets on Brand Portal mithilfe von AEM 6.2 SP 1 - CFP 7 und AEM 6.3 SP 1-CFP 1 (6.3.1.1) veröffentlichen.

![](assets/publish_tags_aemassets.png)

* Sie können aus AEM Assets Sammlungen und Assets veröffentlichen, die Tags (einschließlich Smart-Tags) enthalten. Sie können diese Tags anschließend als Suchschlüsselwörter verwenden, um in Brand Portal nach diesen Sammlungen und Assets zu suchen.

## Häufig gestellte Fragen {#frequently-asked-questions}

**Qus. Verliere ich den Zugriff auf vorhandene Assets, Funktionen oder Konfigurationen, die ich erstellt habe?****Ans.** Alle bestehenden Funktionen und Konfigurationen stehen weiterhin zur Verfügung. Es gibt keine Auswirkungen auf Ihre Endbenutzer und Ihre Inhalte bleiben unverändert.

**Ques. Wann findet der Wechsel zur neuen Brand Portal-Version statt?****Ans.** Markenportal 6.4.4 wurde im Februar 2019 zur Produktion freigegeben. Die nächste Brand Portal-Version wird voraussichtlich im 3. Quartal 2019 veröffentlicht.

>[!NOTE]
>
>Der Veröffentlichungszeitplan ist vorläufig und kann jederzeit geändert werden. Wenden Sie sich an Ihren Adobe-Kundenbetreuer oder den Kundensupport, um aktuelle Informationen zum Veröffentlichungszeitplan zu erhalten.

**Ques. Wie sind die Auswirkungen auf meine Benutzer?****Ans.** Dieser Wechsel findet ausschließlich in Brand Portal statt, sodass Ihre Endbenutzer keine Auswirkungen feststellen.

**Ques. Sind von meiner Seite Schritte erforderlich?****Ans.** Administratoren müssen keine Aktionen durchführen. Sobald Sie Zugriff auf das neue Brand Portal haben, finden Sie in der Dokumentation alle wichtigen Informationen und Neuigkeiten.

**Ques. An wen kann ich mich bei Fragen wenden?****Ans.** Kontaktieren Sie Ihren Adobe-Kundenbetreuer oder den Kundensupport.
