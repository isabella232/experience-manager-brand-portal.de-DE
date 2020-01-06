---
title: Unterstützung für Dynamic Video in Brand Portal
seo-title: Unterstützung für Dynamic Video in Brand Portal
description: Unterstützung für Dynamic Video in Brand Portal
seo-description: Unterstützung für Dynamic Video in Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Unterstützung für Dynamic Video in Brand Portal {#dynamic-video-support-on-brand-portal}

Profitieren Sie von einer Vorschau und adaptiven Wiedergabe von Videos in Brand Portal mit Dynamic Media-Unterstützung. Laden Sie auch die dynamischen Ausgabeformate aus dem Portal und von freigegebenen Links herunter.
Brand Portal-Benutzer haben folgende Möglichkeiten:

* Vorschau von Videos auf der Seite „Asset-Details“, in der Kartenansicht und auf der Vorschauseite der Linkfreigabe
* Wiedergeben von Videokodierungen auf der Seite „Asset-Details“
* Anzeigen dynamischer Ausgabeformate auf der Registerkarte „Asset-Details“ der Seite „Asset-Details“
* Herunterladen von Videokodierungen und Ordnern mit Videos

>[!NOTE]
>
>Um mit Videos zu arbeiten und sie in Brand Portal zu veröffentlichen, stellen Sie sicher, dass die AEM-Autoreninstanz entweder im Dynamic Media Hybrid-Modus oder im Dynamic Media **[!DNL Scene 7]**-Modus.

Um Videos in einer Vorschau anzeigen, diese wiederzugeben und herunterzuladen, stellt Brand Portal die beiden folgenden Konfigurationen für Administratoren bereit:

* [Dynamic Media Hybrid-Konfiguration](#configure-dm-hybrid-settings)
Wenn die AEM-Autoreninstanz im Dynamic Media Hybrid-Modus ausgeführt wird.
* [Dynamic Media [!DNL Scene 7]-Konfiguration](#configure-dm-scene7-settings)
Wenn die AEM-Autoreninstanz im Dynamic Media-**[!DNL Scene 7]**-Modus ausgeführt wird.
Legen Sie eine dieser Konfigurationen basierend auf den Konfigurationen fest, die Sie in Ihrer AEM-Autoreninstanz festgelegt haben, mit der der Brand Portal-Mandant repliziert wird.

>[!NOTE]
>
>Dynamic Video wird nicht für Brand Portal-Mandanten unterstützt, die in der AEM-Autoreninstanz mit **[!UICONTROL Scene7Connect]**-Ausführungsmodus ausgeführt werden.

## Wie wird Dynamic Video abgespielt? {#how-are-dynamic-videos-played}

![Videokodierungen werden aus der Cloud abgerufen.](assets/VideoEncodes.png)

Wenn Dynamic Media-Konfigurationen ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings)- oder [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)-Konfigurationen) in Brand Portal eingerichtet werden, werden die dynamischen Ausgabeformate vom **[!DNL Scene 7]**-Server abgerufen. Videokodierungen werden daher in einer Vorschau angezeigt und ohne Verzögerung und Qualitätsverluste wiedergegeben.

Da Videokodierungen nicht im Brand Portal-Repository gespeichert und vom **[!DNL Scene 7]**-Server abgerufen werden, müssen Sie sicherstellen, dass die Dynamic Media-Konfigurationen in der AEM-Autoreninstanz und in Brand Portal identisch sind.

>[!NOTE]
>
>Video Viewer und Viewer-Voreinstellungen werden in Brand Portal nicht unterstützt. Videos werden in den Standard-Viewern in Brand Portal als Vorschau angezeigt und abgespielt.

## Voraussetzungen {#prerequisites}

Um mit Dynamic Video in Brand Portal zu arbeiten, müssen Sie Folgendes sicherstellen:

* **Starten Sie die AEM-Autoreninstanz im DM (Dynamic Media)-Modus.**
Starten Sie die AEM-Autoreninstanz (mit Brand Portal-Integration) im [Dynamic Media-Hybrid-Modus](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) oder [Dynamic Media [!DNL Scene 7]-Modus](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Konfigurieren Sie Dynamic Media-Cloud Services in der AEM-Autoreninstanz.**
Basierend auf dem Dynamic Media-Modus, in dem die AEM-Autoreninstanz ausgeführt wird, richten Sie entweder [Cloud Services für Dynamic Media](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) oder [[!DNL Scene 7]-Cloud Services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) auf der AEM-Autoreninstanz unter **Tools** | **Cloud Services** | **Dynamic Media** ein.
* **Konfigurieren Sie Dynamic Media in Brand Portal.**
Konfigurieren Sie basierend auf den Dynamic Media-Cloud-Konfigurationen in der AEM-Autoreninstanz die [Dynamic Media-Einstellungen](#configure-dm-hybrid-settings) oder die [[!DNL Scene 7]-Einstellungen](#configure-dm-scene7-settings) über die Admin Tools von Brand Portal.
Stellen Sie sicher, dass [separate Brand Portal-Mandanten](#separate-tenants) für AEM-Autoreninstanzen verwendet werden, die mit dem Dynamic Media Hybrid-Modus und dem Dynamic Media **[!UICONTROL Scene7]**-Modus konfiguriert sind, wenn Sie die Funktionen von Dynamic Media Hybrid und Dynamic Media**[!UICONTROL  S7]** verwenden.
* **Veröffentlichen Sie Ordner mit in Brand Portal angewendeten Videokodierungen.**
Wenden Sie [Videokodierungen](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) an und veröffentlichen Sie den Ordner mit Rich-Media-Assets von der AEM-Autoreninstanz in Brand Portal.
* **Setzen Sie Egress-IPs in SPS auf die Whitelist, wenn die sichere Vorschau aktiviert ist.**
Bei der Nutzung von Dynamic Media-**[!DNL Scene 7]**(mit[aktivierter sicherer Vorschau](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)für ein Unternehmen) wird empfohlen, dass der**[!DNL Scene 7]**-Unternehmens-Administrator [die öffentlichen Egress-IPs auf die Whitelist setzt](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service). Dies erfolgt für die betreffenden Regionen mittels der SPS (**[!UICONTROL Scene 7]**Publishing System)-Flash-Benutzeroberfläche.
Die Egress-IPs lauten wie folgt:

| **Region** | **Egress-IP** |
|--- |--- |
| nicht vorhanden | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Informationen zum Hinzufügen einer dieser Egress-IPs zur Whitelist finden Sie unter [Vorbereiten Ihres Kontos für sicheres Testen](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best Practices

Um sicherzustellen, dass Ihre Dynamic Video-Assets erfolgreich in einer Vorschau angezeigt, wiedergegeben und aus Brand Portal (und den freigegebenen Links) heruntergeladen werden, gehen Sie wie folgt vor:

### Aufteilen von Mandanten für den Dynamic Media Hybrid-Modus und den Dynamic Media Scene7-Modus {#separate-tenants}

Wenn Sie sowohl Funktionen von Dynamic Media **[!DNL Scene 7]**als auch von Dynamic Media Hybrid verwenden, wird empfohlen, verschiedene Brand Portal-Mandanten für AEM-Autoreninstanzen zu verwenden, die mit dem Dynamic Media Hybrid-Modus bzw. mit dem Dynamic Media-**[!DNL Scene 7]**-Modus konfiguriert sind.<br />

![Autoreninstanz und BP – 1:1-Zuordnung](assets/BPDynamicMedia.png)

### Gleiche Konfigurationsdetails in der AEM-Autoreninstanz und in Brand Portal

Stellen Sie sicher, dass die Konfigurationsdetails wie **[!UICONTROL Titel]**,**[!UICONTROL  Registrierungs-ID]**, **[!UICONTROL Videodienst-URL]**(in**[!UICONTROL  Dynamic Media Hybrid]**) und **[!UICONTROL Titel]**, Anmeldeinformationen (**[!UICONTROL  E-Mail-Adresse]** und Passwort), **[!UICONTROL Region]**,**[!UICONTROL  Firma]** (in Dynamic Media **[!DNL Scene 7]**) in Brand Portal und**[!UICONTROL  AEM-Cloud-Konfiguration]** identisch sind.

### Öffentliche Ausgangs-IPs für den Dynamic Media Scene7-Modus auf die Whitelist setzen

Wenn Dynamic Media **[!UICONTROL Scene 7]**mit aktivierter[sicherer Vorschau](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)genutzt wird, um Video-Assets für Brand Portal bereitzustellen, richtet**[!UICONTROL  Scene 7]** einen dedizierten Image-Server für Staging-Umgebungen oder interne Anwendungen ein. Mit einer beliebigen Anforderung an diesen Server wird die IP-Ursprungsadresse geprüft. Wenn die eingehende Anforderung nicht in der Liste genehmigter IP-Adressen enthalten ist, wird eine Fehlerantwort zurückgegeben.
Der **[!UICONTROL Scene7]**-Unternehmensadministrator konfiguriert daher eine Liste genehmigter IP-Adressen für die**[!UICONTROL  sichere Testumgebung]** seines Unternehmens. Dies erfolgt über die Flash-Benutzeroberfläche von **[!UICONTROL SPS]**(Scene7-Veröffentlichungssystem). Stellen Sie sicher, dass die Egress-IP für Ihre jeweilige Region (siehe unten) in diese genehmigte Liste aufgenommen wird.
Informationen zum Hinzufügen einer dieser Egress-IPs zur Whitelist finden Sie unter[Vorbereiten Ihres Kontos für sicheres Testen](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Die Egress-IPs lauten wie folgt:

| **Region** | **Egress-IP** |
|--- |--- |
| nicht vorhanden | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Konfigurieren von Dynamic Media (Hybrid)-Einstellungen {#configure-dm-hybrid-settings}

Wenn die AEM-Autoreninstanz im Dynamic Media Hybrid-Modus ausgeführt wird, konfigurieren Sie die Dynamic Media-Gateway-Einstellungen über die Kachel **[!UICONTROL Video]**im Admin Tools-Bereich.
>[!NOTE]
>
>Die [Videokodierungsprofile](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) werden nicht in Brand Portal veröffentlicht, sondern vom Scene 7-Server abgerufen. ****Stellen Sie daher sicher, dass die Konfigurationsdetails der[[!UICONTROL Scene 7-Cloud-Konfiguration]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)in Ihrer AEM-Autoreninstanz entsprechen, damit Videokodierungen erfolgreich in Brand Portal wiedergegeben werden können.
So richten Sie Dynamic Media-Konfigurationen für Brand Portal-Mandanten ein:

1. Wählen Sie in Brand Portal in der Symbolleiste am oberen Rand das AEM-Logo aus, um die Admin Tools aufzurufen.

2. Wählen Sie im Admin Tools-Bereich die Kachel **[!UICONTROL Video]**aus.<br />   ![Dynamic Media Hybrid-Konfiguration in Brand Portal](assets/DMHybrid-Video.png)
   Die Seite **[!UICONTROL Konfiguration für Dynamic Media bearbeiten]**wird geöffnet.<br />   ![Dynamic Media-Hybrid-Konfiguration in Brand Portal](assets/edit-dynamic-media-config.png)

3. Geben Sie die **[!UICONTROL Registrations-ID]**und**[!UICONTROL  die Video Service-URL]** (DM-Gateway URL) an. Stellen Sie sicher, dass diese Details mit denen unter **[!UICONTROL Tools > Cloud Services]**in Ihrer AEM-Autoreninstanz übereinstimmen.

4. Wählen Sie **Speichern** aus, um die Konfiguration zu speichern.

## Konfigurieren von Dynamic Media-Scene 7-Einstellungen {#configure-dm-scene7-settings}

Wenn die AEM-Autoreninstanz im Dynamic Media **[!UICONTROL Scene7]**-Modus ausgeführt wird, dann legen Sie über die Kachel**[!UICONTROL  Dynamic Media-Konfiguration]** im Admin Tools-Bereich die **[!UICONTROL Scene7]**-Servereinstellungen fest.

Gehen Sie wie folgt vor, um Dynamic Media **[!UICONTROL Scene7]**-Konfigurationen für Brand Portal-Mandanten einzurichten:

1. Wählen Sie in Brand Portal in der Symbolleiste am oberen Rand das AEM-Logo aus, um die Admin Tools aufzurufen.

2. Wählen Sie im Admin Tools-Bereich die Kachel **[!UICONTROL Dynamic Media-Konfiguration]**aus.<br />   ![DM [!UICONTROL Scene7]-Konfiguration in Brand Portal](assets/DMS7-Tile.png)
   Die Seite **[!UICONTROL Konfiguration für Dynamic Media bearbeiten]**wird geöffnet.<br />   ![Scene7-Konfiguration in Brand Portal](assets/S7Config.png)

3. Geben Sie Folgendes an:
   * **[!UICONTROL Titel]**
   * Anmeldedaten (**[!UICONTROL E-Mail-ID]**und**[!UICONTROL  Passwort]**) für den Zugriff auf den Scene7-Server
   * **[!UICONTROL Region]**Stellen Sie sicher, dass diese Werte mit denen in Ihrer AEM-Autoreninstanz übereinstimmen.

4. Wählen Sie **[!UICONTROL Mit Dynamic Media verbinden]**aus.

5. Geben Sie den **[!UICONTROL Unternehmensnamen]**an und**[!UICONTROL  speichern]** Sie die Konfiguration.
