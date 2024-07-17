---
title: Erstellen einer Datenkultur und einer besseren Lösungsdesign-Referenz
description: Revolutionieren Sie Ihre Datenstrategie und stärken Sie Ihr Team bei der Erstellung eines soliden SDR-Dokuments (Solution Design Reference). Beseitigen Sie Messlücken und fördern Sie eine partizipative Datenkultur durch schrittweise Methoden.
feature: Implementation Basics
topic: Administration
role: User
level: Experienced
doc-type: Article
duration: 72000
last-substantial-update: 2024-04-25T00:00:00Z
jira: KT-15338
thumbnail: KT-15338.jpeg
exl-id: 99fcf68f-5698-4270-9055-ab224e6323a1
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 0%

---

# Erstellen einer Datenkultur und einer besseren Referenz zum Lösungsdesign

_Revolutionieren Sie Ihre Datenstrategie und ermächtigen Sie Ihr Team, ein solides Dokument zur Lösungsdesign-Referenz (Solution Design Reference, SDR) zu erstellen. Beseitigen Sie Messlücken und fördern Sie eine partizipative Datenkultur durch schrittweise Methoden._

Endlich ist es Zeit. Sie haben eine solide SZR zusammengestellt. Ein SDR ist das Handbuch, das Sie zur Implementierung Ihrer Metriken und Dimensionen verwenden. Du hast definiert, wie sie heißen, wenn sie feuern, und deine Entwickler lieben es. Sie haben den gesamten Bereitstellungsprozess durchlaufen, Akzeptanzkriterien geschrieben, Ihre Sprints durchlaufen, getestet und es ist fertig! Ihre Instanz von [!DNL Adobe Analytics] sollte Marketing- und Produktteams dazu bringen, zu feiern, während sie die Daten untersuchen, neue Enthüllungen über Ihre Kunden erhalten und alle Bereiche des Erfolgs und, naja, Bereiche mit geringerem Erfolg finden. Aber Sie hören nicht die Akoladen, die Sie erwartet haben.

Von einem Team hören Sie Beschwerden wie:

&quot;Warum kann ich die Konversionsrate für diesen Trichter nicht ermitteln?&quot;

&quot;Warum gibt es dafür keine Metrik?&quot;

&quot;Ich brauche mehr Details! Eine Metrik allein reicht nicht aus. Es gibt mindestens drei verschiedene Dimensionen, die ich für ein besseres Verständnis der Leistung benötige. Warum hast du sie nicht hineingesteckt?&quot;

Aber es ist das andere Team, das eine noch größere Sorge bereitet. Von ihnen hört man überhaupt nichts. Schlimmer noch: Sie sehen Diagramme, die eindeutig aus Ihrer alten Analyselösung entnommen wurden (die nicht mehr gepflegt wird und jeden Tag weiter in einen Sumpf von Abfall und schmutzigen Daten fällt). Ein Gefühl der Angst erfüllt Sie, wenn Sie die Entscheidungen betrachten, die mit diesem ursprünglichen Chaos getroffen werden könnten.

_Was ist schiefgelaufen?_

_Warum gibt es Lücken in der Messung?_

_Warum nehmen Ihre Teammitglieder das nicht an?_

Ich beginne, indem ich dich ein wenig aus dem Haken lasse. Es wird _always_ eine Revision geben. Wenn Ihre Site oder Anwendung komplex genug ist, um eine Enterprise Analytics-Lösung zu benötigen, wird Ihnen garantiert etwas fehlen. Aber in diesem Fall haben Sie nicht genug verpasst, um die Messlücken zu erklären, die ich beschreibe.

Was schiefgelaufen ist, ist viel schwieriger in eine Tabelle einzufügen. Im Grunde haben Sie Ihre erste Chance verpasst, eine partizipative Datenkultur aufzubauen, während Sie Ihre SDR erstellt haben.

Ich möchte Sie durch eine Methode führen, die meine Kollegen und ich entwickelt haben, um sowohl eine bessere SDR mit weniger Lücken zu erstellen als auch um Endbenutzer dazu zu bringen, über ihre neue Instanz von [!DNL Adobe Analytics] zu investieren (und sogar gelegentlich aufgeregt). Lassen Sie uns darüber sprechen, wie und warum Sie diese Methode in Erwägung ziehen sollten.

## Die

_Erfahren Sie mehr über die Messungskonferenz. Verwenden Sie eine Trichterzuordnung, um jeden Schritt Ihres Plans zu visualisieren. Erstellen Sie Modelle-Dashboards, die als Gruppe überprüft werden. Erstellen Sie ein Datenwörterbuch für Benutzer._

### Messungskonferenz

