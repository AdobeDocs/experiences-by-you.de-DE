---
title: Entwerfen von Omnichannel-Konversationsmarketing mit Dynamic Chat
description: Erhalten Sie einen schnellen Einstieg in die Gestaltung von konversativem Marketing mit Adobe Dynamic Chat, dem nativen Kanal für konversatives Engagement in Adobe Marketo Engage. Dieses Tutorial bietet umsetzbare Rezepte zur Implementierung von Anwendungsfällen wie z. B. Buchung von Verkaufs-Meetings, Interaktion mit Website-Inhalten und Veranstaltungen/Webinar-Promotion.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-23T00:00:00Z
jira: KT-14814
exl-id: 160dfb25-9f54-4dce-a08a-4a8d3c4c5368
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# Gestalten von Omni-Channel-Konversationsmarketing mit Dynamic Chat

Marketing-Experten und -Expertinnen können Ihre Website entscheidend dazu beitragen, Leads zu generieren, Konversionen zu steigern und Verkaufszyklen zu beschleunigen. Durch die Interaktion mit Besuchern in Echtzeit auf Ihrer Website kann Ihr Vertriebsteam Käufer effizienter qualifizieren. Adobe Dynamic Chat, der native Chat-Kanal innerhalb Ihres Adobe Marketo Engage-Abonnements, ermöglicht es Ihnen, Konversationen zu automatisieren, um die Funktionen der Marketo Engage zu erweitern.

In diesem Tutorial werden der Denkprozess und die wichtigsten Anwendungsfälle beschrieben, die Sara Barriuso, Marketing Operations Manager bei Cornerstone OnDemand, während des „Lernens von Gleich gesinnten“ vorgestellt hat. Sie erklärte, wie ihr Unternehmen Dynamic Chat nutzt, um die Fähigkeiten der Marketo Engage zu maximieren.

## Gesprächsführung in die Strategie zur Bedarfsgenerierung integrieren

Besucher können Ihre Website aus einem bestimmten Grund durchsuchen. Möglicherweise suchen sie nach Inhalten zu Ihren Produkten oder Services oder suchen Kontaktinformationen, um mit Ihren Vertriebsmitarbeitern zu sprechen. Es könnten auch Ihre Kunden sein, die nach zusätzlichen Produktinformationen suchen. Der Chat ermöglicht es den Besuchern Ihrer Website, sich selbst zu bedienen und sich selbst zu qualifizieren, wenn sie bereit sind, mit Ihrem Verkaufsteam zu sprechen.

Als Sara Barriuso Dynamic Chat implementierte, war sie von der nahtlosen Integration mit Marketo Engage und den [vordefinierten Aktivitäts-Trigger ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities){target="_blank"} die Marketo Engage-Programme aktivieren und umgekehrt angezogen. Sie entwickelte ihre Strategien zur konversativen Interaktion mit drei Zielgruppensegmenten:

1. Unbekannte Interessenten: Bieten Sie proaktiv Demo-Aufrufe an, um neue Leads zu generieren.
2. Bekannte Leads/Kunden: Verlängern Sie die Besuchszeit für das Durchsuchen von Inhalten und bieten Sie Demo-Aufrufe an, um Upsell- und Crosssell-Möglichkeiten zu generieren.
3. Interessenten/Kunden: Bieten Sie personalisierte Erlebnisse, indem Sie die Anstrengungen der Marketing-Kampagnen erweitern.


## Wichtige Anwendungsfälle, um mit der Erstellung Ihrer Dialoge zu beginnen

Um diese Strategien zu implementieren, erstellte Sara ihre Dynamic Chat-Dialogfelder um die folgenden Anwendungsfälle herum:

1. Standarddialogfeld für alle Besucherinnen und Besucher: Geben Sie allen Besucherinnen und Besuchern eine erste Option, damit sie ihre Aufgaben effizienter erledigen können.

