---
title: Omnichannel-Konversationsmarketing mit Dynamic Chat entwerfen
description: Verschaffen Sie sich einen schnellen Einstieg in die Konzeption von Konversationsmarketing mit Adobe Dynamic Chat, dem nativen Konversationskanal innerhalb von Adobe Marketo Engage. In diesem Tutorial finden Sie umsetzbare Rezepte zur Implementierung von Anwendungsfällen wie z. B. Buchung von Verkaufstreffen, Interaktion mit Website-Inhalten und Veranstaltungen/Webinar-Promotion.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-23T00:00:00Z
jira: KT-14814
exl-id: 160dfb25-9f54-4dce-a08a-4a8d3c4c5368
source-git-commit: 80553c5127afda315e97183e0d3b160871352183
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# Omnichannel-Konversationsmarketing mit Dynamic Chat entwerfen

Marketingexperten ist Ihre Website von entscheidender Bedeutung für die Generierung von Leads, die Steigerung von Konversionen und die Beschleunigung von Verkaufszyklen. Durch die Interaktion mit Besuchern in Echtzeit auf Ihrer Website kann Ihr Verkaufsteam Käufer effizienter qualifizieren. Mit Adobe Dynamic Chat, dem nativen Chat-Kanal in Ihrem Adobe Marketo Engage-Abonnement, können Sie Konversationen automatisieren, um die Marketo Engage-Funktionen zu erweitern.

In diesem Tutorial werden der Denkprozess und die wichtigsten Anwendungsfälle erläutert, die Sara Barriuso, Marketing Operations Manager bei der zentralen OnDemand, während der &quot;Lernen von Ihren Kollegen&quot;freigegeben hat. Sie erläuterte, wie ihre Organisation Dynamic Chat nutzte, um die Marketo Engage-Funktionen zu maximieren.

## Integrieren des Dialogeinsatzes in Ihre Strategie zur Nachfragegenerierung

Besucher durchsuchen Ihre Website aus einem Grund. Möglicherweise suchen sie Inhalte zu Ihren Produkten oder Dienstleistungen oder suchen nach Kontaktinformationen, um mit Ihren Vertriebsmitarbeitern zu sprechen. Sie können auch Ihre Kunden sein, die nach zusätzlichen Produktinformationen suchen. Chat ermöglicht es Besuchern Ihrer Website, sich selbst zu versorgen und sich selbst zu qualifizieren, wenn sie bereit sind, mit Ihrem Verkaufsteam zu sprechen.

Als Sara Barriuso Dynamic Chat implementierte, wurde sie von seiner nahtlosen Integration in Marketo Engage und [vordefinierte Aktivitäts-Trigger](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities){target="_blank"} die Marketo Engage-Programme aktivieren und umgekehrt. Sie entwickelte ihre Konversationsstrategien mit Blick auf drei Zielgruppensegmente:

1. Unbekannte potenzielle Kunden: proaktiv Demoaufrufe anbieten, um neue Leads zu generieren.
2. Bekannte Leads/Kunden: Verkürzen Sie die Besuchszeit für das Durchsuchen von Inhalten und bieten Sie Demoaufrufe an, um Upsell- und Crosssell-Möglichkeiten zu generieren.
3. Perspektiven/Kunden: Stellen Sie personalisierte Erlebnisse bereit, indem Sie die Anstrengungen der Marketing-Kampagnen erweitern.


## Wichtige Anwendungsbeispiele für den Beginn der Dialogfelderstellung

Um diese Strategien zu implementieren, erstellte Sara ihre Dynamic Chat-Dialoge um die folgenden Anwendungsfälle herum:

1. Standarddialogfeld &quot;Alles einholen&quot;: Geben Sie allen Besuchern eine erste Option, um sie bei der effizienteren Erfüllung ihrer Aufgaben zu unterstützen.

2. Veranstaltung und Webinarregistrierung bewerben: Leiten Besucher der Website dazu, sich für Veranstaltungen und Webinare zu registrieren, um sie schneller in die Kaufphase zu stürzen.

