---
title: Verwalten der digitalen Rechte von Assets
seo-title: Verwalten der digitalen Rechte von Assets
description: Das Lizenzieren von Assets und das Festlegen eines Ablaufdatums für Assets und freigegebene Links ermöglichen eine kontrollierte Asset-Nutzung und den Schutz dieser Assets.
seo-description: Das Lizenzieren von Assets und das Festlegen eines Ablaufdatums für Assets und freigegebene Links ermöglichen eine kontrollierte Asset-Nutzung und den Schutz dieser Assets.
uuid: ce 30 e 398-0109-41 bf-a 4 d 2-2 fcca 476 f 499
contentOwner: bdhar
topic-tags: download-install
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: Referenz
discoiquuid: f 77003 ba -31 fe -4 a 9 e -96 c 8-dbc 4 c 2 eba 79 e
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Verwalten der digitalen Rechte von Assets {#manage-digital-rights-of-assets}

Eine sichere Verteilung und Nutzung von Kreativ-Assets und Markenmaterial ist für den Schutz Ihrer Marke wichtig. Dies kann innerhalb der Organisation und außerhalb der Organisation erzwungen werden, indem Sie ein Ablaufdatum (und eine Uhrzeit) mit genehmigten Assets verknüpfen, die von AEM in Brand Portal veröffentlicht wurden, oder indem Sie diese Assets zur bedingten Nutzung lizenzieren. Auch in Brand Portal können Sie ein Ablaufdatum für Links zu den Assets angeben, die über Brand Portal freigegeben werden.

Erfahren Sie, wie die Assets in Brand Portal gesichert werden und welche Nutzungsberechtigungen damit verknüpft sind.

## Asset-Ablauf {#asset-expiration}

Der Asset-Ablauf ist eine effektive Möglichkeit, die Nutzung der genehmigten Assets in Brand Portal unternehmensweit zu kontrollieren. Alle Assets, die von AEM Assets an Brand Portal veröffentlicht werden, können ein Ablaufdatum haben, das die Nutzung dieser Assets nach verschiedenen Benutzerrollen einschränkt.

### Nutzungsberechtigungen in Bezug auf abgelaufene Assets {#usage-permissions-expired-assets}

In Brand Portal können Administratoren abgelaufene Assets anzeigen, herunterladen und zu Sammlungen hinzufügen. Bearbeiter und Betrachter können dagegen nur abgelaufene Assets anzeigen und sie zu Sammlungen hinzufügen.

Administratoren können abgelaufene Assets aus AEM Assets in Brand Portal veröffentlichen. Abgelaufene Assets können jedoch nicht über einen Link aus Brand Portal freigegeben werden. If you select any expired asset from a folder containing both expired and non-expired assets, the **[!UICONTROL Share Link]** action is not available. Wenn Sie jedoch einen Ordner auswählen, der abgelaufene und nicht abgelaufene Assets enthält, sind die [!UICONTROL Aktionen "Freigeben] «und **[!UICONTROL " Verknüpfen"]** verfügbar.

>[!NOTE]
>
>Ein Ordner kann weiterhin als Link freigegeben werden, auch wenn er abgelaufene Assets enthält. In diesem Fall enthält der Link keine abgelaufenen Assets, und nur die nicht abgelaufenen Assets werden freigegeben.

In der folgenden Tabelle werden die Nutzungsberechtigungen der abgelaufenen Assets angezeigt:

|  | **[!UICONTROL Linkfreigabe]** | **[!UICONTROL Download]** | **[!UICONTROL Eigenschaften]** | **[!UICONTROL Zu Sammlung hinzufügen]** | **[!UICONTROL Löschen]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrator]** | Nicht verfügbar | Verfügbar | Verfügbar | Verfügbar | Verfügbar |
| **[!UICONTROL Bearbeiter]** | Nicht verfügbar | Nicht verfügbar | Verfügbar | Verfügbar | Nicht verfügbar |
| **[!UICONTROL Betrachter]** | Nicht verfügbar | Nicht verfügbar | Verfügbar | Verfügbar | Nicht verfügbar |
| **[!UICONTROL Gastbenutzer]** | Nicht verfügbar | Nicht verfügbar | Verfügbar | Verfügbar | Nicht verfügbar |

>[!NOTE]
>
>Wenn Viewer und Editors einen Ordner herunterladen, der abgelaufene und nicht abgelaufene Assets enthält, werden nur die nicht abgelaufenen Assets heruntergeladen. Wenn ein Ordner nur abgelaufene Assets enthält, wird ein leerer Ordner heruntergeladen.

### Gültigkeitsstatus und Assets {#expiration-status-of-assets}

You can view the expiration status of assets in their [!UICONTROL Card View]. Abgelaufene Assets sind mit einer roten Flagge gekennzeichnet.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>In den Listen- und Spaltenansichten wird der Gültigkeitsstatus der Assets nicht angezeigt.

## Ablauf des Asset-Links {#asset-link-expiration}

While sharing assets through links, Administrators and Editors can set a date and time of expiration using the **[!UICONTROL Expiration]** field in the **[!UICONTROL Link Sharing]** dialog box. Der Standardmäßige Link-Ablauf beträgt sieben Tage nach dem Datum der Freigabe des Links.

![](assets/asset-link-sharing.png)

So wird sichergestellt, dass Assets, die als Links freigegeben werden, an dem Tag und zu der Uhrzeit ablaufen, die Brand Portal-Administratoren und -Bearbeiter festgelegt haben. Nach diesem Ablaufdatum können sie nicht mehr angezeigt und heruntergeladen werden. Da die über Links freigegebenen Assets auch von externen Benutzern angesehen werden können, die nicht Teil des Unternehmens sind, können Sie durch Angabe von Ablauf sicherstellen, dass Ihre genehmigten Assets geschützt sind und nicht unbekannte Entitäten nach einer bestimmten Zeit offen gelegt werden.

For more information about link sharing, refer to [Share assets as a link](../using/brand-portal-link-share.md).

## Lizenzierte Assets {#licensed-assets}

Das Herunterladen von lizenzierten Assets aus Brand Portal unterliegt einer Lizenzvereinbarung. Diese Vereinbarung für lizenzierte Assets wird angezeigt, wenn Sie das Asset direkt aus Brand Portal oder über einen freigegebenen Link herunterladen. Abgelaufene oder nicht abgelaufene Assets, die durch eine Lizenz geschützt sind, können von allen Benutzern angezeigt werden. Jedoch ist der Download und die Verwendung von abgelaufenen genehmigten Assets begrenzt. Informationen zum Verhalten von abgelaufenen lizenzierten Assets und den zulässigen Aktivitäten basierend auf Benutzerrollen finden Sie unter [Nutzungsberechtigungen in Bezug auf abgelaufene Assets](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in AEM Assets.

If you choose to download license-protected asset(s), you are redirected to [!UICONTROL Copyright Management] page.

![](assets/asset-copyright-mgmt.png)

Hier müssen Sie das Asset auswählen, das Sie herunterladen möchten, und die zugehörige Lizenzvereinbarung annehmen. If you do not accept the license agreement, the [!UICONTROL Download] button is not enabled.

![](assets/licensed-asset-download-2.png)

Falls die Auswahl mehrere geschützte Assets enthält, wählen Sie jeweils eines aus, nehmen Sie die Lizenzvereinbarung an und fahren Sie mit dem Herunterladen des Assets fort.

## Erstellen von Berichten zu abgelaufenen Assets {#generate-report-about-expired-assets}

Administratoren können einen Bericht erstellen und herunterladen, in dem alle Assets aufgeführt sind, die innerhalb eines bestimmten Zeitraums abgelaufen sind. Dieser Bericht enthält detaillierte Informationen (z. B. Größe, Typ, Pfad für den Asset-Speicherort in der Asset-Hierarchie, wann das Asset abläuft) und wann das Asset veröffentlicht wurde - zu den abgelaufenen Assets. Die Spalten dieses Berichts können angepasst werden, um basierend auf den Benutzeranforderungen mehr Daten anzuzeigen.

![](assets/assets-expired.png)

For more information about the reports feature, refer [Work with reports](../using/brand-portal-reports.md#work-with-reports).