2. Förderung der Anmeldung für Veranstaltungen und Webinare: Ermutigen Sie Website-Besucher, sich für Veranstaltungen und Webinare zu registrieren, um sie schneller in die Kaufphase zu bringen.

3. Erweiterung der Interaktion mit Kampagneninhalten: Bieten Sie zusätzlichen Kontext an oder beantworten Sie potenzielle Fragen, wenn Besucher Inhalte auf der Website durchsuchen.

Sehen wir uns diese Anwendungsfälle in Aktion an, während Sara ihren Prozess präsentiert, von der Zuordnung des Gesprächsflusses über die Konfiguration der Dialoge bis hin zum Targeting in Dynamic Chat und Marketo Engage.

### Anwendungsfall 1: Standarddialogfeld „Alle auffangen“ für alle Site-Besucher

Dieses Dialogfeld bietet fünf erste Optionen für Website-Besuchende, aus denen sie wählen können, sodass sie ein selbstgesteuertes Erlebnis erhalten, das ihnen hilft, die benötigten Informationen basierend auf ihrer Rolle zu finden. Zunächst sollten Sie Ihren E-Mail-Posteingang „Kontakt“ erkunden, um allgemeine Themen zu identifizieren und sie in Dialogoptionen zu kategorisieren, die für Ihre Site-Besucher gelten. Sehen Sie sich die Demo an und führen Sie die folgenden Schritte aus, um Ihr standardmäßiges Catch-All-Dialogfeld zu erstellen:

