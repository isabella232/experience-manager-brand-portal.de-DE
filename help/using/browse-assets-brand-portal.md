---
title: Durchsuchen von Assets in Brand Portal
seo-title: Durchsuchen von Assets in Brand Portal
description: Durchsuchen Sie Assets, navigieren Sie in Assethierarchien und suchen Sie nach Assets – mithilfe verschiedener Anzeigeoptionen und Benutzeroberflächen-Elemente in Brand Portal.
seo-description: Durchsuchen Sie Assets, navigieren Sie in Assethierarchien und suchen Sie nach Assets – mithilfe verschiedener Anzeigeoptionen und Benutzeroberflächen-Elemente in Brand Portal.
uuid: 178 ce 217-0050-4922-a 204-f 4539 d 46 f 539
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: Referenz
topic-tags: Einführung
discoiquuid: a 70 ce 694-81 d 1-4829-9 e 61-b 6412 e 013 e 5 c
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Durchsuchen von Assets in Brand Portal {#browsing-assets-on-brand-portal}

[!DNL AEM] Assets [! DNL Brand Portal bietet verschiedene Funktionen und Oberflächenelemente, mit denen Sie Ressourcen durchsuchen, Asset-Hierarchien durchsuchen und Assets durchsuchen können, während Sie verschiedene Ansichtsoptionen verwenden.

[!DNL AEM] logo in der [!DNL AEM] Symbolleiste oben erleichtert Administratoren den Zugriff auf das Bedienfeld für die Verwaltung von Administratoren.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Rail selector at the upper left in [!DNL Brand Portal] drops-down to expose options to navigate into asset hierarchies, streamline your search, and display resources.

![](assets/siderail-1.png)

You can view, navigate through, and select assets using any of the available views (Card, Column, and List) in the view selector at the upper right in [!DNL Brand Portal].

![](assets/viewselector.png)

## Anzeigen und Auswählen von Ressourcen {#viewing-and-selecting-resources}

Anzeige, Navigation und Auswahl sind grundsätzlich in allen Ansichten gleich. Je nach verwendeter Ansicht kommt es aber zu geringfügigen Abweichungen beim Umgang.

Sie können Ressourcen in jeder der verfügbaren Ansichten anzeigen, durchblättern und auswählen (für weitere Aktionen):

* Spaltenansicht
* Kartenansicht
* Listenansicht

### Kartenansicht

![](assets/card-view.png)

In der Kartenansicht werden Informationskarten für jedes Element auf der aktuellen Ebene angezeigt. Auf diesen Karten sind Die folgenden Details:

* eine visuelle Darstellung des Assets bzw. Ordners
* Typ
* Titel
* Name
* Datum und Uhrzeit, an dem bzw. zu der das Asset [!DNL Brand Portal] wurde von [!DNL AEM]
* Größe
* Dimensionen

You can navigate down the hierarchy by tapping/clicking cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### Kartenansicht für Benutzer ohne Administratorrechte

Karten von Ordnern in der Kartenansicht zeigen Ordnerhierarchie-Informationen an nicht-admin-Benutzer (Editor, Viewer und Gastbenutzer) an. Mit dieser Funktion können die Benutzer den Speicherort der Ordner kennen und auf die übergeordnete Hierarchie zugreifen.
Ordnerhierarchieinformationen sind besonders hilfreich, um die Ordner zu unterscheiden, deren Namen anderen Ordnern ähnlich sind, die in einer anderen Ordnerhierarchie freigegeben wurden. Wenn Benutzer ohne Administratorrechte nicht die Ordnerstruktur der für sie freigegebenen Assets berücksichtigen, können Assets bzw. Ordner mit denselben Namen für Verwirrung sorgen.

* Die auf den jeweiligen Karten angezeigten Pfade werden abgeschnitten, um sie an die Kartengrößen anzupassen. Benutzer können den vollständigen Pfad jedoch als quickinfo über den abgeschnittenen Pfad sehen.

![](assets/folder-hierarchy1.png)

**Option „Überblick“ zur Anzeige der Asset-Eigenschaften**

Die Option "Überblick" steht Benutzern ohne Administratorrechte (Editors, Viewer, Gäste) zur Verfügung, um Asset-Eigenschaften der ausgewählten Assets/Ordner anzuzeigen. Die Option „Überblick“ finden Sie an folgenden Stellen:

1. In der Symbolleiste am oberen Rand des ausgewählten Assets/Ordners
2. in der Dropdown-Liste des ausgewählten Leistenselektors

Bei Auswahl der Option „Überblick“ bei ausgewähltem Asset/Ordner können die Benutzer den Titel, den Pfad und den Zeitpunkt der Asset-Erstellung sehen. Wohingegen die Benutzer bei Auswahl der Option „Überblick“ auf der Asset-Detailseite die Metadaten des Assets sehen können.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### Anzeigeeinstellungen in der Kartenansicht

Das Dialogfeld „Anzeigeeinstellungen“ wird bei Auswahl der Option „Anzeigeeinstellungen“ im Ansichtselektor geöffnet. Damit können Sie die Größe der Asset-Miniaturansichten in der Kartenansicht ändern. Auf diese Weise können Sie Ihre Ansicht personalisieren und Einfluss auf die Anzahl der angezeigten Miniaturansichten nehmen.

![](assets/cardviewsettings.png)

### Listenansicht

![](assets/list-view.png)

In der Listenansicht werden Informationen für jede Ressource auf der aktuellen Ebene aufgelistet. In der Listenansicht werden die folgenden Details angezeigt:

* Miniaturbild der Assets
* Name
* Titel
* Gebietsschema
* Typ
* Dimension
* Größe
* Bewertung
* Ordnerpfad, der die Assethierarchie anzeigt<sup>*</sup>
* Datum der Veröffentlichung des Assets in Brand Portal

* Über die Spalte „Pfad“ können Sie die Position des Assets in der Ordnerhierarchie identifizieren. You can navigate down the hierarchy by tapping/clicking the resource name, and back up by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### Anzeigeeinstellungen in der Listenansicht

List view shows asset **Name** as the first column by default. Darüber hinaus werden weitere Informationen wie der Titel, das Gebietsschema, der Typ, die Dimensionen, die Größe, die Bewertung und der Veröffentlichungsstatus des Assets angezeigt. Sie können jedoch die anzuzeigenden Spalten über die Anzeigeeinstellungen auswählen.

![](assets/list-view-setting.png)

### Spaltenansicht

![](assets/column-view.png)

Navigieren Sie in der Spaltenansicht in der Inhaltsstruktur durch eine Reihe von kaskadierenden Spalten. Diese Ansicht hilft Ihnen, die Assethierarchie zu visualisieren und in ihr zu navigieren.

Durch die Auswahl einer Ressource in der ersten Spalte (ganz links) werden die untergeordneten Ressourcen in der zweiten Spalte rechts daneben angezeigt. Durch die Auswahl einer Ressource in der zweiten Spalte werden die untergeordneten Ressourcen in der dritten Spalte rechts daneben angezeigt usw.

Sie können in der Struktur nach oben und unten navigieren, indem Sie auf einen Ressourcennamen oder den Pfeil rechts vom Ressourcennamen tippen oder klicken.

* Beim Tippen bzw. Klicken werden der Ressourcenname und der Pfeil hervorgehoben.
* Durch Tippen oder Klicken auf die Miniaturansicht wird die Ressource ausgewählt.
* Wenn diese Option ausgewählt ist, wird ein Häkchen auf der Miniaturansicht angezeigt und der Ressourcenname wird hervorgehoben.
* Die Details der ausgewählten Ressource werden in der letzten Spalte angezeigt.

Wird ein Asset in der Spaltenansicht ausgewählt, wird die visuelle Darstellung des Assets in der letzten Spalte zusammen mit den folgenden Details angezeigt:

* Titel
* Name
* Dimensionen
* Date and time when asset was published to [!DNL Brand Portal] from [!DNL AEM]
* Größe
* Typ
* Option „Weitere Details“ zum Aufrufen der Seite „Details“ des Assets

<!--
Comment Type: draft

<h3>Selecting Resources</h3>
-->

<!--
Comment Type: draft

<p>Selecting a specific resource depends on a combination of the view and the device:</p>
-->

<!--
Comment Type: draft

<table border="1" cellpadding="1" cellspacing="0" width="100%">
<tbody>
<tr>
<td> </td>
<td>Select</td>
<td>Deselect</td>
</tr>
<tr>
<td>Column View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
<tr>
<td>Card View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap-and-hold the card</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the card</li>
<li>Mobile device:<br /> Tap the card</li>
</ul> </td>
</tr>
<tr>
<td>List View</td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
</tbody>
</table>
-->

<!--
Comment Type: draft

<h4>Deselecting All</h4>
-->

<!--
Comment Type: draft

<p>In all cases, as you select items the count of the items selected is displayed at the upper right of the toolbar.</p>
<p>You can deselect all items and exit selection mode by clicking or tapping the X next to the count.</p>
-->

<!--
Comment Type: draft

<p>In all views, all items can be deselected by tapping escape on the keyboard if you are using a desktop device.</p>
-->

## Inhaltsstruktur {#content-tree}

Verwenden Sie zusätzlich zu diesen Ansichten die Baumansicht, um die Asset-Hierarchie aufzuschlüsseln, während Sie die gewünschten Assets oder Ordner anzeigen und auswählen.

To open the tree view, tap/click the rail selector at upper left and select the **Content tree** from the menu.

![](assets/contenttree.png)

Navigieren Sie in der Inhaltshierarchie zum gewünschten Asset.

![](assets/content-tree.png)

## Asset-Details {#asset-details}

Auf der Seite „Details“ eines Assets können Sie das Asset anzeigen und herunterladen, einen Link zum Asset freigeben, das Asset in eine Sammlung verschieben oder dessen Seite „Eigenschaften“ anzeigen. Sie können nacheinander auch durch die Seite „Details“ anderer Assets im selben Ordner navigieren.

![](assets/asset-detail.png)

Zeigen Sie mithilfe des Leistenselektors auf der Seite „Details“ des Assets einen Überblick der Metadaten des Assets oder dessen zahlreiche Ausgabeformate an.

![](assets/asset-overview.png)

Sie können alle verfügbaren Ausgabeformate des Assets auf der Seite „Details“ des Assets anzeigen und ein Ausgabeformat zur Anzeige in der Vorschau auswählen.

![](assets/renditions.png)

To open the asset properties page, use *Properties (p)* option on the top bar.

![](assets/asset-properties.png)

You can also view a list of all its related assets (source or derived assets on AEM) on an asset's properties page, as asset relationship is also published from [!DNL AEM] to [!DNL Brand Portal].