1. Treffen Sie Ihre Interessengruppen, entweder persönlich oder virtuell, um herauszufinden, was gemessen werden soll. Diese Sitzung sollte einige Führungskräfte umfassen.
1. Sie haben bereits offensichtliche Beispiele auf der Pinnwand in Kurznotizen, wie Umsatz, Vertrieb oder Leads, die wichtigsten Produktindikatoren (KPIs), von denen Sie wissen, dass sie gemessen werden. Wiederholen Sie diese Schritte mit Dimensionen wie angemeldetem Status, Produktkategorien oder Suchbegriffen.
1. Lassen Sie alle ihre eigenen Notizen hinzufügen und gruppieren Sie sie nach Bedarf.
1. Bitten Sie die Menschen, über die zu wählen, die sie für wichtig halten. Dies sind unbegrenzte Abstimmungen, da diese Metriken und Dimensionen wahrscheinlich von Bedeutung sind.
1. Weisen Sie für alle Metriken und Dimensionen mit geringen Stimmen die Interessengruppen, die sie gebeten haben, zu, warum diese Komponenten verwendet werden. Wenn ein guter Anwendungsfall vorliegt, behalten Sie diese Komponenten bei. Wenn es eine bessere Methode gibt, diese Daten zu erhalten, oder niemand erklären kann, wie diese Daten verarbeitet werden können, oder wenn ein anderer guter Grund besteht, die Metriken und Dimensionen zu entfernen, tun Sie dies.
1. Fügen Sie diese Metriken und Dimensionen zu Ihrer SDR hinzu, um sie zunächst von den beteiligten Benutzern zu überprüfen, die anwesend waren.

### Trichterzuordnung

1. Hier erhalten Sie eine Visualisierung aller Trichter, Schritt für Schritt mit jedem Status.
1. Nehmen Sie mit den Designern und Produktmanagern die einzelnen Schritte vor und besprechen Sie, was jeder für Erfolg in diesem Trichter hält. Ist es die Konversionsrate? Wählt sie einen bestimmten Pfad? Verwendet sie bestimmte Funktionen?
1. Stellen Sie Fragen dazu, welche Metriken und Dimensionen erforderlich sind, um die Trichterleistung bei jedem Schritt des Trichters und insgesamt zu verstehen.
1. Fügen Sie über jedem Schritt des Trichters die Metriken und Dimensionen hinzu, die bei diesem Schritt gemessen werden, einschließlich der berechneten Metriken.
1. Schreiben Sie zu Beginn jedes Trichters die Berichte in das Dashboard, die der Produkt-Manager zum Tracking der Leistung verwenden kann. Diese Berichte enthalten einen [Fallout-Bericht](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/visualizations/fallout/fallout-flow), [aktuellen Monat](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/components/calendar-date-ranges/custom-date-ranges), [Trend-Konversionsraten](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/visualizations/line) und alles andere, was speziell für diesen Trichter gilt.
1. Fügen Sie die neuen Metriken und Dimensionen, die Sie entdeckt haben, zum SDR hinzu und senden Sie sie zur zweiten Überprüfung an die Stakeholder.

### Vorschau-Dashboards

1. Erstellen Sie mithilfe der Trichterzuordnung als Anleitung Mockup-Dashboards.
1. Es sollte eine Gesamtansicht geben, z. B. ein [Executive Summary Dashboard](driving-success-with-executive-summary-dashboards.md) und Dashboards für jeden Trichter.
1. Es gibt auch einige spezifischere Aspekte für Ihre Site oder App, z. B. Produktleistung oder Inhaltsleistung.
1. Verteilen Sie diese an die relevanten Interessengruppen und erhalten Sie Feedback zum Entwurf.
1. Nehmen Sie alle erforderlichen Aktualisierungen vor und fügen Sie sie Ihrem SDR hinzu, wenn neue Metriken oder Dimensionen erforderlich sind.
1. Senden Sie die aktualisierten Vorschau-Dashboards und SDR für eine endgültige Überprüfung.

### Instrumente zur Datendemokratisierung

1. Erstellen Sie ein Datenwörterbuch. Die SDR richtet sich an Ihre Entwickler, aber das Datenwörterbuch richtet sich an Ihre Endbenutzer. Machen Sie es lesbar, damit jeder einfach nachschlagen kann, welche Daten verfügbar sind und wie sie verwendet werden können. Ihre Endbenutzer sollten die endgültigen Genehmiger sein.
1. Anmerken. In jeder Organisation gibt es bestimmte Termine, die jedes Jahr wichtig sind, und andere, die sich ergeben werden. Stellen Sie sicher, dass Sie die relevanten Daten von Ihren Interessengruppen erfassen und sie als Anmerkungen hinzufügen, um das Verständnis der angezeigten Daten zu verbessern.
1. Kuratieren. Wenn Ihre SZR groß sind, könnte es überwältigend sein. Eine Lähmung der Wahl trifft nicht nur auf Ihre Kunden zu. Sehen Sie, was für die einzelnen Benutzergruppen wichtig ist, und kuratieren Sie die Elemente, die sie sehen werden.

## Der Grund

_Erfahren Sie mehr über die Erfassung von Anforderungen, den Aufbau einer Datenkultur, tief greifende Gedanken über Daten, die Schaffung eines Bewusstseins für die Daten und die Vereinfachung der Daten._

