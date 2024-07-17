---
title: Erstellen von Personenbewertungsmodellen für Marketo Engage-Programme
description: Mit Adobe Marketo Engage können Sie Ihre Scoring-Modelle von Grund auf erstellen. Bevor Sie direkt in die Marketo Engage springen, um Ihre Scoring-Programme zu erstellen, müssen Sie die wesentlichen Punktfelder wie demografische Punktzahl, Verhaltensergebnis und Personen-Gesamtbewertung einrichten. Erfahren Sie mehr über die Strategien, die von Marketo Engage Champions zur Entwicklung von Scoring-Modellen verwendet werden, die Ihr Unternehmen benötigt.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14810
thumbnail: KT-14810.jpeg
exl-id: 73976144-f02b-4423-9b4b-410330117ba9
source-git-commit: e0d0c47eec98b7259363350d331ba69bbcaaa64b
workflow-type: tm+mt
source-wordcount: '2111'
ht-degree: 2%

---

# Erstellen eines Personen-Scoring-Modells

Mit der Personensortierung können Sie die Personen identifizieren, die am stärksten mit Ihrem Unternehmen verbunden sind, und Ihr ideales Kundenprofil darstellen, sodass Sie diese Leads mit Ihrem Verkaufsteam teilen und Geschäfte schließen können. Gemeinsam mit dem Vertrieb legen Sie fest, welche Leads Sie an sie übergeben möchten, indem Sie ein Lead/Person-Scoring-Programm in Adobe Marketo Engage verwenden. Dies kann entweder durch eine minimale verhaltensbasierte Bewertung, demografische Auswertung oder beides bestimmt werden.

In diesem Tutorial führen wir Sie durch drei Übungen, die von Marketo Engage Champions Christina Zuniga und Katja Keesom vorgeschlagen wurden. Im Folgenden erfahren Sie, welche Aktivitäten und Merkmale wichtige Indikatoren dafür sind, dass ein Interessent an einem Kauf interessiert ist (verhaltensbasierte Bewertung) und für Sie geeignet ist (demografische Bewertung), und berücksichtigen die Nuancen der Märkte.

## Warum entwickeln und verwenden Sie ein Personenbewertungsmodell?

Sie haben vielleicht viele Leads in Ihrer Datenbank, aber wie wissen Sie, welche Sie jetzt bereit sind, Ihre Produkte und Dienstleistungen zu kaufen? Da Ihre Marketing-Organisation die Lead-Qualität und die Verkaufsbereitschaft optimieren möchte, kommt hier das Scoring-Modell zum Tragen.

Indem Sie Personen in Ihrer Marketo Engage-Datenbank auswerten, können Sie messen, wie qualifiziert Ihre generierten Leads sind, und Kriterien dafür festlegen, wann sie umsatzbereit sind. Dadurch kann sich Ihr Verkaufsteam auf die Leads konzentrieren, die am ehesten geschlossen werden, während das Marketing-Team die anderen Personen in der Datenbank über seine Marketing-Programme weiter pflegt.

## Übung 1 - Bestimmung des Kaufinteresses mit Verhaltensbewertungen

Die Verhaltensscoring bietet nachverfolgten Aktionen, die ein Interessent unternimmt, einen numerischen Wert, der das Interesse an Ihren Produkten und Dienstleistungen und die Absicht zum Kauf angibt. Zum Beispiel zeigt der Besuch der Website Interesse und der Besuch der Preisseite zeigt möglicherweise die Absicht. Im Gegensatz dazu kann der Besuch der Karriereseite darauf hinweisen, dass die Person nicht kaufen wird.

**Schritt 1** - Erstellen Sie eine Liste der potenziellen Aktivitäten, die für Ihren Verkaufsprozess von Bedeutung sind oder für Ihre Organisation von Nutzen sind. Es kann hilfreich sein, mit Ihrem Verkaufsteam zusammenzuarbeiten, um festzustellen, welche Aktivitäten darauf hindeuten, dass ein Lead die Kaufabsicht hat. So können Sie die Kriterien an den Umsatz anpassen und anhand der Beobachtung geschlossener Geschäfte Prioritäten setzen. Im Folgenden finden Sie einige Fragen, die Sie an Ihr Verkaufsteam richten können:

* Welche Aktivitäten weisen auf einen guten oder einen schlechten Ausgang zu Ihnen hin?
* Welche Art von Inhalten, die von einem Lead konsumiert werden, hat eine stärkere Kaufabsicht?

