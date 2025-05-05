---
title: Erstellen von Personenbewertungsmodellen für Marketo Engage-Programme
description: Erfahren Sie, wie Sie Ihre Bewertungsmodelle von Grund auf erstellen.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14810
thumbnail: KT-14810.jpeg
exl-id: 73976144-f02b-4423-9b4b-410330117ba9
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '2055'
ht-degree: 2%

---

# Erstellen eines Personenbewertungsmodells

Mit der Personenbewertung können Sie die Personen identifizieren, die mit Ihrem Unternehmen am meisten interagieren und Ihr ideales Kundenprofil sind, damit Sie diese Leads mit Ihrem Verkaufsteam teilen und Angebote abschließen können! Zusammen mit dem Vertrieb bestimmen Sie mithilfe eines Lead/Personen-Bewertungsprogramms in Adobe Marketo Engage, welche Leads Sie an sie weitergeben möchten. Dies kann entweder durch ein Minimum an Verhaltensbewertung, demografischer Bewertung oder beides bestimmt werden.

In diesem Tutorial führen wir Sie durch drei Übungen, die von den Marketo Engage-Champions Christina Zuniga und Katja Keesom vorgeschlagen wurden. Bestimmen Sie anschließend, welche Aktivitäten und Merkmale wichtige Indikatoren sind, an deren Kauf eine Interessentin interessiert ist (Verhaltens-Scoring), und finden Sie heraus, welche für Sie am besten geeignet sind (demografisches Scoring). Berücksichtigen Sie außerdem die Feinheiten in den verschiedenen Märkten.

## Warum sollte ein Personen-Scoring-Modell entwickelt und verwendet werden?

Sie haben vielleicht viele Leads in Ihrer Datenbank, aber woher wissen Sie, welche jetzt bereit sind, Ihre Produkte und Services zu kaufen? Da Ihr Marketing-Team die Lead-Qualität und die Verkaufsbereitschaft optimieren möchte, kommt hier das Scoring-Modell ins Spiel.

Wenn Sie Personen in Ihrer Marketo Engage-Datenbank bewerten, können Sie messen, wie qualifiziert Ihre generierten Leads sind, und Kriterien festlegen, nach denen sie verkaufsbereit sind. Auf diese Weise kann sich Ihr Vertriebsteam auf die Leads konzentrieren, die am wahrscheinlichsten geschlossen werden, während das Marketing-Team die anderen Personen in der Datenbank über seine Marketing-Programme weiterhin unterstützt.

## Übung 1: Ermittlung des Käuferinteresses mit Verhaltenscores

Die Verhaltens-Bewertung gibt nachverfolgbaren Aktionen eines potenziellen Kunden einen numerischen Wert, der auf Interesse an Ihren Produkten und Services und Kaufabsicht hinweist. Beispielsweise ist der Besuch der Website interessant, und der Besuch der Preisseite kann absichtlich sein. Dagegen kann der Besuch der Karriereseite darauf hindeuten, dass die Person keinen Kauf tätigt.

**Schritt 1**: Erstellen Sie eine Liste der Aktivitäten potenzieller Kunden, die für Ihren Verkaufsprozess wichtig sind oder für Ihr Unternehmen von Nutzen sind. Es kann hilfreich sein, mit Ihrem Verkaufs-Team zusammenzuarbeiten, um zu ermitteln, welche Aktivitäten darauf hindeuten, dass ein Lead eine Kaufabsicht hat. Auf diese Weise können Sie die Kriterien an den Vertrieb anpassen und basierend auf der Beobachtung abgeschlossener Abschlüsse Prioritäten setzen. Im Folgenden finden Sie einige empfohlene Fragen, die Sie Ihrem Verkaufsteam stellen können:

* Welche Aktivitäten deuten auf einen guten oder schlechten Lead hin?
* Welche Art von Inhalten, die von einem Lead genutzt werden, haben eine stärkere Kaufabsicht?

**Schritt 2** - Listet Aktionen auf, die darauf hinweisen, dass ein potenzieller Kunde nicht an Ihrem Produkt interessiert ist. Stellen Sie sicher, dass Sie Aktivitäten auflisten, die über Marketo Engage nachverfolgt werden können.

**Beispiel 1a - Aktivitäten, die eine Kaufabsicht anzeigen**

| **Aktivitäten, die eine Kaufabsicht anzeigen** | **Aktivitäten, die KEINE Kaufabsicht anzeigen** |
| --- | --- |
| Preisseite besuchen | Keine Interaktion in den letzten 90 Tagen |
| An jährlicher Kundenveranstaltung teilnehmen | Karriereseite besuchen |
| Anmeldung zum Webinar | Abo-Stornierungen |
| Whitepaper herunterladen |     |
| Füllen Sie das Demoformular für Anfragen aus |     |

