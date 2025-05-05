---
title: Aufbau einer Datenkultur und eine Referenz für ein besseres Lösungsdesign
description: Revolutionieren Sie Ihre Datenstrategie und ermöglichen Sie Ihrem Team, ein solides Referenzdokument für das Lösungs-Design (Solution Design Reference, SDR) zu erstellen. Beseitigen Sie Messlücken und fördern Sie eine partizipative Datenkultur durch schrittweise Methoden.
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

# Aufbau einer Datenkultur und eine bessere Referenz für das Lösungsdesign

_Revolutionieren Sie Ihre Datenstrategie und ermöglichen Sie Ihrem Team die Erstellung eines soliden Referenzdokuments für das Lösungs-Design (Solution Design Reference, SDR). Beseitigung von Messlücken und Förderung einer kollaborativen Datenkultur durch schrittweise Methoden._

Es ist endlich Zeit. Man stellt eine solide SZR zusammen. Ein SDR ist das Handbuch, das Sie zur Implementierung Ihrer Metriken und Dimensionen verwenden. Man definiert, wie sie heißen, wenn sie feuern, und Ihre Entwickler lieben es. Sie haben den gesamten Bereitstellungsprozess durchlaufen, Akzeptanzkriterien geschrieben, Ihre Sprints durchlaufen, sie getestet und es ist geschafft! Ihre Instanz von [!DNL Adobe Analytics] sollte darin bestehen, dass Marketing- und Produkt-Teams feiern, während sie in die Daten eintauchen, neue Enthüllungen über Ihre Kunden erhalten und alle Erfolgsbereiche und, nun ja, Bereiche mit geringerem Erfolg finden. Aber Sie hören nicht die Auszeichnungen, die Sie erwartet haben.

Von einem Team hört man Klagen wie:

„Warum kann ich die Konversionsrate in diesem Trichter nicht ermitteln?“

„Warum gibt es dafür keine Metrik?“

„Ich brauche mehr Details! Eine Metrik allein reicht nicht aus. Es gibt mindestens drei verschiedene Dimensionen, in denen ich Leistung verstehen muss. Warum habt ihr sie nicht reingelegt?“

Aber die andere Mannschaft gibt noch mehr Anlass zur Sorge. Von ihnen hört man überhaupt nichts. Schlimmer noch: Sie sehen Diagramme, die eindeutig aus Ihrer alten Analyselösung übernommen wurden (die nicht mehr gepflegt wird und jeden Tag weiter in einen Sumpf aus Mangel und schmutzigen Daten fällt). Ein Gefühl der Angst erfüllt Sie, wenn Sie über die Entscheidungen nachdenken, die mit diesem ursprünglichen Schlamassel getroffen werden könnten.

_Was ist schiefgelaufen?_

_Warum gibt es Messlücken?_

_Warum unterstützen Ihre Team-Mitglieder das nicht?_