### Anforderungen sammeln

Das Sammeln von Anforderungen ist offensichtlich, aber es gibt mehrere effektive Möglichkeiten, dies zu tun. Ich habe Einzelgespräche, Fragebögen und Überprüfungen bestehender Berichte verwendet. Diese Strategien funktionieren, aber nicht so gut wie die Methoden, die ich gerade beschrieben habe. Ich glaube jedoch nicht, dass der Unterschied zwischen den Methoden für die Anforderungserfassung bedeutend ist. Die Methode, die ich beschrieben habe, bringt Sie zu 95% des Weges, und diese anderen Methoden bringen Ihnen 90% des Weges.

Was ist also der _Warum_?

### Erstellen einer Datenkultur

Bei diesem Vorgang gehen Sie folgendermaßen vor:

* Spark-Gedanken über die Erfolgsmessung
* Eigenverantwortung in Ihren Stakeholdern schaffen
* Den Stakeholdern das Verständnis ihrer Daten erleichtern

### Spark - tiefer Gedanke über Daten

Für viele Personen in Ihrem Unternehmen sind Daten etwas, das sie konsumieren. Sie benutzen es. Sie analysieren es. Sie denken nicht tief darüber nach. Manche Menschen haben Berichte und Prozesse von ihren Vorgängern geerbt, aber sie haben sie nicht um der Kontinuität willen verändert. Vielleicht mussten diese Personen nie über die _Warum_ der Daten nachdenken.

Dieser Prozess gibt ihnen die Möglichkeit, wirklich __ Daten zu verstehen. Fragen stellen wie: Was ist Erfolg? Woher würdest du wissen, ob du erfolgreich warst? Wie würdest du wissen, was du ändern würdest, wenn du nicht erfolgreich wärest? Diese Fragen müssen zu Beginn der Erstellung jeder Website, Anwendung und jedes Produkt beantwortet werden - aber viel zu oft nicht. Indem Sie diese Fragen stellen, helfen Sie, das Verständnis einer Person nicht nur über die Daten, sondern auch über ihr Produkt zu vertiefen.

### Eigenverantwortung für die Daten schaffen

Ein Gefühl des Eigentums ist nicht etwas, das ein Mensch leicht erwirbt. Es ist nicht in dem dreißigminütigen Treffen zu finden, das vor drei Monaten stattfand. Es wird nicht durch einen lästigen Fragebogen geschaffen, den sie zu schnell beantwortet haben, wegen anderer dringender Arbeitsfragen wie Demos und Sprint-Releasedatum.

Eigentum ist das Ergebnis des tiefen Denkens und der Zusammenarbeit mit Ihnen und Kollegen. Es ist das, worüber sie mehrmals nachgesehen haben, laufendes Feedback gegeben haben und was sie genehmigt haben, nachdem dieses Feedback aufgenommen wurde. Das sind ihre! Dass es nützlich ist, liegt an ihnen. Es sind _ihre_ Daten und dieser Prozess hat sie zu ihren gemacht.

### Daten vereinfachen

Sie haben ihnen auch gezeigt, wie sie den Prozess verwenden und wie er durch die [Vorschau-Dashboards](#the-preview-dashboards) aussehen wird. Jede neue Lösung ist _hard_. Es gibt so viel zu lernen, und angesichts der enormen Anpassungsfähigkeit von [!DNL Adobe Analytics] kann die Lernkurve steil sein. Sie haben jedoch 80 % davon entfernt. Noch bevor die erste Codezeile geschrieben wurde, wissen Ihre Stakeholder, wie ihre Dashboards aussehen werden. Sie werden wissen, wie sie sie lesen und von ihnen Sinn bekommen. Sie werden wissen, wie Erfolg buchstäblich aussieht, weil sie Ihnen gesagt haben, welche Metriken und Dimensionen Erfolg definieren. Und Sie haben ihnen erzählt, wie dieser Erfolg für sie visualisiert wird. Bei der Bereitstellung der eigentlichen Dashboards handelt es sich um einen Auffrischungskurs, keine beängstigende neue Lernaufgabe.

Dies ist nicht unbedingt der schnellste Weg, um SZR zusammenzubringen. Es ist viel Arbeit und erfordert eine große Koordinierung der Zeitpläne, besonders da es wichtig ist, dass Sie einige Führungskräfte in der Mischung haben. Am Ende ist eine Enterprise Analytics-Lösung jedoch eine enorme Investition in Zeit und Geld, und Sie möchten sicherstellen, dass die Akzeptanz und die Zufriedenheit hoch sind. Diese Methode geht weit in Richtung, dies zu erreichen.

**Autor**

Dieses Dokument wurde geschrieben von:

![gitai-headshot](assets/gitai-headshot-150.jpg)

Gitai Ben-Ammi, Associate Manager für Unternehmensarchitektur in Accenture

[!DNL Adobe Analytics] Champion