**Schritt 3** - Analyse und Auswahl eines Schwellenwerts für die Übergabe von Verkäufen.

* Sobald ein Lead ausreichend Interesse zeigt, indem Sie einige der in Schritt 1 definierten Aktivitäten durchführen, und der Gesamtwert diesen Schwellenwert überschreitet, werden Sie ihn an den Verkauf übergeben. Dieser Schwellenwert ist einfach eine Zahl, die dabei hilft, einen Benchmark für die Bewertungen festzulegen, die Sie den einzelnen Verhaltensweisen zuweisen.
* Der Schwellenwert sollte groß genug sein, damit eine Person mehrere Interaktionen mit Ihrer Marke durchführen muss, um ihn zu erreichen. Beispielsweise ist eine geöffnete E-Mail wahrscheinlich kein ausreichender Qualifizierer. Wenn Sie gerade erst begonnen haben, versuchen Sie, mit einem Schwellenwert von 100 zu arbeiten und Ihre Person von dort aus zu ermitteln.
* Ob Sie einen hohen oder einen niedrigen Schwellenwert festlegen, hängt davon ab, welche Leiter Ihr Vertriebsteam am meisten daran interessiert ist, Geschäftsmöglichkeiten zu erhalten und zu entwickeln. Wenn Sie Daten über Ihre letzten Verkaufsangebote haben, analysieren Sie diese und sehen Sie, welche Aktionen die Personen bei erfolgreichen Angeboten unternommen haben. Auf diese Weise können Sie ermitteln, wie viele Kontaktpunkte in einen qualifizierten Vertriebs-Lead eingehen, und von dort aus extrapolieren, wie hoch Ihre Schwellenwertanzahl sein sollte.

**Beispiel 1b - Schwellenwert für Verkaufsübergabe:**

| Durchschnittliche Anzahl an Touchpoints für qualifizierten Lead | 4 |
| --- | --- |
| Schwelle für die Übergabe von Verkäufen | 50 |

**Schritt 4** - Jeder in „Beispiel 1a - Aktivitäten, die eine Kaufabsicht anzeigen“ aufgelisteten Aktivität einen Score zuweisen.

* Verwenden Sie einen positiven Verhaltens-Score für die Aktivitäten, die Interesse zeigen, um den Gesamt-Lead-Score eines Interessenten zu steigern, und einen negativen Score, um Desinteresse anzuzeigen.
* Bestimmen Sie anhand Ihres Schwellenwerts aus „Beispiel 1b - Schwellenwert für die Verkaufsübergabe“ als Benchmark Ihr Verhalten in Bezug auf die Wichtigkeit ihrer Aktionen. Interessenten, die eine Demo anfordern, sollten sich beispielsweise direkt an den Verkauf wenden. Am sinnvollsten ist es, dieser Aktion einen Punktwert zuzuweisen, der dem Schwellenwert für die Übergabe an den potenziellen Kunden entspricht. In der Zwischenzeit ist das Herunterladen eines Whitepapers nicht so ein starker Indikator für Kaufinteresse und sollte daher weniger Punkte wert sein.

**Beispiel 1c - Bewertungsaktivitäten, die eine Kaufabsicht anzeigen:**

| Schwellenwert für die Verkaufsübergabe = 50 Punkte |     |
| --- | --- |
| Aktivität | Ergebnis |
| „Demo-Formular anfordern“ ausgefüllt | +50 |
| Keine Interaktion in den letzten 90 Tagen | \-10 |
| Whitepaper herunterladen | +5 |
| Besuchen Sie uns auf einer Messe | +15 |

**Schritt 5** - Denken Sie daran, dass die Bewertung ein iterativer Prozess ist! Überprüfen und passen Sie Bewertungen und Schwellenwerte kontinuierlich an, während Sie weitere Daten für die Analyse sammeln.

## Übung 2: Identifizieren der richtigen Anpassung an demografische Bewertungen

Nachdem Sie nun die Aktivitäten definiert haben, die auf Ihre Kaufabsicht hinweisen, sollten Sie das Scoring-Modell mit Ihren Idealprofilen für Interessenten abschließen. Um festzustellen, ob ein Interessent für weitere Verkaufsgespräche am besten geeignet ist, ist es wichtig, zusätzlich zum Verhaltenswert demografische Bewertungen zuzuweisen, damit das Modell dazu beiträgt, die besten Leads in Bezug auf Anpassungsfähigkeit und Absicht zu ermitteln.

