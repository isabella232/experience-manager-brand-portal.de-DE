---
title: Häufig gestellte Fragen
seo-title: null
description: Lernen Sie die häufig gestellten Fragen im Adobe Experience Manager Assets Brand Portal kennen.
seo-description: null
uuid: null
content-type: reference
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: f8d95ab1e1c17ef2cf86d0206a36134996e4fe07

---


# Häufig gestellte Fragen {#frequently-asked-questions}

Die häufig gestellten Fragen zum Markenportal betreffen die Fragen und Probleme von Endbenutzern, die bei der Arbeit mit der neuesten Version von AEM Assets Brand Portal 6.4.5 oder früher auftreten können.



**Frage. Was ist die Hauptänderung in der Markenportal-Version 6.4.5?**

**Antwort.** AEM Assets Brand Portal 6.4.5 ist eine Funktionsversion, die es den Benutzern des Markenportals ermöglicht, Inhalte aus der Brand Portal-Instanz hochzuladen und den Beitragsordner ohne Administratorrechte wieder in AEM Assets zu veröffentlichen.
Weitere Informationen finden Sie in [Asset-Beschaffung in Brand Portal](brand-portal-asset-sourcing.md).



**Frage. Verliere ich den Zugriff auf vorhandene Assets, Funktionen oder Konfigurationen, die ich erstellt habe?**

**Antwort.** Alle bestehenden Funktionen und Konfigurationen stehen weiterhin zur Verfügung. Ihre Endbenutzer sind nicht betroffen und Ihre Inhalte bleiben intakt.



**Frage. Wann findet der Wechsel zur neuen Brand Portal-Version statt?**

**Antwort.** Brand Portal 6.4.5 wurde im Oktober 2019 zur Produktion freigegeben. Die nächste Markenportal-Version wird voraussichtlich im 3. Quartal 2020 veröffentlicht.
Für Updates und Versionsänderungen wird empfohlen, die [Versionshinweise](brand-portal-release-notes.md) und [Neuigkeiten im Markenportal](whats-new.md)zu verfolgen.



**Frage. Wie sind die Auswirkungen auf meine Benutzer?**

**Antwort.** Die Version des Markenportals 6.4.5 ist ausschließlich im Markenportal verfügbar, sodass keine Auswirkungen auf Ihre Endbenutzer auftreten.



**Frage. Ist für mich als Benutzer von Brand Portal eine Aktion erforderlich?**

**Antwort.** Die Version des Markenportals 6.4.5 enthält eine neue Funktion namens "Asset Sourcing". Der AEM-Administrator muss die Asset-Sourcing-Funktion in AEM Assets konfigurieren, um die Funktion für die Benutzer des Markenportals zu aktivieren. Weitere Informationen finden Sie unter Asset- [Beschaffung](brand-portal-configure-asset-sourcing.md)aktivieren.



**Frage. Wer kann einen Beitragsordner erstellen?**

**Antwort.** AEM-Benutzer können in AEM Assets einen neuen Ordner erstellen und die Eigenschaft **Asset Contribution** zuweisen. Der neu erstellte Ordner wird als **Beitragsordner** bezeichnet.
Dieser Ordner wird dann für die aktiven Benutzer des Markenportals freigegeben, um einen Beitrag zu erhalten.



**Frage. Was enthält ein Beitragsordner?**

**Antwort.** Der **Beitragsordner** enthält zwei Unterordner **NEW** und **SHARED**. Zunächst ist der Ordner NEW leer, und der Ordner SHARED enthält den Referenzinhalt (wiederverwendbare Assets) für die Benutzer des Markenportals.
Die Markenportal-Benutzer greifen auf den **Beitragsordner** zu und laden Inhalte in den **NEUEN** Ordner hoch.



**Frage. Wie hoch sind die Vermögensanforderungen ohne Beitrag?**

**Antwort.** Das **kurze** Dokument, das dem **Beitragsordner** angehängt ist, und der im **SHARED** -Ordner hochgeladene Referenzinhalt (wiederverwendbare Elemente) helfen dem Markenportal-Benutzer, die Notwendigkeit von Beiträgen und Erwartungen als Beitragszahler zu verstehen und wird kollektiv als Asset-Anforderungen bezeichnet.



**Frage. Kann ich Assets in einen beliebigen zulässigen Ordner hochladen?**

**Antwort.** Nicht alle zulässigen Ordner. Ein Markenportal-Benutzer kann Inhalte nur in den **Beitragsordner** hochladen, der vom AEM- oder Markenportal-Administrator freigegeben wird.



**Frage. Wie erhalte ich Zugriff auf einen Beitragsordner?**

**Antwort.** Sie können nur dann auf einen **Beitragsordner** zugreifen, wenn dieser für Sie freigegeben wurde. Sie erhalten eine E-Mail-/Pulsbenachrichtigung, sobald ein Beitragsordner für Sie freigegeben wurde. Sie können entweder über den in der E-Mail freigegebenen Link auf den Beitragsordner zugreifen oder sich bei Ihrer Markenportal-Instanz anmelden und zum Glockensymbol für die Benachrichtigung navigieren, um auf den Beitragsordner zuzugreifen.