>[!VIDEO](https://video.tv.adobe.com/v/3429194/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Phase 1

1. Erstellen Sie das Dialogfeld und erstellen Sie einen Test-Link.
2. Fügen Sie ein Ziel hinzu, um die Konversionen zu verfolgen (z. B. Übermittlung von Demoanfragen).
3. Lassen Sie es von 2-3 Personen testen und sammeln Sie Feedback.

#### Phase 2

1. Fügen Sie unter „Zielgruppe“ eine Web-Seiten-URL in „Target“ hinzu, um anzugeben, wo das Dialogfeld angezeigt werden soll.
2. Fügen Sie in „Einstellungen“ den Kampagnennamen, die Beschreibung, die Priorität und die Sprache hinzu.
3. Klicken Sie auf &quot;Publish&quot;

>[!TAB Marketo Engage]

#### Phase 1

1. Erstellen Sie Ihre intelligente Tracking-Kampagne.
2. Verwenden Sie in „Smart List“ den Trigger „Reaches Dialogue Goal“. Verwenden Sie das gleiche Ziel (z. B. Demoanfrage) wie bei Dialogfeld
3. Fügen Sie in „Fluss“ den Schritt „Programmstatus ändern“ ein, um die Konvertierung zu verfolgen.
4. Die Quelle wird als „dynamicChat“ angezeigt. Sie können eine Smart-Kampagne erstellen, um die Quelle auf einen Namen zu aktualisieren, der für Sie sinnvoll ist.

#### Phase 2

1. Testen Sie Ihre Tracking-Smart-Kampagne erneut, wenn sie live ist.

>[!ENDTABS]

#### Stufe höher: Account-Based Marketing

Sie können den standardmäßigen Catch-All-Dialog weiter verbessern, indem Sie branchenspezifische Inhalte integrieren, wodurch die Konversationen für Besuchende noch nützlicher werden. Schlagen Sie beispielsweise branchenspezifische Whitepapers oder Fallstudien vor, die Ihre Besucher herunterladen können. Sehen Sie sich die Demo an und führen Sie die folgenden Schritte aus, um ein standardmäßiges Sammeldialogfeld für Account-basiertes Marketing zu erstellen:

>[!VIDEO](https://video.tv.adobe.com/v/3429195/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Klonen Sie das „Standarddialogfeld“ und benennen Sie es um.
2. Passen Sie in „Stream Designer&quot; Dialognachrichten an die Zielbranche an (nur ein Stream + die ursprüngliche Frage).
3. Lassen Sie 2-3 Personen das Dialogfeld testen und Feedback einholen.
4. Erstellen Sie einen Test-Link und teilen Sie ihn.
5. Fügen Sie unter „Zielgruppe“ eine Web-Seiten-URL hinzu, über die das Dialogfeld angezeigt und die Zielgruppe für die gewünschte Branche aktualisiert wird.
6. Fügen Sie in „Einstellungen“ den Kampagnennamen, die Beschreibungspriorität und die Sprache hinzu.
7. Klicken Sie auf &quot;Publish&quot;.

>[!TAB Marketo Engage]

1. Erstellen Sie Ihre intelligente Tracking-Kampagne und testen Sie das Ziel.
2. Testen Sie die Tracking-Smart-Kampagne nach der Veröffentlichung des Dialogfelds erneut.

>[!ENDTABS]

### Anwendungsfall 2: Registrierung für Veranstaltungen und Webinare bewerben

Veranstaltungen und Webinare sind beliebte Marketing-Taktiken für B2B-Unternehmen, um Nachfrage zu generieren. Sie bieten ansprechende Erlebnisse und umfangreiche Informationen, die potenzielle Kunden anziehen. Wenn Sie Ihre Website-Besucher mit anstehenden Veranstaltungen und Webinaren verbinden, können Sie potenzielle Kunden noch schneller qualifizieren. Die Erstellung dieses Dialogfelds ist mit geringem Aufwand und geringen Kosten verbunden und kann schnell den Erfolg demonstrieren, sodass Sie Unterstützung von Marketing-Stakeholdern erhalten, um Ihrem Omni-Channel-Automatisierungsplan Gesprächsinteraktionen hinzuzufügen. Sehen Sie sich die Demo an und führen Sie die folgenden Schritte aus, um Ihr Ereignis-/Webinar-Promotion-Dialogfeld zu erstellen:

>[!VIDEO](https://video.tv.adobe.com/v/3429196/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Phase 1

1. Erstellen Sie eine Vorlage für das Dialogfeld „Ereignisregistrierung“ für die laufende Verwendung in Kampagnen.

#### Phase 2

1. Klonen Sie die Vorlage .
2. Kopieren Sie Text und fügen Sie ihn in die Dialogfeldnachricht für ein neues Ereignis ein.
3. Aktualisieren Sie die in Ihrem Ereignis-Link verwendeten UTM-Parameter (z. B. utm_medium=website&amp;utm_source=adobe).
4. Erstellen Sie einen Test-Link, klicken Sie auf &quot;Publish&quot; und teilen Sie ihn mit dem Antragsteller.
5. Peer-Review und Anwendung von Feedback.


>[!TAB Marketo Engage]

#### Phase 1

1. Erstellen Sie Ihre Smart-Tracking-Kampagne in der Vorlage des Webinars/Veranstaltungsprogramms und testen Sie sie.

#### Phase 2

1. Fügen Sie Ihren Kampagnennamen zur Tracking-Smart-Kampagne in Marketo Engage hinzu und testen Sie sie.

>[!ENDTABS]


#### Level up: Bekannte Personen registrieren

Sie können Besuchenden der Website ein noch besseres Erlebnis bieten, indem Sie sie für Ihre Veranstaltungen und Webinare registrieren, ohne dass sie ein Formular ausfüllen müssen. Personalisierte Erlebnisse schaffen Vertrauen und zeigen Besuchern, dass Sie sich an sie erinnern. Sehen wir uns an, wie Sie Ihr Ereignis- und Webinar-Promotion-Dialogfeld in Aktion abgleichen.

>[!NOTE]
>Beachten Sie das potenzielle Sicherheitsrisiko in bestimmten Schutzstaaten/Ländern und setzen Sie diese Personalisierung sorgfältig durch Beratung mit Ihrer Rechtsabteilung um.

>[!VIDEO](https://video.tv.adobe.com/v/3429197/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Klonen Sie das Dialogfeld Ereignis-/Webinar-Promotion .
2. Fügen Sie in Stream Designer, nachdem der Benutzer „Ja“ geantwortet hat, eine Fragekarte hinzu: „Sie haben Ihre E-Mail-Adresse zuvor für uns freigegeben. Möchten Sie dies für die Veranstaltungsdetails beibehalten?“
3. Falls sie mit „Ja“ antworten, fügen Sie eine Nachrichtenkarte hinzu: „Sie erhalten eine Bestätigungs-E-Mail in Ihrer E-Mail mit den Details zum Ereignis/Webinar“.
4. Falls sie mit „Nein“ antworten, fügen Sie eine Nachrichtenkarte hinzu: „Bitte füllen Sie das Formular auf der Registrierungsseite aus“.
5. Erstellen Sie einen Test-Link, klicken Sie auf &quot;Publish&quot; und teilen Sie ihn mit dem Antragsteller.
6. Fügen Sie in der Registerkarte Zielgruppe hinzu [E-Mail ist nicht leer].

>[!TAB Marketo Engage]

1. Fügen Sie dieses neue Dialogfeld zur Tracking-Smart-Kampagne in Marketo Engage hinzu und testen Sie es.

>[!ENDTABS]

### Anwendungsfall 3: Erweiterung der Interaktion mit Kampagneninhalten

Stellen Sie sich ein fesselndes Schaufenster vor, das Sie ins Auge fasst und in einen Laden zieht. Wenn Ihnen ein Rezeptionist bei der Auswahl der Produkte hilft oder Ihre Fragen beantwortet, könnten Sie sich wohler fühlen, wenn Sie einen Kauf tätigen. Um dieses Erlebnis online zu replizieren, können Sie Ihr Dynamic Chat-Dialogfeld auf den Web-Seiten anzeigen lassen, auf denen Ihre Marketing-Kampagnen Besucher anleiten. Wenn Anwender mit den Web-Inhalten interagieren, zeigt Dynamic Chat sofort relevante Unterhaltungen an, schlägt zusätzliche Inhalte vor oder adressiert potenzielle Fragen. Dies wird durch die Nutzung von Automatisierungs-Trigger erreicht, um Dynamic Chat-Kampagnen basierend auf der Benutzerinteraktion innerhalb von Marketo Engage-Programmen zu aktivieren. Lassen Sie uns nun sehen, wie wir diesen Anwendungsfall zum Leben erwecken.

>[!VIDEO](https://video.tv.adobe.com/v/3429199/?learn=on)

Erweitern der Interaktion mit Campaign-Inhalten - Konfiguration:

>[!VIDEO](https://video.tv.adobe.com/v/3429200/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Generieren Sie neue Leads für Ihre Kampagnen über E-Mails und die Touchpoints sozialer Kampagnen. In diesem Beispiel wird die Talent Health Index-Umfrage auf der Website der Marke gehostet.
2. Klonen Sie eine vorhandene Dialogfeldvorlage (z. B. das standardmäßige Catch-all-Dialogfeld), um drei Dialogfelder für die folgenden Szenarien zu erstellen und die „Ziel-URL“ im Tab „Zielgruppe“ entsprechend zu aktualisieren:
   * Wenn Web-Besucher von Ihren Marketing-Kanälen kamen und auf Ihrer Web-Seite landen.
   * Auf der Dankeseite
   * Besucherinnen und Besucher, die innerhalb von 45 Tagen nach der Marketing-Kampagne auf Ihre Website zurückkehren (Retargeting)

>[!ENDTABS]

## Wie geht es weiter?

* Ordnen Sie Ihren Gesprächsfluss in [Stream Designer](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer){target="_blank"} oder einem Flussdiagramm offline zu.
* Erstellen Sie ein standardmäßiges Auffangdialogfeld im Dynamic Chat.
* Aktivieren Sie die Konversationen nach der Kampagneninteraktion mithilfe von Automatisierungs-Trigger in Marketo Engage.


## Autoren

{{sara-barriuso}}

{{amy-chiu}}