**Schritt 2** - Aktionen auflisten, die darauf hinweisen, dass ein Interessent nicht an Ihrem Produkt interessiert ist. Stellen Sie sicher, dass Sie Aktivitäten auflisten, die über Marketo Engage verfolgt werden können.

**Beispiel 1a - Aktivitäten, die die Absicht angeben, zu kaufen**

| **Aktivitäten, die die Absicht angeben, zu kaufen** | **Aktivitäten, die KEINE Absicht zum Kauf angeben** |
| --- | --- |
| Seite mit Besucherpreisen | Keine Interaktion in den letzten 90 Tagen |
| Jahrestagung des Kundenereignisses | Besuchslaufbahn-Seite |
| Webinar registrieren | Abo-Stornierungen |
| Whitepaper herunterladen |     |
| Demoformular für Anfrage ausfüllen |     |

**Schritt 3** - Analysieren und wählen Sie einen Schwellenwert für die Übergabe aus dem Verkauf.

* Sobald ein Lead durch Ausführung einiger der in Schritt 1 definierten Aktivitäten genügend Interesse zeigt und das Gesamtergebnis diesen Schwellenwert überschreitet, übergeben Sie ihn an den Umsatz. Dieser Schwellenwert ist einfach eine Zahl, mit der Sie einen Benchmark für die Bewertungen festlegen können, die Sie einzelnen Verhaltensweisen zuweisen.
* Ihre Schwelle sollte groß genug sein, sodass eine Person mehrere Interaktionen mit Ihrer Marke abschließen muss, um sie erreichen zu können. Beispielsweise ist es unwahrscheinlich, dass eine E-Mail-Öffnung einen ausreichenden Qualifikator aufweist. Wenn Sie gerade angefangen haben, versuchen Sie, mit einem Schwellenwert von 100 zu arbeiten und Ihre Person von dort aus zu bewerten.
* Die Festlegung eines hohen oder niedrigen Schwellenwerts hängt davon ab, welche Führungsrolle Ihr Verkaufsteam am meisten daran interessiert, Geschäftsmöglichkeiten zu erhalten und zu entwickeln. Wenn Sie über vorhandene Daten zu Ihren jüngsten Verkaufsgeschäften verfügen, analysieren Sie diese und sehen Sie, welche Aktionen Kunden bei erfolgreichen Geschäften durchgeführt haben. Auf diese Weise können Sie ermitteln, wie viele Touchpoints in einen qualifizierten Verkaufs-Lead eingehen, und können von dort aus die gewünschte Schwellenzahl extrapolieren.

**Beispiel 1b - Schwellenwert für die Verkaufshandlung:**

| Durchschnittliche Anzahl der Touchpoints für qualifizierten Lead | 4 |
| --- | --- |
| Schwellenwert für die Übergabe an den Vertrieb | 50 |

**Schritt 4** - Weisen Sie jeder Aktivität eine Punktzahl zu, die unter &quot;Beispiel 1a - Aktivitäten aufgeführt ist, die auf die Absicht zum Kauf hinweisen&quot;aufgeführt ist.

* Verwenden Sie einen positiven Verhaltensergebnis für die Aktivitäten, die das Interesse anzeigen, um den Gesamt-Interessenergebnis eines Interessenten zu steigern, und einen negativen Wert, der auf Desinteresse hinweist.
* Legen Sie anhand des Schwellenwerts von &quot;Beispiel 1b - Schwellenwert für die Übergabe von Verkaufszahlen&quot;Ihre Verhaltensergebnisse in Bezug auf die Wichtigkeit ihrer Aktionen fest. Beispielsweise sollten potenzielle Kunden, die eine Demo anfordern, direkt zum Verkauf gehen. Am sinnvollsten ist es, dieser Aktion einen Punktwert zuzuweisen, der Ihrem potenziellen Übergabeschwellenwert entspricht. Inzwischen ist der Download eines Whitepaper kein so starker Indikator für Kaufinteressen und sollte daher weniger Punkte wert sein.

**Beispiel 1c - Scoring-Aktivitäten, die den Kaufabsicht angeben:**

| Schwellenwert für Verkaufstransfer = 50 Punkte |     |
| --- | --- |
| Aktivität | Ergebnis |
| &quot;Demoformular anfordern&quot;ausgefüllt | +50 |
| Keine Interaktion in den letzten 90 Tagen | \-10 |
| Whitepaper herunterladen | +5 |
| Besuchen Sie uns auf einer Messe | +15 |