>[!NOTE]
>
>Wenn Sie kein bestehender Brand Portal-Benutzer sind, bitten Sie den AEM-Administrator, Ihren Benutzer in der AEM-Admin-Konsole zu erstellen und Ihr Profil der Benutzerkonfigurationsdatei in der Benutzerliste von Brand Portal-Benutzern hinzuzufügen. Siehe [Hinzufügen von Markenportal-Benutzern](brand-portal-configure-asset-sourcing.md).



**Frage. Welches Format hat die CSV-Datei für den Benutzerimport?**

**Antwort.** Das Format entspricht dem Format, das von der Admin-Konsole für den Massenimport von Benutzern unterstützt wird. E-Mail, Vorname und Nachname sind obligatorisch.



**Frage. Wie wird die Liste der Benutzer (Markenportal-Mitarbeiter) in der Dropdown-Liste "Asset Contribution-Benutzer"gefüllt?**

**Antwort.** Die Benutzer in der Dropdown-Liste werden aus der in AEM hochgeladenen Datei für die Markenportal-Benutzerkonfiguration (.csv) gefüllt.



**Frage. Wo kann ich den Status von Import- und Veröffentlichungsaufträgen sehen?**

**Antwort.** In AEM können Sie den Status eines Imports auf einer **asynchronen** Auftragsseite sehen. Im Markenportal können Sie den Status eines Veröffentlichungsauftrags unter **[!UICONTROL Werkzeuge &gt; Asset-Beitragsstatus]** anzeigen.



**Frage. Wie häufig wird ein Importauftrag ausgeführt, der regelmäßig in AEM ausgeführt wird?**

**Antwort.** In AEM wird die Abfrage alle 5 Minuten ausgeführt.



**Frage. Gibt es einen Schwellenwert dafür, wie oft ein Ordner vom Markenportal in AEM Assets veröffentlicht werden kann?**

**Antwort.** Nein, alle Assets im Ordner **NEW** werden unabhängig davon, ob sie zuvor veröffentlicht wurden, in AEM Assets veröffentlicht. Jedes Mal, wenn ein **Beitragsordner** vom Markenportal in AEM Assets veröffentlicht wird, überschreibt er den Inhalt des **NEUEN** Ordners.



**Frage. Wie können Sie neue Assets in einen Beitragsordner hochladen?**

**Antwort.** Lesen Sie die detaillierte Dokumentation zum [Hochladen von Assets in den Beitragsordner](brand-portal-upload-assets-to-contribution-folder.md).



**Frage. Ich sehe keine Miniaturansichten/Vorschauen zu den Assets, die von einem Brand Portal-Benutzer in den Ordner NEW hochgeladen wurden?**

**Antwort.** Es ist wie entworfen, coz es gibt keinen Workflow am Ende des Brand Portal.



**Frage. Was passiert, wenn ein Ordner von AEM Assets an das Markenportal veröffentlicht wird, der sich im Fluss befindet?**

**Antwort.** In AEM werden Protokolle für jedes Mal gepflegt, wenn ein Ordner im Markenportal veröffentlicht wird. Zum Zeitpunkt der Veröffentlichung werden alle Assets, die nicht im Markenportal veröffentlicht werden, in eine Replikationswarteschlange gestellt. Assets, die dem Ordner nach dem Auslösen des Veröffentlichungsauftrags hinzugefügt wurden, werden nicht im Markenportal veröffentlicht. Wenn der AEM-Benutzer den Ordner erneut veröffentlicht, werden nur die Assets, die zuvor noch nicht veröffentlicht wurden (in der Replikationswarteschlange vorhanden), im Markenportal veröffentlicht.
Dies gilt für alle Ordner, die von AEM Assets im Markenportal veröffentlicht werden, und für freigegebene Ordner in einem Beitragsordner.



**Frage. An wen kann ich mich bei Fragen wenden?**

**Antwort.** Kontaktieren Sie Ihren Adobe-Kundenbetreuer oder den Kundensupport.


>[!NOTE]
>
>Der Veröffentlichungszeitplan ist vorläufig und kann jederzeit geändert werden. Wenden Sie sich an Ihren Adobe-Kundenbetreuer oder den Kundensupport, um aktuelle Informationen zum Veröffentlichungszeitplan zu erhalten.




## Produktzugriff und Support (Websites mit Zugriffsbeschränkung) {#product-access-and-support-restricted-sites}

Diese Sites sind nur für Kunden verfügbar. Wenn Sie Kunde sind und Zugriff benötigen, wenden Sie sich an Ihren Adobe-Kundenbetreuer.

* [](https://daycare.day.com) [Produktzugriff](https://login.marketing.adobe.com)

* [Adobe-Kundendienst](https://helpx.adobe.com/contact.html)
