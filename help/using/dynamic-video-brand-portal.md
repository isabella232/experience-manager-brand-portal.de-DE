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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Unterstützung dynamischer Videos in Brand Portal {#dynamic-video-support-on-brand-portal}

Preview and play videos adaptively on [!DNL Brand Portal] with Dynamic Media support. Laden Sie außerdem die dynamischen Darstellungen aus dem Portal und freigegebenen Links herunter.
[!DNL Brand Portal] Benutzer können:

* Vorschau von Videos auf der Seite „Asset-Details“, in der Kartenansicht und auf der Vorschauseite der Linkfreigabe
* Wiedergeben von Videokodierungen auf der Seite „Asset-Details“
* Anzeigen dynamischer Ausgabeformate auf der Registerkarte „Asset-Details“ der Seite „Asset-Details“
* Herunterladen von Videokodierungen und Ordnern mit Videos

>[!NOTE]
>
>To work with videos and to publish them to [!DNL Brand Portal], make sure that your [!DNL AEM] Author instance is set up either on Dynamic Media Hybrid mode or Dynamic Media [!DNL Scene 7] mode.

To preview, play, and download videos, [!DNL Brand Portal] exposes the following two configurations to administrators:

* [Hybrid-Media-Hybrid-Konfiguration](#configure-dm-hybrid-settings),
wenn [!DNL AEM] die Autoreninstanz im Hybrid-Modus der dynamischen Medien ausgeführt wird.
* [Dynamische Medien [! DNL Scene 7] Konfiguration](#configure-dm-scene7-settings)
wenn [!DNL AEM] die Autoreninstanz im dynamischen Medien-Modus[!DNL Scene 7] ausgeführt wird.
Set either of these configurations based on the configurations you set in your [!DNL AEM] Author instance with which [!DNL Brand Portal] tenant is replicated.

>[!NOTE]
>
>Dynamic videos are not supported on [!DNL Brand Portal] tenants integrated with [!DNL AEM] Author running on [!UICONTROL Scene7Connect] runmode.

## Wie werden dynamische Videos abgespielt? {#how-are-dynamic-videos-played}

![Videokodierungen werden aus der Cloud abgerufen.](assets/VideoEncodes.png)

If Dynamic Media configurations ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) or [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurations) are set up on [!DNL Brand Portal], the dynamic renditions are fetched from [!DNL Scene 7] server. Videokodierungen werden daher in einer Vorschau angezeigt und ohne Verzögerung und Qualitätsverluste wiedergegeben.

As video encodes are not stored in [!DNL Brand Portal] repository and are fetched from [!DNL Scene 7] server, ensure that the Dynamic Media configurations on [!DNL AEM] Author Instance and [!DNL Brand Portal] are the same.

>[!NOTE]
>
>Video viewers and viewer presets are not supported in [!DNL Brand Portal]. Videos are previewed and played on the default viewers in [!DNL Brand Portal].

## Voraussetzungen {#prerequisites}

To work with dynamic videos on [!DNL Brand Portal], make sure to:

* **Starten[!DNL AEM]Sie den Autor auf dem DM-Modus**
(dynamischer Medien) Starten Sie die [!DNL AEM] Instanz im Autorenmodus [!DNL Brand Portal] (mit integriertem Inhalt) entweder im [Hybrid-Modus](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) oder [dynamischen Medien [! DNL Scene 7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Konfigurieren Sie dynamische Mediendienste für dynamische Medien,[!DNL AEM]die auf dem**
Autor des dynamischen Medienmodus [!DNL AEM] basieren, oder setzen Sie eine der [dynamischen Mediencloud-Services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) oder [[! DNL Scene 7] Cloud-Services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) für [!DNL AEM] Authoring aus **Tools** | **Cloud Services** | **Dynamische Medien**.
* **Konfigurieren Sie dynamische Medien auf dem Markenportal**
basierend auf den Cloud-Konfigurationen für dynamische Medien im [!DNL AEM] Autor, konfigurieren [Sie dynamische Medieneinstellungen](#configure-dm-hybrid-settings) oder [[DNL Scene 7]-Einstellungen](#configure-dm-scene7-settings) aus [!DNL Brand Portal] Verwaltungstools.
Stellen Sie sicher, [dass separate [! DNL Brand Portal] Mandanten](#separate-tenants) werden für [!DNL AEM] Autoreninstanzen verwendet, die mit den Modi für dynamische Medien und dynamische Medien [!UICONTROL konfiguriert sind, wenn] Sie die Funktionen dynamischer Medien- und dynamischer Medien [!UICONTROL S 7 verwenden].
* **Veröffentlichen Sie Ordner mit Videokodierungen, die auf das Marken-Portal**
angewendet werden, [und](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) veröffentlichen Sie den Ordner, der Rich-Media-Assets aus [!DNL AEM] der Autoreninstanz enthält.[!DNL Brand Portal]
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

To ensure that your dynamic video assets are successfully previewed, played, and downloaded from [!DNL Brand Portal] (and shared links), follow these practices:

### Separate Mandanten für dynamische Medien- und Scene 7-Modi für dynamische Medien {#separate-tenants}

Wenn Sie die Funktionen für dynamische Medien [!DNL Scene 7] und dynamische Medien verwenden, wird empfohlen, verschiedene [!DNL Brand Portal] Mandanten für [!DNL AEM] die mit Dynamic Media-Hybrid- und dynamischen Medienmodi [!DNL Scene 7] konfigurierten Autoreninstanzen zu verwenden.
![Autoreninstanz und BP – 1:1-Zuordnung](assets/BPDynamicMedia.png)

### Gleiche Konfigurationsdetails in der AEM-Autoreninstanz und im Markenportal

Stellen Sie sicher, dass die Konfigurationsdetails - wie Titel, Registrierungs-ID, Video-Dienst-URL (in Dynamic Media Hybrid) und Title, die Anmeldeinformationen (E-Mail und Kennwort), Region, Firma (in dynamischen Medien [!DNL Scene 7]) in [!DNL Brand Portal] und [!DNL AEM] Cloud-Konfiguration identisch sind.

### Whitelist Public Egress ips für den Scene 7-Modus für dynamische Medien

Wenn für die Bereitstellung von Video-Assets auf dynamische Medien Scene 7- [sichere Vorschau aktiviert](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)wurde [!DNL Brand Portal], erstellt Scene 7 einen dedizierten Image-Server für Staging-Umgebungen oder interne Anwendungen. Mit einer beliebigen Anforderung an diesen Server wird die IP-Ursprungsadresse geprüft. Wenn die eingehende Anforderung nicht in der Liste genehmigter IP-Adressen enthalten ist, wird eine Fehlerantwort zurückgegeben.
Der Scene -7 Unternehmensadministrator konfiguriert daher eine genehmigte Liste von IP-Adressen für die Secure Testing-Umgebung ihres Unternehmens über SPS (Scene -7 Publishing System) Flash-Benutzeroberfläche. Stellen Sie sicher, dass die Egress-IP für Ihre jeweilige Region (siehe unten) in diese genehmigte Liste aufgenommen wird.
To whitelist either of these egress IPs, see [prepare your account for secure testing service](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Die egress ips lauten wie folgt:

| **Region** | **Egress-IP** |
|--- |--- |
| Nordamerika | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Konfigurieren von Dynamic Media (Hybrid)-Einstellungen {#configure-dm-hybrid-settings}

If [!DNL AEM] Author instance is running on dynamic media hybrid mode, then use Video tile from administrative tools panel to configure Dynamic Media gateway settings.
>[!NOTE]
>
>The [video encoding profiles](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) are not published to [!DNL Brand Portal], instead are fetched from the Scene 7 server. Therefore, for video encodes to be played successfully in [!DNL Brand Portal], ensure that the configuration details are the same as the [Scene7 cloud configuration](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in your [!DNL AEM] Author instance.
To set up Dynamic Media configurations on [!DNL Brand Portal] tenants:

1. Select the [!DNL AEM] logo to access administrative tools from the toolbar at the top, in [!DNL Brand Portal].

2. From the administrative tools panel, select the **Video** tile.
   ![Dynamic Media Hybrid-Konfiguration in Brand Portal](assets/DMHybrid-Video.png)
   **Die Seite "Dynamische Medienkonfiguration** bearbeiten" wird geöffnet.
   ![Dynamic Media Hybrid-Konfiguration in Brand Portal](assets/edit-dynamic-media-config.png)

3. Specify **Registration ID** and **Video Service URL** (DM-Gateway URL). Make sure these details are the same as those in **Tools** &gt; **Cloud Services** in your [!DNL AEM] Author instance.

4. Wählen Sie **Speichern** aus, um die Konfiguration zu speichern.

## Konfigurieren von Dynamic Media Scene 7-Einstellungen {#configure-dm-scene7-settings}

If [!DNL AEM] Author instance is running on Dynamic Media- [!UICONTROL Scene 7] mode, then use **Dynamic Media Configuration** tile from administrative tools panel to configure the [!UICONTROL Scene 7] server settings.

To set up Dynamic Media [!UICONTROL Scene 7] configurations on [!DNL Brand Portal] tenants:

1. Select the [!DNL AEM] logo to access administrative tools from the toolbar at the top, in [!DNL Brand Portal].

2. From the administrative tools panel, select the **Dynamic Media Configuration** tile.
   ![Die Konfiguration von DM Scene 7 auf der [!DNL Brand Portal]](assets/DMS7-Tile.png)Seite "Dynamische Medienkonfiguration bearbeiten" wird geöffnet.
   ![Scene 7-Konfiguration auf [!DNL Brand Portal]](assets/S7Config.png)

3. Geben Sie Folgendes an:
   * Titel
   * Anmeldedaten (E-Mail-ID und Kennwort) für den Zugriff auf den Scene 7-Server
   * Region
Make sure these values are the same as those in your [!DNL AEM] Author instance.

4. Wählen Sie **Mit Dynamic Media verbinden** aus.

5. Provide the **Company name**, and **Save** the configuration.