**Schritt 1** - Erstellen Sie eine Liste mit Merkmalen für Ihre idealen Interessenten.

* Erwägen Sie, Attribute wie Branche, Unternehmen, Abteilung und Rolle aufzulisten. Stellen Sie sicher, dass diese Merkmale den verfügbaren demografischen Feldern in Ihrer Marketo Engage-Instanz entsprechen.
* Arbeiten Sie mit Ihrem Verkaufsteam zusammen, um zu ermitteln, welche Leads am häufigsten auf Verkaufsanfragen reagieren und welche wichtige Kontakte während der Vertriebschancen sind.
   * Es kann hilfreich sein, kürzlich abgeschlossene Opportunities zu analysieren, um zu sehen, welche Eigenschaften Ihre besten Kunden haben. So wird beispielsweise
      * Durch das Durchforschen von verschlossenen verlorenen Gelegenheiten nach Mustern können Sie demografische Daten finden, die Sie vermeiden möchten.
      * Identifizieren Sie Entscheidungsträger und interne Champions, die Ihre Verkaufsbemühungen vorantreiben. Tauchen Sie tief in die Daten ein und bringen Sie Ihre Ergebnisse in einen Workshop mit einigen Ihrer Vertriebsmitarbeiter ein, um Ihre Schlussfolgerungen zu validieren oder zu verfeinern.
   * Sie können Ihr Vertriebsteam auch mit den folgenden Beispielfragen interviewen:
      * Mit welcher Abteilung beschäftigen sie sich normalerweise?
      * Was sind die Berufsbezeichnungen der Personen, die an Produktdemos beteiligt sind, und wer sind die Personen, die den Kauf abzeichnen müssen?

**Beispiel 2a - Ideale Merkmale des potenziellen Kunden**

| **Kategorie** | **Ideale Merkmale des potenziellen Kunden** |
| --- | --- |
| Branche | Luft- und Raumfahrt, verarbeitendes Gewerbe |
| Unternehmensgröße | 100 - 999, 1.000 - 9.999 |
| Stellenbezeichnung | Director, Vice President, C-Level |
| Abteilung | STD |

**Schritt 2** - Weisen Sie jedem Merkmal einen Wert entsprechend seiner Relevanz in Ihrem idealen Interessentenprofil zu. Verwenden Sie positive Werte für wünschenswerte Eigenschaften und negative Werte für Eigenschaften, die den Lead weniger gut für Ihr Produkt geeignet machen.

**Beispiel 2b - Bewertung idealer und unerwünschter Merkmale potenzieller Kundinnen und Kunden**

| **Merkmal** | **Ergebnis** |
| --- | --- |
| Industrie - Luft- und Raumfahrt | +10 |
| Industrie - Verarbeitendes Gewerbe | +5 |
| Unternehmensgröße - 100 - 999 | +5 |
| Unternehmensgröße - 1.000 - 9.999 | +10 |
| Unternehmensgröße - &lt;10 | \-10 |

## Übung 3: Integration lokaler Flexibilität in Ihr Scoring-Modell

Mit den grundlegenden verhaltensbezogenen und demografischen Bewertungsmodellen, die Sie abgeschlossen haben, können Sie es auf die nächste Ebene bringen, indem Sie lokale Flexibilität zulassen. Geschäftswerte können in verschiedenen Märkten variieren, wenn ein Unternehmen global agiert. In der folgenden Übung erfahren Sie, wie Sie Scores anwenden können, um den tatsächlichen Geschäftswert der Lead-Aktivitäten oder -Merkmale in verschiedenen Situationen widerzuspiegeln.

Bevorzugen Sie eine Videoeinführung für diese Übung? Melde dich als Marketo Engage-Champion an Katja Keesom zeigt, wie man lokale Flexibilität in das Scoring-Modell einbaut.

