---
title: Unterstützung dynamischer Videos in Brand Portal
seo-title: Unterstützung dynamischer Videos in Brand Portal
description: Unterstützung dynamischer Videos in Brand Portal
seo-description: Unterstützung dynamischer Videos in Brand Portal
uuid: a 3502 a 4 d -3971-4 ea 4-953 c -44 ba 04446269
contentOwner: mgulati
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: Referenz
topic-tags: download-install
discoiquuid: e 18 d 992 a-a 3 b 5-45 f 2-9696-8161993213 ee
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Unterstützung dynamischer Videos in Brand Portal {#dynamic-video-support-on-brand-portal}

Profitieren Sie von einer Vorschau und adaptiven Wiedergabe von Videos in Brand Portal mit Dynamic Media-Unterstützung. Laden Sie außerdem die dynamischen Darstellungen aus dem Portal und freigegebenen Links herunter.
Brand Portal-Benutzer haben folgende Möglichkeiten:

* Vorschau von Videos auf der Seite „Asset-Details“, in der Kartenansicht und auf der Vorschauseite der Linkfreigabe
* Wiedergeben von Videokodierungen auf der Seite „Asset-Details“
* Anzeigen dynamischer Ausgabeformate auf der Registerkarte „Asset-Details“ der Seite „Asset-Details“
* Herunterladen von Videokodierungen und Ordnern mit Videos

>[!NOTE]
>
>To work with videos and to publish them to Brand Portal, make sure that your AEM Author instance is set up either on Dynamic Media Hybrid mode or Dynamic Media [!DNL Scene 7] mode.

Um Videos in einer Vorschau anzeigen, diese wiederzugeben und herunterzuladen, stellt Brand Portal die beiden folgenden Konfigurationen für Administratoren bereit:

* [Hybridkonfiguration](#configure-dm-hybrid-settings)
für dynamische Medien, wenn die AEM-Autoreninstanz im Hybrid-Modus für dynamische Medien ausgeführt wird.
* [Dynamische Medien [! DNL Scene 7] Konfiguration](#configure-dm-scene7-settings)
wenn AEM Author-Instanz im dynamischen Medien-Modus[!DNL Scene 7] ausgeführt wird.
Legen Sie eine dieser Konfigurationen basierend auf den Konfigurationen fest, die Sie in Ihrer AEM-Autoreninstanz festgelegt haben, mit der der Brand Portal-Mandant repliziert wird.

>[!NOTE]
>
>Dynamic videos are not supported on Brand Portal tenants integrated with AEM Author running on [!UICONTROL Scene7Connect] runmode.

## Wie werden dynamische Videos abgespielt? {#how-are-dynamic-videos-played}

![Videokodierungen werden aus der Cloud abgerufen.](assets/VideoEncodes.png)

If Dynamic Media configurations ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) or [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurations) are set up on Brand Portal, the dynamic renditions are fetched from [!DNL Scene 7] server. Videokodierungen werden daher in einer Vorschau angezeigt und ohne Verzögerung und Qualitätsverluste wiedergegeben.

As video encodes are not stored in Brand Portal repository and are fetched from [!DNL Scene 7] server, ensure that the Dynamic Media configurations on AEM Author Instance and Brand Portal are the same.

>[!NOTE]
>
>Video Viewer und Viewer-Voreinstellungen werden in Brand Portal nicht unterstützt. Videos werden in den Standard-Viewern in Brand Portal als Vorschau angezeigt und abgespielt.

## Voraussetzungen {#prerequisites}

Um mit dynamischen Videos in Brand Portal zu arbeiten, müssen Sie Folgendes sicherstellen:

* **Starten Sie AEM Author on DM (Dynamic Media)-Modus**
Starten Sie die AEM-Autoreninstanz (mit integriertem Brand Portal) entweder im [Hybrid-Media-Hybrid](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) - oder [dynamischen Medien [! DNL Scene 7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Konfigurieren Sie die Dynamic Media Cloud-Dienste auf dem AEM-Autor**
basierend auf dem dynamischen Medienmodus, auf dem AEM Author ausgeführt wird, und legen Sie eine der [Cloud-Services für dynamische Medien](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) oder [[! DNL Scene 7] Cloud Services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in AEM Author aus **Tools** | **Cloud Services** | **Dynamische Medien**.
* **Konfigurieren Sie dynamische Medien auf dem Markenportal**
basierend auf den Cloud-Konfigurationen für dynamische Medien auf AEM Author, konfigurieren [Sie dynamische Medieneinstellungen](#configure-dm-hybrid-settings) oder [[DNL Scene 7]-Einstellungen](#configure-dm-scene7-settings) aus den Verwaltungstools von Marken Portal.
Make sure that [separate Brand Portal tenants](#separate-tenants) are used for AEM Author instances configured with Dynamic Media Hybrid and Dynamic Media [!UICONTROL Scene7] modes, if you are using functionalities of Dynamic Media Hybrid and Dynamic Media [!UICONTROL S7].
* **Veröffentlichen Sie Ordner mit Videokodierungen, die auf das Marken-Portal**
 [angewendet werden, und](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) veröffentlichen Sie den Ordner, der Rich Media-Assets aus der AEM-Autoreninstanz in Brand Portal enthält.
* **Whitelist Egress ips in SPS, wenn die sichere Vorschau aktiviert**
ist Bei Verwendung dynamischer Medien ([!DNL Scene 7] mit [aktivierter Vorschau für](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) ein Unternehmen) wird diesem [!DNL Scene 7] Unternehmensadministrator [empfohlen, die öffentlichen Epress-ips](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) für bestimmte Regionen in der Flash-Benutzeroberfläche von SPS ([!UICONTROL Scene 7] Publishing System) zu verwenden.
Die Egress-IPs lauten wie folgt:

| **Region** | **Egress-IP** |
|--- |--- |
| Nordamerika | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

To whitelist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best Practices

Um sicherzustellen, dass Ihre dynamischen Video-Assets erfolgreich in einer Vorschau angezeigt, wiedergegeben und aus Brand Portal (und den freigegebenen Links) heruntergeladen werden, gehen Sie wie folgt vor:

### Separate Mandanten für dynamische Medien- und Scene 7-Modi für dynamische Medien {#separate-tenants}

Wenn Sie die Funktionen für dynamische Medien [!DNL Scene 7] und dynamische Medien verwenden, wird empfohlen, dass Sie verschiedene Marken-Portal-Mandanten für AEM Author-Instanzen verwenden, die mit Hybrid-Media-Hybrid- und dynamischen Medienmodi [!DNL Scene 7] konfiguriert wurden.
![Autoreninstanz und BP – 1:1-Zuordnung](assets/BPDynamicMedia.png)

### Gleiche Konfigurationsdetails in der AEM-Autoreninstanz und im Markenportal

Ensure that the configuration details–such as [!UICONTROL Title], [!UICONTROL Registration ID], [!UICONTROL Video Service URL] (in [!UICONTROL Dynamic Media Hybrid]) and [!UICONTROL Title], credentials ([!UICONTROL Email] and Password), [!UICONTROL Region], [!UICONTROL Company] (in Dynamic Media [!DNL Scene 7])–are the same in Brand Portal and [!UICONTROL AEM cloud configuration].

### Whitelist Public Egress ips für den Scene 7-Modus für dynamische Medien

Wenn für die Bereitstellung von Video-Assets auf Brand Portal aktiviert ist, wenn Scene 7 [!UICONTROL -Scene 7]-kompatible Vorschau aktiviert [](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)ist, erstellt [!UICONTROL Scene 7] einen dedizierten Image-Server für Staging-Umgebungen oder interne Anwendungen. Mit einer beliebigen Anforderung an diesen Server wird die IP-Ursprungsadresse geprüft. Wenn die eingehende Anforderung nicht in der Liste genehmigter IP-Adressen enthalten ist, wird eine Fehlerantwort zurückgegeben.
The [!UICONTROL Scene-7] Company Administrator, therefore, configures an approved list of IP addresses for their company’s [!UICONTROL Secure Testing] environment, through [!UICONTROL SPS] (Scene-7 Publishing System) flash UI. Stellen Sie sicher, dass die Egress-IP für Ihre jeweilige Region (siehe unten) in diese genehmigte Liste aufgenommen wird.
To whitelist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Die egress ips lauten wie folgt:

| **Region** | **Egress-IP** |
|--- |--- |
| Nordamerika | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Konfigurieren von Dynamic Media (Hybrid)-Einstellungen {#configure-dm-hybrid-settings}

If AEM Author instance is running on dynamic media hybrid mode, then use [!UICONTROL Video] tile from administrative tools panel to configure Dynamic Media gateway settings.
>[!NOTE]
>
>The [video encoding profiles](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) are not published to Brand Portal, instead are fetched from the [!UICONTROL Scene 7] server. Therefore, for video encodes to be played successfully in Brand Portal, ensure that the configuration details are the same as the [[!UICONTROL Scene7 cloud configuration]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in your AEM Author instance.
So richten Sie Dynamic Media-Konfigurationen für Brand Portal-Mandanten ein:

1. Wählen Sie in Brand Portal in der Symbolleiste am oberen Rand das AEM-Logo aus, um die Admin Tools aufzurufen.

2. From the administrative tools panel, select the **[!UICONTROL Video]** tile.

![Dynamic Media Hybrid-Konfiguration in Brand Portal](assets/DMHybrid-Video.png)

**[!UICONTROL Die Seite "Dynamische Medienkonfiguration]** bearbeiten" wird geöffnet.

![Dynamic Media Hybrid-Konfiguration in Brand Portal](assets/edit-dynamic-media-config.png)

3. Specify **[!UICONTROL Registration ID]** and **[!UICONTROL Video Service URL]** (DM-Gateway URL). Stellen Sie sicher, dass diese Details mit denen unter **[!UICONTROL Tools &gt; Cloud-Services]in Ihrer AEM-Autoreninstanz übereinstimmen.**

4. Wählen Sie **Speichern** aus, um die Konfiguration zu speichern.

## Konfigurieren von Dynamic Media Scene 7-Einstellungen {#configure-dm-scene7-settings}

If AEM Author instance is running on Dynamic Media- [!UICONTROL Scene 7] mode, then use **[!UICONTROL Dynamic Media Configuration]** tile from administrative tools panel to configure the [!UICONTROL Scene 7] server settings.

To set up Dynamic Media [!UICONTROL Scene 7] configurations on Brand Portal tenants:

1. Wählen Sie in Brand Portal in der Symbolleiste am oberen Rand das AEM-Logo aus, um die Admin Tools aufzurufen.

2. From the administrative tools panel, select the **[!UICONTROL Dynamic Media Configuration]** tile.
   ![[!UICONTROL DM Scene 7-Konfiguration in Brand Portal]](assets/DMS7-Tile.png)

[!UICONTROL Die Seite "Dynamische Medienkonfiguration] bearbeiten" wird geöffnet.

![Scene 7-Konfiguration in Brand Portal](assets/S7Config.png)

3. Geben Sie Folgendes an:
   * [!UICONTROL Titel]
   * Credentials ([!UICONTROL Email ID] and [!UICONTROL Password]) to access the Scene 7 server
   * [!UICONTROL Region]Stellen Sie
sicher, dass diese Werte denen in Ihrer AEM-Autoreninstanz entsprechen.

4. Wählen Sie **[!UICONTROL Mit Dynamic Media verbinden aus]**.

5. Provide the **[!UICONTROL Company name]**, and **[!UICONTROL Save]** the configuration.