**Schritt 5** - Beachten Sie, dass Scoring ein iterativer Prozess ist! Überprüfen und passen Sie kontinuierlich Bewertungen und Schwellenwerte an, wenn Sie mehr Daten für die Analyse sammeln.

## Übung 2 - Ermittlung des richtigen Passes mit demografischen Werten

Nachdem Sie nun die Aktivitäten definiert haben, die auf die Kaufabsicht hinweisen, sollten Sie das Scoring-Modell mit Ihren Idealprojekten abschließen. Um festzustellen, ob ein Interessent für weitere Verkaufsgespräche geeignet ist, müssen demografische Werte zusätzlich zu den Verhaltenswerten zugewiesen werden, damit das Modell bei der Ermittlung der besten Leads hinsichtlich Eignung und Absicht hilft.

**Schritt 1** - Erstellen Sie eine Liste der Eigenschaften für Ihre idealen Perspektiven.

* Erwägen Sie die Auflistung von Attributen wie Branche, Unternehmen, Abteilung und Rolle. Stellen Sie sicher, dass diese Eigenschaften den verfügbaren demografischen Feldern in Ihrer Marketo Engage-Instanz entsprechen.
* Arbeiten Sie mit Ihrem Verkaufsteam zusammen, um zu bestimmen, welche Leads am meisten auf Kundenanfragen reagieren und wichtige Kontakte bei Verkaufsmöglichkeiten darstellen.
   * Es kann hilfreich sein, kürzlich geschlossene Chancen zu analysieren, um zu sehen, welche Merkmale Ihre besten Kunden haben. So wird beispielsweise
      * Wenn Sie sich durch geschlossene verlorene Möglichkeiten für Muster bewegen, können Sie demografische Daten finden, die Sie vermeiden möchten.
      * Identifizieren Sie Entscheidungsträger und interne Champions, die Ihre Verkaufsbemühungen vorantreiben. Machen Sie sich mit den Daten vertraut und bringen Sie Ihre Ergebnisse in einen Workshop mit einigen Ihrer Vertriebsteams, um Ihre Schlussfolgerungen zu validieren oder zu verfeinern.
   * Sie können Ihr Verkaufsteam auch mit den folgenden Beispielfragen befragen:
      * Mit welcher Abteilung sind sie normalerweise beschäftigt?
      * Wie lauten die Berufstitel der Personen, die an Produktdemos beteiligt sind und wer sind die Personen, die beim Kauf abmelden müssen?

**Beispiel 2a - Ideal Prospekt-Merkmale**

| **Kategorie** | **Ideal Prospect Characters** |
| --- | --- |
| Branche | Luft- und Raumfahrt, Produktion |
| Firmengröße | 100 - 999, 1.000 - 9.999 |
| Stellenbezeichnung | Director, Vizepräsident, C-Level |
| Abteilung | HR |

**Schritt 2** - Weisen Sie jedem Merkmal eine Punktzahl zu, die seiner Relevanz in Ihrem idealen Prospektprofil entspricht. Verwenden Sie positive Werte für wünschenswerte Eigenschaften und negative Werte für Eigenschaften, die den Lead weniger passend für Ihr Produkt machen.

**Beispiel 2b - Zuweisen von Bewertungen zu idealen und unerwünschten potenziellen Merkmalen**

| **CharacterIST** | **Ergebnis** |
| --- | --- |
| Industrie - Luft- und Raumfahrt | +10 |
| Industrie - Produktion | +5 |
| Unternehmensgröße - 100 - 999 | +5 |
| Unternehmensgröße - 1.000 - 9.999 | +10 |
| Unternehmensgröße - &lt;10 | \-10 |

## Übung 3 - Integrieren der lokalen Flexibilität in Ihr Scoring-Modell

Mit den grundlegenden verhaltensbezogenen und demografischen Bewertungsmodellen, die Sie abgeschlossen haben, können Sie es auf die nächste Stufe bringen, indem Sie lokale Flexibilität zulassen. Geschäftswerte können auf verschiedenen Märkten variieren, wenn eine Organisation global tätig ist. In der folgenden Übung erfahren Sie, wie Sie Bewertungen anwenden, um den tatsächlichen Geschäftswert der Lead-Aktivitäten oder -Merkmale in verschiedenen Situationen widerzuspiegeln.