>[!VIDEO](https://video.tv.adobe.com/v/3426914/?learn=on)

**Schritt 1** - Nehmen Sie die Aktivitäten und Merkmale aus den Übungen 1 und 2 und bestimmen Sie für jeden Artikel, ob sie nach Standort oder Produktlinie variieren.

**Beispiel 3a - Signale auf globalen und lokalen Märkten:**

| **Signal** | **Global** | **local** |
| --- | --- | --- |
| Aktivitäten | <ul><li>Formular „Demo anfordern“ ausgefüllt</li><li>Keine Interaktion in den letzten 90 Tagen (ca. 3 Monate)</li></ul> | <ul><li>Besuchen Sie uns auf der Messe</li><li>Whitepaper herunterladen</li></ul> |
| Eigenschaften | <ul><li>Abteilung</li><li>Stellenbezeichnung</li></ul> | <ul><li>Branche</li><li>Unternehmensgröße</li></ul> |

**Schritt 2** - Definieren Sie Ihre Scoring-Matrix für lokale Märkte:

* Richten Sie eine andere Matrix für demografische und Verhaltenselemente ein.
* Bestimmen Sie die Themen mit Prioritäten, zu denen Sie das lokale Team um Beiträge bitten können.
* Anzahl der Werte definieren, die zur Bewertung in den Themen verwendet werden
* Weisen Sie einzelne Werte zu, indem Sie den relativen Wert mit den globalen Werten abgleichen.
* Erwägen Sie die Definition gängiger Szenarien, in denen potenzielle Kunden mit Ihrer Marke interagieren, und testen Sie Ihre Gesamtbewertung für sie.
   * Eine gängige Journey besteht beispielsweise darin, dass eine Person Ihre Website auf einer Inhaltsseite aufruft und dann auf eine Produktseite klickt, um eine Broschüre herunterzuladen. Sie richten eine Webinar-Einladung an die Zielgruppe aus. Diese antwortet mit der Registrierung, nimmt jedoch nicht teil. Überlegen Sie, ob Ihr Verkauf bereits mit dieser Person sprechen möchte oder nicht, und bewerten Sie, ob Ihr Scoring-Modell diese potenziellen Kunden zum richtigen Gesamtergebnis bringt, um dieses Interessensniveau widerzuspiegeln.

**Beispiel 3b - Demografische Bewertungsmatrix:**

| **Demografische Matrix** | **Priorität 1** | **Priorität 2** | **Priorität 3** |
| --- | --- | --- | --- |
| Hohe Werte | 20 Punkte | 10 Punkte | 7 Punkte |
| Medium-Werte | 10 Punkte | 7 Punkte | 3 Punkte |
| Niedrige Werte | 5 Punkte | 3 Punkte | 1 Punkt |

**Schritt 3** - Sammeln Sie Beiträge von Ihren lokalen oder regionalen Vertriebsteams, um eine ganzheitliche Sicht zu entwickeln. Sie werden feststellen, dass in Beispiel 3c keine individuellen Bewertungen enthalten sind. Auf diese Weise kann sich das Vertriebsteam während des Überprüfungsprozesses auf den relativen Wert der verschiedenen Themen konzentrieren. Sie sollten Ihr vollständiges Modell jedoch als Hintergrundmaterial für andere Marketo Engage-Administratoren dokumentieren lassen.

* Sperren Sie, was nicht für die globale Konsistenz angepasst werden kann (hier in der Spalte „Thema implementieren„).
* Markieren Sie (hier in den Spalten „Priorität“ und „Score„), was an lokale Einflüsse angepasst werden kann.

**Beispiel 3c - Relativer Wert der Bewertungsthemen:**

<table>
 <tr>
    <th>#</th>
    <th>Thema implementieren</th>
    <th>Demografisch/Verhaltensbezogen</th>
    <th>Thema</th>
    <th>Priorität</th>
    <th>Werte</th>
    <th>Scores</th>
 </tr>
 <tr>
    <td rowspan="6">1</td>
    <td rowspan="6"><b>ERFORDERLICH</b></td>
    <td rowspan="6">Demografisch</td>
    <td rowspan="6">Branche</td>
    <td rowspan="6"><b>2</b></td>
    <td>Technologie</td>
    <td><b>Hoch</b></td>
  </tr>
  <tr>
    <td>Mode</td>
    <td><b>Hoch</b></td>
  </tr>
  <tr>
    <td>Einzelhandel</td>
    <td><b>Mittel</b></td>
  </tr>  
  <tr>
    <td>Fertigung</td>
    <td><b>Mittel</b></td>
  </tr>
  <tr>
    <td>Gesundheitswesen</td>
    <td><b>Niedrig</b></td>
  </tr>
  <tr>
    <td>...</td>
    <td><b>Niedrig</b></td>
  </tr>
<tr>
    <td rowspan="3">2</td>
    <td rowspan="3"><b>Ja</td>
    <td rowspan="3">Demografisch</td>
    <td rowspan="3">Unternehmensgröße (Mitarbeiter)</td>
    <td rowspan="3"><b>3</td>
    <td>&gt;1000 Mitarbeiter</td>
    <td><b>Hoch</td>
  </tr>
  <tr>
    <td>250-999 Beschäftigte</td>
    <td><b>Mittel</td>
  </tr>
  <tr>
    <td>1-249 Mitarbeiter</td>
    <td><b>Niedrig</td>
  </tr>  
<tr>
    <td rowspan="3">3</td>
    <td rowspan="3"><b>Nein</b></td>
    <td rowspan="3">Verhalten</td>
    <td rowspan="3">Seitenbesuche auf Ihrer Website</td>
    <td rowspan="3"><b>2</b></td>
    <td>&gt;Produktinformationsseiten</td>
    <td><b>Niedrig</b></td>
  </tr>
  <tr>
    <td>Preisseiten</td>
    <td><b>Mittel</b></td>
  </tr>
  <tr>
    <td>Demo-Anfrageseite</td>
    <td><b>Hoch</b></td>
  </tr>
</table>

## Wie geht es weiter?

* Laden Sie das [Übungsblatt zur Personenbewertung](./assets/build-person-scoring-model-and-local-flexibility-in-adobe-marketo-engage.docx){target="_blank} herunter, um Ihr Bewertungsmodell offline zu entwickeln.
* Erstellen Sie Ihre Personenbewertung in Marketo Engage. Lesen Sie dieses [Tutorial](https://experienceleague.adobe.com/de/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch){target="_blank} und [Demo](https://experienceleague.adobe.com/de/docs/events/marketo-and-mochas-recordings/2023/lead-scoring){target="_blank}, um loszulegen. Sie können ein Lead/Personen-Bewertungsprogramm [Vorlage](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program){target="_blank} aus der Marketo Engage-Referenzbibliothek importieren, um die Programmerstellung zu beschleunigen.
* Erstellen Sie zwei Versionen des Scoring-Programms:
   * Ein zentrales Programm, das die gesamte Bewertung ausführt, die nicht lokal aktualisiert werden kann.
   * Eine lokale Kopie mit den konfigurierbaren Bewertungselementen.
* Richten Sie Ihre Scoring-Werte als Token innerhalb Ihres Scoring-Programms ein. Dadurch wird Konsistenz sichergestellt, auch wenn Sie die Bewertungen im Laufe der Zeit anpassen.
   * Ein gängiges Beispiel für tokenisierte Scores ist ein Token für hochwertige Aktivitäten, die Ihren Schwellenwert automatisch erreichen, z. B. die Anforderung einer Demo oder die Buchung eines Meetings mit Ihrem Verkaufsteam. Selbst wenn Sie die erforderliche Mindestpunktzahl ändern, um Ihren Schwellenwert zu erreichen, können Sie alle Aktivitäten mit hohem Wert einfach gleichzeitig aktualisieren, indem Sie ein Token aktualisieren.
* Passen Sie Ihre lokale Smart-Kampagne für jeden Standort an:
   * Legen Sie fest, welche demografischen und verhaltensbezogenen Aktivitäten nur einmal bewertet werden sollen (d. h. die Branche) und welche jedes Mal bewertet werden sollen, wenn sich ein potenzieller Kunde qualifiziert (d. h. an einem Webinar teilgenommen hat). Dadurch wird sichergestellt, dass potenzielle Kontakte, die durch die Datenwertänderung ausgelöst werden, für den Verkauf relevant sind.
   * Achten Sie darauf, dass sich Ihre Auswahl gegenseitig ausschließt.
   * Nehmen Sie in beiden Flussschritten Aktualisierungen vor, damit der Personenwert auf die gleiche Weise wie der demografische Wert aktualisiert wird. Auf diese Weise bleibt die Personenbewertung auf einer Linie mit der Kombination aus Verhaltensbewertung und demografischem Wert.
* Testen Sie die intelligente Kampagne, sobald Sie die Erstellung Ihres Programms abgeschlossen haben. Gehen Sie beispielsweise zu Ihrem Demoformular, füllen Sie es mit einer Test-E-Mail aus und überprüfen Sie das Ergebnis Ihrer Testperson in der [Marketo Engage-Datenbank](https://experienceleague.adobe.com/de/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring#step-view-the-person-info){target="_blank}.
* Nachdem Sie Ihr Modell erstellt haben, sollten Sie einen Warnhinweis einrichten, der an den Verkauf gesendet wird, sobald die Punktzahl der Person Ihren Schwellenwert für die Übergabe des Verkaufs erreicht hat. Weitere Informationen zum Einrichten eines Warnhinweises finden Sie in diesem [Tutorial](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert){target="_blank}.

### Autoren

{{christina-zuniga}}

{{katja-keesom}}

{{amy-chiu}}