Ich werde dich ein wenig aus dem Schneider lassen. Es _(immer_ eine Überarbeitung geben. Wenn Ihre Site oder Anwendung komplex genug ist, um eine Unternehmensanalyselösung zu benötigen, wird Ihnen garantiert etwas entgehen. Aber in diesem Fall haben Sie nicht genug verpasst, um die Messlücken zu erklären, die ich beschreibe.

Was schief gelaufen ist, lässt sich viel schwieriger in eine Tabelle einfügen. Im Wesentlichen haben Sie Ihre erste Chance verpasst, eine kollaborative Datenkultur aufzubauen, während Sie Ihre SDR erstellt haben.

Ich möchte Ihnen eine Methode vorstellen, die meine Kollegen und ich entwickelt haben, um sowohl ein besseres SDR mit weniger Lücken zu erstellen als auch die Endbenutzer für die neue Instanz von [!DNL Adobe Analytics] zu begeistern. Sehen wir uns an, wie und warum Sie diese Methode in Betracht ziehen sollten.

## Die Show

_Erfahren Sie mehr über die Messkonferenz. Verwenden Sie eine Trichterkarte, um jeden Schritt Ihres Plans zu visualisieren. Erstellen Sie Pseudo-Dashboards, um sie als Gruppe zu überprüfen. Erstellen Sie ein Datenwörterbuch für Benutzer._

### Die Messkonferenz

1. Holen Sie Ihre Stakeholder entweder persönlich oder virtuell zusammen, um herauszufinden, was gemessen werden soll. An dieser Sitzung sollten einige Führungskräfte teilnehmen.
1. Wenn Sie bereits auf dem Board offensichtliche Beispiele für Haftnotizen haben, wie z. B. Umsatz, Umsatz oder Leads, werden die wichtigsten Produktindikatoren (KPIs) gemessen. Wiederholen Sie dies mit Dimensionen wie dem angemeldeten Status, Produktkategorien oder Suchbegriffen.
1. Bitten Sie alle Benutzer, eigene Notizen hinzuzufügen und diese nach Bedarf zu gruppieren.
1. Bitten Sie die Leute, über diejenigen abzustimmen, die sie für wichtig halten. Es handelt sich um unbegrenzte Stimmen, da alle diese Metriken und Dimensionen wahrscheinlich von Bedeutung sind.
1. Lassen Sie die Stakeholder für Metriken und Dimensionen mit niedrigen Stimmen, die darum gebeten haben, erklären, warum diese Komponenten verwendet werden. Wenn es einen guten Anwendungsfall gibt, behalten Sie diese Komponenten bei. Wenn es eine bessere Möglichkeit gibt, an diese Daten zu gelangen, oder niemand erklären kann, wie diese Daten umsetzbar sind, oder wenn es einen anderen guten Grund gibt, die Metriken und Dimensionen zu entfernen, tun Sie dies.
1. Fügen Sie diese Metriken und Dimensionen Ihrer SDR hinzu, um eine erste Überprüfung durch die anwesenden Stakeholder durchzuführen.

### Die Trichterkarte

1. Erhalten Sie eine Visualisierung aller Trichter, Schritt für Schritt mit jedem Status enthalten.
1. Führen Sie mit den Designern und Produkt-Managern jeden Schritt durch und besprechen Sie, was jeder als Erfolg in diesem Trichter betrachtet. Ist es die Konversionsrate? Wählt sie einen bestimmten Pfad? Verwendet es bestimmte Funktionen?
1. Stellen Sie Fragen dazu, welche Metriken und Dimensionen erforderlich sind, um die Trichterleistung bei jedem Schritt des Trichters und insgesamt zu verstehen.
1. Fügen Sie über jedem Schritt des Trichters die Metriken und Dimensionen hinzu, die bei diesem Schritt gemessen werden, einschließlich der berechneten Metriken.
1. Schreiben Sie zu Beginn jedes Trichters die Berichte in das Dashboard, die der Produkt-Manager verwenden kann, um die Leistung zu verfolgen. Diese Berichte enthalten einen [Fallout](https://experienceleague.adobe.com/de/docs/analytics/analyze/analysis-workspace/visualizations/fallout/fallout-flow), [aktuellen Monat](https://experienceleague.adobe.com/de/docs/analytics/analyze/analysis-workspace/components/calendar-date-ranges/custom-date-ranges), [Trend-Konversionsraten](https://experienceleague.adobe.com/de/docs/analytics/analyze/analysis-workspace/visualizations/line) und alles, was speziell für diesen Trichter gilt.
1. Fügen Sie die neuen Metriken und Dimensionen, die Sie erkannt haben, zur SDR hinzu und senden Sie sie zur zweiten Überprüfung an die Stakeholder.

### Die Vorschau-Dashboards

1. Erstellen Sie Mockup-Dashboards anhand der Trichterzuordnung als Anleitung.
1. Es sollte eine Gesamtansicht vorhanden sein, z. B[ ein ](driving-success-with-executive-summary-dashboards.md)Executive Summary Dashboard) und Dashboards für jeden Trichter.
1. Es gibt auch einige spezifischere Optionen für Ihre Site oder Ihr Programm, z. B. Produkt- oder Inhaltsleistung.
1. Verteilen Sie diese an die relevanten Stakeholder und erhalten Sie Feedback zum Design.
1. Nehmen Sie die angeforderten Aktualisierungen vor und fügen Sie neue Metriken oder Dimensionen zu Ihrer SDR hinzu, wenn Sie sie benötigen.
1. Senden Sie die aktualisierten Vorschau-Dashboards und SDR zur abschließenden Überprüfung.

### Tools zur Datendemokratisierung

1. Erstellen eines Datenwörterbuchs. Die SDR ist für Ihre Entwickler, aber das Datenwörterbuch ist für Ihre Endbenutzer. Machen Sie sie lesbar, damit jeder einfach nachsehen kann, welche Daten verfügbar sind und wissen kann, wie sie verwendet werden. Ihre Endbenutzer sollten die endgültigen genehmigenden Personen für diese Aufgabe sein.
1. Anmerken. In jeder Organisation gibt es bestimmte Daten, die jedes Jahr wichtig sind, und andere, die kommen. Stellen Sie sicher, dass Sie die relevanten Daten von Ihren Stakeholdern erfassen und als Anmerkungen hinzufügen, um das Verständnis der angezeigten Daten zu verbessern.
1. Kuratieren. Wenn die SZR groß sind, könnten sie eine Menge kosten. Die Lähmung der Wahl betrifft nicht nur Ihre Kunden. Sehen Sie, was für jede Benutzergruppe wichtig ist, und kuratieren Sie die Elemente, die sie sehen werden.

## Das Warum

_Erfahren Sie mehr über die Erfassung von Anforderungen, den Aufbau einer Datenkultur, das Auslösen fundierter Überlegungen zu Daten, die Schaffung eines Gefühls der Verantwortung für die Daten und die Vereinfachung der Daten._

### Sammeln von Anforderungen

Die Erfassung von Anforderungen ist naheliegend, doch gibt es mehrere effektive Möglichkeiten. Ich habe Einzelinterviews, Fragebögen und Überprüfungen vorhandener Berichte verwendet. Diese Strategien funktionieren, aber nicht so gut wie die eben beschriebenen Methoden. Ich glaube jedoch nicht, dass der Unterschied zwischen den Methoden für die Anforderungserfassung signifikant ist. Die Methode, die ich beschrieben habe, führt zu 95% des Weges dorthin. Und mit diesen anderen Methoden erreichen wir 90% des Weges.

Also, was ist das _warum_?

### Aufbau einer Datenkultur

In diesem Prozess:

* Spark tiefe Gedanken über die Messung des Erfolgs
* Schaffen Sie Verantwortungsbewusstsein bei Ihren Stakeholdern
* Erleichtern Sie den Stakeholdern das Verständnis ihrer Daten

### Auslösen eingehender Überlegungen zu Daten

Für viele Mitarbeiter Ihres Unternehmens sind Daten etwas, das sie konsumieren. Sie benutzen es. Sie analysieren es. Sie denken nicht tief darüber nach. Manche haben Berichte und Prozesse von ihren Vorgängern geerbt, aber nicht um der Kontinuität willen geändert. Vielleicht mussten diese Leute nie über das &quot;_&quot;_ Daten nachdenken.

Dieser Prozess gibt ihnen die Möglichkeit, Daten wirklich _zu_. Fragen zu stellen wie: Was ist Erfolg? Wie würdet ihr wissen, ob ihr erfolgreich wart? Wie wüsstest du, was du ändern sollst, wenn du nicht erfolgreich wärst? Diese Fragen müssen zu Beginn der Erstellung jeder Site, jedes Programms und jedes Produkts beantwortet werden - aber viel zu oft ist dies nicht der Fall. Indem Sie diese Fragen stellen, helfen Sie einer Person, nicht nur die Daten, sondern auch ihr Produkt besser zu verstehen.

### Schaffen Sie ein Gefühl der Verantwortung für die Daten

Ein Gefühl von Eigentum ist nicht etwas, das sich eine Person leicht aneignet. Es wurde in dem 30-minütigen Treffen, an dem die Teilnehmer vor drei Monaten teilnahmen, nicht gefunden. Es wird nicht dadurch erstellt, dass ein ärgerlicher Fragebogen, den sie wegen anderer dringender Arbeitsprobleme wie Demos und Sprint-Veröffentlichungstermine zu schnell beantwortet haben.

Eigenverantwortlichkeit ist das Produkt eines tiefen Denkens und der Arbeit, die jemand mit Ihnen und Kollegen geleistet hat. Es ist die Sache, die sie mehrmals betrachtet haben, für die sie kontinuierliches Feedback gegeben haben, und was sie nach dem Feedback genehmigt haben, wenn es eingearbeitet wurde. Es gehört ihnen! Die Tatsache, dass es nützlich ist, ist ihnen zu verdanken. Es sind _ihre_ Daten und es ist dieser Prozess, der sie zu ihren gemacht hat.

### Vereinfachen der Daten

Sie haben ihnen auch gezeigt, wie sie den Prozess verwenden werden und wie er durch die [Vorschau-Dashboards“ aussehen ](#the-preview-dashboards). Jede neue Lösung ist _schwer_. Es gibt so viel zu lernen. Und angesichts der enormen Anpassbarkeit von [!DNL Adobe Analytics] kann die Lernkurve steil sein. Sie haben aber 80 % davon entfernt. Noch bevor die erste Code-Zeile geschrieben wurde, wissen Ihre Stakeholder, wie ihre Dashboards aussehen werden. Sie werden wissen, wie sie sie lesen und was sie ihnen bedeuten. Sie wissen, wie Erfolg buchstäblich aussieht, weil sie Ihnen gesagt haben, welche Metriken und Dimensionen Erfolg definieren. Und ihr habt ihnen gesagt, wie dieser Erfolg für sie visualisiert wird. Die Bereitstellung der eigentlichen Dashboards ist eine Auffrischung und keine beängstigende neue Lernaufgabe.

Das ist nicht unbedingt der schnellste Weg, um ein SZR zusammenzubekommen. Das ist sehr arbeitsintensiv und erfordert viel Koordination der Zeitpläne, zumal es wichtig ist, dass einige Führungskräfte im Mix sind. Am Ende bedeutet eine Enterprise-Analyselösung jedoch eine enorme Investition von Zeit und Geld, und Sie möchten sicherstellen, dass Akzeptanz und Zufriedenheit hoch sind. Diese Methode trägt viel dazu bei, dass dies geschieht.

**author**

Dieses Dokument wurde verfasst von:

![gitai-headshot](assets/gitai-headshot-150.jpg)

Gitai Ben-Ammi, Associate Manager Business Architecture bei Accenture

[!DNL Adobe Analytics] Champion