3. Erweiterung der Interaktion mit Kampagneninhalten: Bieten Sie zusätzlichen Kontext oder adressieren Sie potenzielle Fragen, wenn Besucher Inhalte auf der Website durchsuchen.

Sehen wir uns diese Anwendungsfälle in Aktion an, als Sara ihren Prozess präsentiert, von der Zuordnung des Dialogflusses bis zur Konfiguration der Dialoge und des Targetings in Dynamic Chat und Marketo Engage.

### Nutzungsszenario 1: Standard-Sammeldialogfeld für alle Site-Besucher

Dieses Dialogfeld bietet fünf Optionen, aus denen Site-Besucher auswählen können. Es bietet ein selbstgeführtes Erlebnis, das ihnen dabei hilft, die benötigten Informationen basierend auf ihrer Person zu finden. Zunächst möchten Sie möglicherweise Ihren E-Mail-Posteingang &quot;Kontakt&quot;durchsuchen, um allgemeine Themen zu identifizieren und sie in Dialogoptionen zu kategorisieren, die für Ihre Site-Besucher gelten. Sehen Sie sich die Demo an und führen Sie die folgenden Schritte aus, um Ihr standardmäßiges &quot;catch all&quot;-Dialogfeld zu erstellen:

>[!VIDEO](https://video.tv.adobe.com/v/3429194/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Phase 1

1. Erstellen Sie das Dialogfeld und erstellen Sie einen Test-Link.
2. Fügen Sie ein Ziel hinzu, um die Konversionen zu verfolgen (z. B. die Übermittlung von Demoanfragen).
3. Lassen Sie es von 2 bis 3 Personen testen und Feedback sammeln.

#### Phase 2

1. Fügen Sie in &quot;Zielgruppe&quot;eine Web-Seiten-URL in &quot;Target&quot;hinzu, um anzugeben, wo das Dialogfeld angezeigt wird.
2. Fügen Sie unter &quot;Einstellungen&quot;den Kampagnennamen, die Beschreibung, die Priorität und die Sprache hinzu.
3. Klicken Sie auf &quot;Veröffentlichen&quot;

>[!TAB Marketo Engage]

#### Phase 1

1. Erstellen Sie Ihre Tracking-Smart-Kampagne.
2. Verwenden Sie in &quot;Smart List&quot;den Trigger &quot;Reaches Dialog Goal&quot;. Verwenden Sie dasselbe Ziel (z. B. Demoanfrage), das Sie im Dialogfeld verwendet haben
3. Fügen Sie in &quot;Fluss&quot;den Schritt &quot;Programmstatus ändern&quot;ein, um die Konvertierung zu verfolgen.
4. Die Quelle wird als &quot;dynamicChat&quot;angezeigt. Sie können eine Smart-Kampagne erstellen, um die Quelle auf einen für Sie sinnvollen Namen zu aktualisieren.

#### Phase 2

1. Testen Sie Ihre Verfolgung für Smart Campaign erneut, wenn sie aktiv ist.

>[!ENDTABS]

#### Ebene nach oben: Account-basiertes Marketing

Sie können das standardmäßige &quot;Catch-all&quot;-Dialogfeld weiter verbessern, indem Sie branchenspezifische Inhalte integrieren und so die Konversationen für Besucher noch nützlicher machen. Sie können beispielsweise branchenspezifische Whitepapers oder Fallstudien vorschlagen, die Ihre Besucher herunterladen können. Sehen Sie sich die Demo an und führen Sie die folgenden Schritte aus, um ein standardmäßiges Sammeldialogfeld für kontobasiertes Marketing zu erstellen:

>[!VIDEO](https://video.tv.adobe.com/v/3429195/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Klonen Sie das &quot;Standarddialogfeld&quot;und benennen Sie es um.
2. Passen Sie in &quot;Stream Designer&quot;Dialogfeldnachrichten an die Zielbranche an (nur ein Stream und die erste Frage).
3. Lassen Sie 2-3 Personen das Dialogfeld testen und Feedback sammeln.
4. Erstellen Sie einen Test-Link und geben Sie ihn frei.
5. Fügen Sie in &quot;Zielgruppe&quot;eine Web-Seiten-URL hinzu, in der das Dialogfeld angezeigt wird, und aktualisieren Sie das Ziel für die Branche, die Sie möchten.
6. Fügen Sie unter &quot;Einstellungen&quot;den Kampagnennamen, die Beschreibungspriorität und die Sprache hinzu.
7. Klicken Sie auf &quot;Veröffentlichen&quot;.

>[!TAB Marketo Engage]

1. Erstellen Sie Ihre Tracking-Smart-Kampagne und testen Sie das Ziel.
2. Testen Sie die Verfolgung von Smart-Campaign nach der Veröffentlichung des Dialogfelds erneut.

>[!ENDTABS]

### Anwendungsfall 2: Veranstaltung bewerben und Webinar-Registrierung

Veranstaltungen und Webinare sind beliebte Marketingtaktiken für B2B-Unternehmen, um Nachfrage zu generieren. Sie bieten ansprechende Erlebnisse und umfassende Informationen, die potenzielle Kunden anlocken. Indem Sie Ihre Website-Besucher mit bevorstehenden Veranstaltungen und Webinaren verbinden, können Sie potenzielle Kunden noch schneller qualifizieren. Die Erstellung dieses Dialogfelds ist mit geringem Aufwand und niedrigen Kosten verbunden und kann schnell Erfolg zeigen. So können Sie von Marketing-Stakeholdern Unterstützung erhalten, damit Sie Ihrem Omnichannel-Automatisierungsplan Dialoginteraktionen hinzufügen können. Sehen Sie sich die Demo an und führen Sie die folgenden Schritte aus, um das Dialogfeld zur Veranstaltung/Webinar-Promotion zu erstellen:

>[!VIDEO](https://video.tv.adobe.com/v/3429196/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Phase 1

1. Erstellen Sie eine Vorlage für das Dialogfeld &quot;Ereignisregistrierung&quot;für die laufende Verwendung von Kampagnen.

#### Phase 2

1. Klonen Sie die Vorlage.
2. Kopieren und Einfügen von Text in die Dialogfeldmeldung für ein neues Ereignis
3. Aktualisieren Sie die in Ihrem Ereignislink verwendeten UTM-Parameter (z. B. utm_medium=website&amp;utm_source=adobe).
4. Erstellen Sie einen Test-Link, klicken Sie auf &quot;Veröffentlichen&quot;und geben Sie ihn für den Anforderer frei.
5. Peer Review und Feedback anwenden.


>[!TAB Marketo Engage]

#### Phase 1

1. Erstellen Sie Ihre Tracking-Smart-Kampagne in der Webinar-/Ereignisprogrammvorlage und testen Sie sie.

#### Phase 2

1. Fügen Sie Ihren Kampagnennamen zur Verfolgung von Smart Campaign in Marketo Engage hinzu und testen Sie ihn.

>[!ENDTABS]


#### Stufe up: Bekannte Personen registrieren

Sie können Website-Besuchern ein noch besseres Erlebnis bieten, indem Sie sie für Ihre Veranstaltungen und Webinare registrieren, ohne dass sie ein Formular ausfüllen müssen. Personalisierte Erlebnisse schaffen Vertrauen und zeigen Besuchern, dass Sie sich daran erinnern. Sehen wir uns an, wie Sie Ihr Ereignis- und Webinar-Promotion-Dialogfeld in Aktion einstufen.

>[!NOTE]
>Bitte beachten Sie das potenzielle Sicherheitsrisiko, das in bestimmten Schutzstaaten/Ländern besteht, und setzen Sie diese Personalisierung sorgfältig durch, indem Sie sich mit Ihrem Rechtsabteilung beraten.

>[!VIDEO](https://video.tv.adobe.com/v/3429197/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Klonen Sie das Dialogfeld für die Veranstaltung/Webinar-Promotion.
2. Fügen Sie in Stream Designer, nachdem der Benutzer &quot;Ja&quot; beantwortet, eine Fragenkarte hinzu: &quot;Sie haben Ihre E-Mail-Adresse bereits mit uns geteilt. Möchten Sie dies für die Ereignisdetails beibehalten?&quot;
3. Wenn sie auf &quot;Ja&quot; antworten, fügen Sie eine Nachrichtenkarte hinzu: &quot;Sie erhalten eine Bestätigungs-E-Mail mit den Details zum Ereignis/Webinar in Ihrer E-Mail&quot;.
4. Wenn sie auf &quot;Nein&quot; antworten, fügen Sie eine Nachrichtenkarte hinzu: &quot;Bitte füllen Sie das Formular auf der Registrierungsseite aus&quot;.
5. Erstellen Sie einen Test-Link, klicken Sie auf &quot;Veröffentlichen&quot;und geben Sie ihn für den Anforderer frei.
6. Fügen Sie auf der Registerkarte Zielgruppe hinzu. [email ist nicht leer].

>[!TAB Marketo Engage]

1. Fügen Sie dieses neue Dialogfeld zur Verfolgung von Smart-Kampagnen in Marketo Engage hinzu und testen Sie es.

>[!ENDTABS]

### Anwendungsfall 3: Erweiterung der Interaktion mit Kampagneninhalten

Stellen Sie sich vor, ein faszinierendes Fenster fängt Ihr Auge und zieht Sie in einen Laden. Wenn ein Rezeptionist Ihnen dann hilft, Produkte auszuwählen oder Ihre Fragen zu beantworten, können Sie sich bei einem Kauf besser fühlen. Um dieses Erlebnis online zu replizieren, kann Ihr Dynamic Chat-Dialogfeld auf den Webseiten angezeigt werden, auf denen Ihre Marketingkampagnen Besucher direkt leiten. Wenn Benutzer mit den Webinhalten interagieren, zeigt Dynamic Chat sofort relevante Unterhaltungen an, um zusätzliche Inhalte vorzuschlagen oder potenzielle Fragen zu beantworten. Dies wird durch die Nutzung von Automatisierungs-Triggern erreicht, um Dynamic Chat-Kampagnen basierend auf der Benutzerinteraktion innerhalb von Marketo Engage-Programmen zu aktivieren. Sehen wir uns an, wie wir diesen Anwendungsfall zum Leben erwecken können.

>[!VIDEO](https://video.tv.adobe.com/v/3429199/?learn=on)

Erweiterung der Interaktion mit Campaign-Inhalten - Konfiguration:

>[!VIDEO](https://video.tv.adobe.com/v/3429200/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Erstellen Sie neue Leads für Ihre Kampagnen über die Touchpoints von E-Mail- und Social-Media-Kampagnen. In diesem Beispiel wird die Talent Health Index-Umfrage auf der Website der Marke gehostet.
2. Klonen Sie eine vorhandene Dialogfeldvorlage (z. B. standardmäßiges Sammeldialogfeld), um drei Dialogfelder für die folgenden Szenarien zu erstellen und die &quot;Ziel-URL&quot;auf der Registerkarte &quot;Zielgruppe&quot;entsprechend zu aktualisieren:
   * Wenn Webbesucher von Ihren Marketingkanälen kamen und auf Ihre Webseite kamen.
   * Auf der Dankeseite
   * Alle Besucher, die innerhalb von 45 Tagen nach der Teilnahme an der Marketingkampagne (Retargeting) zu Ihrer Website zurückkehren

>[!ENDTABS]

## Wie geht es weiter?

* Verfolgen Sie Ihren Gesprächsfluss in [Stream-Designer](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer){target="_blank"} oder ein Flussdiagramm offline.
* Erstellen Sie ein standardmäßiges &quot;catch-all&quot;-Dialogfeld im Dynamic Chat.
* Aktivieren Sie die Interaktion der Konversationen nach der Kampagne, indem Sie Automatisierungs-Trigger in Marketo Engage verwenden.


## Autoren

{{sara-barriuso}}

{{amy-chiu}}
