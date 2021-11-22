---
title: Unterstützung für Dynamic Video in Brand Portal
seo-title: Dynamic video support on Brand Portal
description: Unterstützung für Dynamic Video in Brand Portal
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: 7128c71576ae938a49f9bff0b95b98b7fc480f69
workflow-type: tm+mt
source-wordcount: '1256'
ht-degree: 55%

---

# Unterstützung für Dynamic Video in Brand Portal {#dynamic-video-support-on-brand-portal}

Profitieren Sie von einer Vorschau und adaptiven Wiedergabe von Videos in Brand Portal mit Dynamic Media-Unterstützung. Laden Sie auch die dynamischen Ausgabedarstellungen aus dem Portal und von freigegebenen Links herunter.
Brand Portal-Benutzer haben folgende Möglichkeiten:

* Vorschau von Videos auf der Seite „Asset-Details“, in der Kartenansicht und auf der Vorschauseite der Linkfreigabe
* Wiedergeben von Videokodierungen auf der Seite „Asset-Details“
* Anzeigen dynamischer Ausgabedarstellungen auf der Registerkarte „Asset-Details“ der Seite „Asset-Details“
* Herunterladen von Videokodierungen und Ordnern mit Videos

>[!NOTE]
>
>Um mit Videos zu arbeiten und sie in Brand Portal zu veröffentlichen, stellen Sie sicher, dass die Experience Manager-Autoreninstanz entweder im Dynamic Media Hybrid-Modus oder im Dynamic Media **[!DNL Scene7]**-Modus.

Um Videos in einer Vorschau anzeigen, diese wiederzugeben und herunterzuladen, stellt Brand Portal die beiden folgenden Konfigurationen für Administratoren bereit:

* [Dynamic Media Hybrid-Konfiguration](#configure-dm-hybrid-settings)
Wenn die Experience Manager-Autoreninstanz im Dynamic Media Hybrid-Modus ausgeführt wird.
* [Dynamic Media  [!DNL Scene7] -Konfiguration](#configure-dm-scene7-settings)
Wenn die Experience Manager-Autoreninstanz im Dynamic Media **[!DNL Scene7]**-Modus ausgeführt wird.
Legen Sie eine dieser Konfigurationen basierend auf den Konfigurationen fest, die Sie in Ihrer Experience Manager-Autoreninstanz festgelegt haben, mit der der Brand Portal-Mandant repliziert wird.

>[!NOTE]
>
>Dynamische Videos werden nicht für Brand Portal-Mandanten unterstützt, die mit der Experience Manager-Autoreninstanz konfiguriert sind und auf der **[!UICONTROL Scene7Connect]** Ausführungsmodus.

## Wie wird Dynamic Video abgespielt? {#how-are-dynamic-videos-played}

![Videokodierungen werden aus der Cloud abgerufen.](assets/VideoEncodes.png)

Wenn Dynamic Media-Konfigurationen ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings)- oder [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)-Konfigurationen) in Brand Portal eingerichtet werden, werden die dynamischen Ausgabedarstellungen vom **[!DNL Scene7]**-Server abgerufen. Videokodierungen werden daher in einer Vorschau angezeigt und ohne Verzögerung und Qualitätsverluste wiedergegeben.

Da Videokodierungen nicht im Brand Portal-Repository gespeichert und von abgerufen werden **[!DNL Scene7]** stellen Sie sicher, dass die Dynamic Media-Konfigurationen in der Adobe Experience Manager-Autoreninstanz und in Brand Portal identisch sind.

>[!NOTE]
>
>Video Viewer und Viewer-Voreinstellungen werden in Brand Portal nicht unterstützt. Videos werden in den Standard-Viewern in Brand Portal als Vorschau angezeigt und abgespielt.

## Voraussetzungen {#prerequisites}

Um mit Dynamic Video in Brand Portal zu arbeiten, müssen Sie Folgendes sicherstellen:

* **Starten Sie die Experience Manager-Autoreninstanz im Dynamic Media-Modus.**
Starten Sie die Experience Manager-Autoreninstanz (mit der Brand Portal konfiguriert ist) entweder in [Dynamic Media - [!DNL Scene7] mode](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) oder [Dynamic Media - Hybridmodus](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=de) oder
* **Konfigurieren von Dynamic Media Cloud Services in Experience Manager Author**
Basierend auf dem Dynamic Media-Modus (Scene7-Modus oder Hybridmodus), auf dem der Experience Manager-Autor ausgeführt wird, legen Sie entweder [Dynamic Media Cloud Services ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) oder [Dynamic Media Cloud Services (Hybridmodus)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) zum Experience Manager-Autor von **Instrumente** | **Cloud Services** | **Dynamic Media**.
* **Konfigurieren von Dynamic Media auf Brand Portal**
Konfigurieren Sie basierend auf den Dynamic Media-Cloud-Konfigurationen in Experience Manager Author [Dynamic Media-Einstellungen](#configure-dm-hybrid-settings) oder [[!DNL Scene7] settings](#configure-dm-scene7-settings)  aus den Verwaltungstools von Brand Portal.
Stellen Sie sicher, dass [separate Brand Portal-Mandanten](#separate-tenants) werden für Experience Manager-Autoreninstanzen verwendet, die in Dynamic Media konfiguriert sind - **[!UICONTROL Scene7]** Modus und Dynamic Media - Hybridmodus. Insbesondere bei Verwendung von Funktionen von Dynamic Media **[!UICONTROL S7]** und Dynamic Media Hybrid.
* **Veröffentlichen von Ordnern mit auf Brand Portal angewendeten Videokodierungen**
Anwenden [Videokodierungen](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html?lang=de) und veröffentlichen Sie den Ordner mit Rich-Media-Assets aus der Experience Manager-Autoreninstanz in Brand Portal.
* **Setzen Sie Egress-IPs in SPS auf die Allowlist, wenn die sichere Vorschau aktiviert ist.**
Bei der Nutzung von Dynamic Media-**[!DNL Scene7]** (mit [aktivierter sicherer Vorschau](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html?lang=de) für ein Unternehmen) wird empfohlen, dass der **[!DNL Scene7]** -Unternehmens-Administrator [die öffentlichen Egress-IPs auf die Zulassungsliste setzt](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html?lang=de#testing-the-secure-testing-service). Dies erfolgt für die betreffenden Regionen mittels der SPS (**[!UICONTROL Scene7]** Publishing System)-Flash-Benutzeroberfläche.
Die Egress-IPs lauten wie folgt:

| **Region** | **Egress-IP** |
|--- |--- |
| nicht vorhanden | 130.248.160.68,  20.94.203.130 |
| EMEA | 185.34.189.3,  51.132.146.75 |
| APAC | 63.140.44.54 |

Informationen zum Hinzufügen einer dieser Egress-IPs zur Zulassungsliste finden Sie unter [Vorbereiten Ihres Kontos für sicheres Testen](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best Practices

Um sicherzustellen, dass Ihre Dynamic Video-Assets erfolgreich in einer Vorschau angezeigt, wiedergegeben und aus Brand Portal (und den freigegebenen Links) heruntergeladen werden, gehen Sie wie folgt vor:

### Separate Mandanten für den Dynamic Media - Scene7 und Dynamic Media - Hybridmodus {#separate-tenants}

Wenn Sie beide Dynamic Media verwenden: **[!DNL Scene7]** -Modus und Dynamic Media - Hybridmodus-Funktionen verwenden verschiedene Brand Portal-Mandanten für Experience Manager-Autoreninstanzen, die mit Dynamic Media konfiguriert wurden - **[!DNL Scene7]** und Dynamic Media - Hybridmodus.


![Autoreninstanz und BP – 1:1-Zuordnung](assets/BPDynamicMedia.png)

### Gleiche Konfigurationsdetails in der Experience Manager-Autoreninstanz und Brand Portal

Stellen Sie sicher, dass die Konfigurationsdetails in Brand Portal identisch sind und **[!UICONTROL Experience Manager Cloud-Konfiguration]**. Dieselben Konfigurationsdetails umfassen Folgendes:

* **[!UICONTROL Titel]**
* **[!UICONTROL Registrierungs-ID]**
* **[!UICONTROL Videodienst-URL]** in **[!UICONTROL Dynamic Media - Hybridmodus]**
* **[!UICONTROL Titel]**
* Anmeldeinformationen (**[!UICONTROL Email]** und Kennwort)
* **[!UICONTROL Region]**
* **[!UICONTROL Firma]** in Dynamic Media - **[!DNL Scene7]** mode

### Öffentliche Ausgangs-IPs für den Dynamic Media Scene7-Modus auf die Zulassungsliste setzen

Wenn Dynamic Media **[!UICONTROL Scene7]** mit aktivierter [sicherer Vorschau](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) genutzt wird, um Video-Assets für Brand Portal bereitzustellen, richtet **[!UICONTROL Scene7]** einen dedizierten Image-Server für Staging-Umgebungen oder interne Anwendungen ein. Mit einer beliebigen Anforderung an diesen Server wird die IP-Ursprungsadresse geprüft. Wenn die eingehende Anforderung nicht in der Liste genehmigter IP-Adressen enthalten ist, wird eine Fehlerantwort zurückgegeben.
Die **[!UICONTROL Scene7]** Der Unternehmensadministrator konfiguriert daher eine Liste genehmigter IP-Adressen für die **[!UICONTROL Sichere Tests]** -Umgebung durch **[!UICONTROL SPS]** Flash-Benutzeroberfläche (Scene7 Publishing System). Stellen Sie sicher, dass die Egress-IP für Ihre jeweilige Region (siehe unten) in diese genehmigte Liste aufgenommen wird.
Informationen zum Hinzufügen einer dieser Egress-IPs zur Zulassungsliste finden Sie unter [Vorbereiten Ihres Kontos für sicheres Testen](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Die Egress-IPs lauten wie folgt:

| **Region** | **Egress-IP** |
|--- |--- |
| nicht vorhanden | 130.248.160.66,  52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63 140 44 54 |

## Konfigurieren von Dynamic Media (Hybrid)-Einstellungen {#configure-dm-hybrid-settings}

Wenn die Experience Manager-Autoreninstanz im Dynamic Media-Hybridmodus ausgeführt wird, verwenden Sie **[!UICONTROL Video]** Kachel im Admin Tools-Bereich zum Konfigurieren der Dynamic Media-Gateway-Einstellungen.

>[!NOTE]
>
>Die [Videokodierungsprofile](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) werden nicht in Brand Portal veröffentlicht, sondern vom **[!UICONTROL Scene7]**-Server abgerufen. Damit Videokodierungen erfolgreich in Brand Portal wiedergegeben werden können, müssen Sie daher sicherstellen, dass die Konfigurationsdetails mit den [Dynamic Media Cloud Services ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) in Ihrer Experience Manager-Autoreninstanz.

So richten Sie Dynamic Media-Konfigurationen für Brand Portal-Mandanten ein:

1. Wählen Sie das Experience Manager-Logo aus, damit Sie über die Symbolleiste oben in Brand Portal auf die Admin Tools zugreifen können.
1. Wählen Sie im Admin-Tools-Bereich die Kachel **[!UICONTROL Video]** aus.

   ![Dynamic Media-Hybrid-Konfiguration in Brand Portal](assets/DMHybrid-Video.png)

   Die Seite **[!UICONTROL Konfiguration für Dynamic Media bearbeiten]** wird geöffnet.

   ![Dynamic Media-Hybrid-Konfiguration in Brand Portal](assets/edit-dynamic-media-config.png)

1. Geben Sie die **[!UICONTROL Registrations-ID]** und **[!UICONTROL die Video Service-URL]** (DM-Gateway URL) an. Stellen Sie sicher, dass diese Details mit denen unter **[!UICONTROL Tools > Cloud Services]** in Ihrer Experience Manager-Autoreninstanz.
1. Wählen Sie **Speichern** aus, um die Konfiguration zu speichern.

## Konfigurieren von Dynamic Media Scene7-Einstellungen {#configure-dm-scene7-settings}

Wenn die Experience Manager-Autoreninstanz auf Dynamic Media ausgeführt wird - **[!UICONTROL Scene7]** -Modus und verwenden Sie dann **[!UICONTROL Dynamic Media-Konfiguration]** Kachel im Admin Tools-Bereich zum Konfigurieren **[!UICONTROL Scene7]** Servereinstellungen.

Gehen Sie wie folgt vor, um Dynamic Media **[!UICONTROL Scene7]**-Konfigurationen für Brand Portal-Mandanten einzurichten:

1. Wählen Sie das Experience Manager-Logo aus, damit Sie über die Symbolleiste oben in Brand Portal auf die Admin Tools zugreifen können.

2. Wählen Sie im Admin-Tools-Bereich die Kachel **[!UICONTROL Dynamic Media-Konfiguration]** aus.

   ![DM [!UICONTROL Scene7]-Konfiguration in Brand Portal](assets/DMS7-Tile.png)

   Die Seite **[!UICONTROL Konfiguration für Dynamic Media bearbeiten]** wird geöffnet.

   ![Scene7-Konfiguration in Brand Portal](assets/S7Config.png)

3. Geben Sie Folgendes an:

   * **[!UICONTROL Titel]**
   * Anmeldedaten (**[!UICONTROL E-Mail-ID]** und **[!UICONTROL Passwort]**) für den Zugriff auf den Scene7-Server
   * **[!UICONTROL Region]**

   Stellen Sie sicher, dass diese Werte mit den Werten in Ihrer Experience Manager-Autoreninstanz übereinstimmen.

4. Wählen Sie **[!UICONTROL Mit Dynamic Media verbinden]** aus.

5. Geben Sie den **[!UICONTROL Unternehmensnamen]** an und **[!UICONTROL speichern]** Sie die Konfiguration.