Magst du eine Videoeinführung für diese Übung? Tune in als Marketo Engage Champion Katja Keesom demonstriert, wie man lokale Flexibilität in das Scoring-Modell einbaut.

>[!VIDEO](https://video.tv.adobe.com/v/3426914/?learn=on)

**Schritt 1** - Nehmen Sie die Aktivitäten und Merkmale aus den Übungen 1 und 2 und bestimmen Sie für jedes Element, ob sie je nach Standort oder Produktlinie variieren.

**Beispiel 3a - Signale auf globalen und lokalen Märkten:**

| **Signal** | **Global** | **local** |
| --- | --- | --- |
| Aktivitäten | <ul><li>Ausfüllen des Formulars &quot;Demo anfordern&quot;</li><li>Keine Interaktion in den letzten 90 Tagen (etwa 3 Monate)</li></ul> | <ul><li>Besuchen Sie uns auf der Messe</li><li>Whitepaper herunterladen</li></ul> |
| Eigenschaften | <ul><li>Abteilung</li><li>Stellenbezeichnung</li></ul> | <ul><li>Branche</li><li>Firmengröße</li></ul> |

**Schritt 2** - Definieren Sie Ihre Scoring-Matrix für lokale Märkte:

* Richten Sie eine andere Matrix für demografische Elemente und Verhaltenselemente ein.
* Legen Sie die Prioritäten fest, zu denen Sie die Beiträge des lokalen Teams anfordern können.
* Definieren Sie die Anzahl der Werte, die zur Bewertung in Ihren Themen verwendet werden.
* Weisen Sie einzelne Werte zu, indem Sie den relativen Wert an globalen Werten ausrichten.
* Erwägen Sie die Definition gängiger Szenarien, in denen potenzielle Kunden mit Ihrer Marke interagieren und Ihre Gesamtbewertung für sie testen.
   * Eine häufig angezeigte potenzielle Journey wäre beispielsweise, dass eine Person Ihre Website auf einer Inhaltsseite aufruft, dann durch eine Produktseite klickt und eine Broschüre herunterlädt. Sie würden sie mit einer Webinar-Einladung ansprechen und sie antworten darauf, indem sie sich registrieren, aber nicht teilnehmen. Überlegen Sie, ob Ihre Verkäufe bereits mit dieser Person sprechen möchten oder nicht, und beurteilen Sie, ob Ihr Scoring-Modell diese Perspektiven auf das richtige Gesamtergebnis bringt, um dieses Interessensniveau widerzuspiegeln.

**Beispiel 3b - Demografische Bewertungsmatrix:**

| **Demografische Matrix** | **Priorität 1** | **Priorität 2** | **Priorität 3** |
| --- | --- | --- | --- |
| Hohe Werte | 20 Punkte | 10 Punkte | 7 Punkte |
| Medium-Werte | 10 Punkte | 7 Punkte | 3 Punkte |
| Niedrige Werte | 5 Punkte | 3 Punkte | 1 Punkt |

**Schritt 3** - Erfassen Sie Beiträge von Ihren lokalen oder regionalen Vertriebsteams, um eine ganzheitliche Sicht zu entwickeln. Sie werden feststellen, dass in Beispiel 3c keine einzelnen Punkte enthalten sind. Dadurch kann sich das Verkaufsteam während des Überprüfungsprozesses auf den relativen Wert der verschiedenen Themen konzentrieren. Sie sollten Ihr vollständiges Modell jedoch als Hintergrundmaterial für andere Marketo Engage-Administratoren dokumentieren lassen.

* Sperren Sie das, was nicht für globale Konsistenz angepasst werden kann (hier in der Spalte &quot;Thema implementieren&quot;).
* Markieren Sie (hier in den Spalten &quot;Priorität&quot;und &quot;Punktzahl&quot;), was für lokale Einflüsse angepasst werden kann.

**Beispiel 3c - Relativer Wert der Scoring-Themen:**

<table>
 <tr>
    <th>#</th>
    <th>Implementieren des Themas</th>
    <th>Demografie/Verhaltensweise</th>
    <th>Thema</th>
    <th>Priorität</th>
    <th>Werte</th>
    <th>Bewertungen</th>
 </tr>
 <tr>
    <td rowspan="6">1</td>
    <td rowspan="6"><b>ERFORDERLICH</b></td>
    <td rowspan="6">Demografie</td>
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
    <td rowspan="3">Demografie</td>
    <td rowspan="3">Unternehmensgröße (Angestellte)</td>
    <td rowspan="3"><b>3</td>
    <td>&gt; 1000 Angestellte</td>
    <td><b>Hoch</td>
  </tr>
  <tr>
    <td>250-999 Beschäftigte</td>
    <td><b>Mittel</td>
  </tr>
  <tr>
    <td>1-249 Beschäftigte</td>
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
    <td>Preise für Seiten</td>
    <td><b>Mittel</b></td>
  </tr>
  <tr>
    <td>Demoanforderungsseite</td>
    <td><b>Hoch</b></td>
  </tr>
</table>

## Wie geht es weiter?

* Laden Sie das [Personen-Scoring-Übungsblatt](./assets/build-person-scoring-model-and-local-flexibility-in-adobe-marketo-engage.docx){target="_blank} herunter, um Ihr Scoring-Modell offline zu entwickeln.
* Erstellen Sie Ihre Personenbewertung im Marketo Engage. Sehen Sie sich dieses [Tutorial](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch){target="_blank} und das [Demo](https://experienceleague.adobe.com/en/docs/events/marketo-and-mochas-recordings/2023/lead-scoring){target="_blank} an, um zu beginnen. Sie können ein Lead-/Personen-Scoring-Programm [template](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program){target="_blank} aus der Marketo Engage-Referenzbibliothek importieren, um den Programmaufbau zu beschleunigen.
* Erstellen Sie zwei Versionen des Scoring-Programms:
   * Ein zentrales Programm, das alle Scoring-Vorgänge ausführt, die nicht lokal aktualisiert werden können.
   * Eine lokale Kopie mit den konfigurierbaren Scoring-Elementen.
* Richten Sie Ihre Scoring-Werte in Ihrem Scoring-Programm als Token ein. Dies sorgt für Konsistenz, selbst wenn Sie Bewertungen im Laufe der Zeit anpassen.
   * Ein gängiges Beispiel für tokenisierte Bewertungen ist ein Token für hochwertige Aktivitäten, die automatisch Ihren Schwellenwert erreichen, z. B. Anforderung einer Demo oder Buchung eines Treffens mit Ihrem Verkaufsteam. Selbst wenn Sie den Mindestwert ändern, der zum Erfüllen des Schwellenwerts erforderlich ist, können Sie alle Aktivitäten mit hohem Wert auf einmal aktualisieren, indem Sie ein Token aktualisieren.
* Passen Sie Ihre lokale Smart-Kampagne für jeden Standort an:
   * Bestimmen Sie, welche demografischen und verhaltensbezogenen Aktivitäten nur einmal bewertet werden sollen (d. h. Branche) und welche jedes Mal bewertet werden sollten, wenn sich ein Interessent qualifiziert (d. h. an einem Webinar teilgenommen hat). Dadurch wird sichergestellt, dass potenzielle Kontakte, die durch die Änderung des Datenwerts ausgelöst werden, für den Vertrieb relevant sind.
   * Stellen Sie sicher, dass sich Ihre Auswahlmöglichkeiten gegenseitig ausschließen.
   * Nehmen Sie Ihre Aktualisierungen in beiden Durchsatzschritten vor, damit die Personenergebnis auf die gleiche Weise wie die demografische Bewertung aktualisiert wird. Auf diese Weise bleibt die Personenbewertung in Übereinstimmung mit der Kombination aus Verhaltensergebnis und demografischem Ergebnis.
* Testen Sie die Smart-Kampagne, sobald Sie mit der Erstellung Ihres Programms fertig sind. Gehen Sie beispielsweise zu Ihrem Demoformular, füllen Sie es mit einer Test-E-Mail aus und überprüfen Sie den Punktstand Ihrer Testperson in der [Marketo Engage-Datenbank](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring#step-view-the-person-info){target="_blank}.
* Nachdem Sie Ihr Modell erstellt haben, sollten Sie eine Warnung einrichten, die an den Verkauf gesendet wird, sobald das Ergebnis der Person Ihren Schwellenwert für die Übergabe im Vertrieb erreicht hat. Weitere Informationen zum Einrichten eines Warnhinweises finden Sie in diesem [Tutorial](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert){target="_blank}.

### Autoren

{{christina-zuniga}}

{{katja-keesom}}

{{amy-chiu}}
