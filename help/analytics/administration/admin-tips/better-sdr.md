---
title: Erstellen einer Datenkultur und einer besseren Referenz zum Lösungsdesign
description: Revolutionieren Sie Ihre Datenstrategie und stärken Sie Ihr Team bei der Erstellung eines soliden SDR-Dokuments (Solution Design Reference). Beseitigung von Messlücken und Förderung einer partizipativen Datenkultur durch schrittweise Methoden.
feature: Implementation Basics
topic: Administration
role: User
level: Experienced
doc-type: Article
duration: 72000
last-substantial-update: 2024-04-25T00:00:00Z
jira: KT-15338
thumbnail: KT-15338.jpeg
source-git-commit: 484f93bc2828d2565486eff8ae4801a8d203d280
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 0%

---


# Erstellen einer Datenkultur und einer besseren Referenz zum Lösungsdesign

**Revolutionieren Sie Ihre Datenstrategie und stärken Sie Ihr Team bei der Erstellung eines soliden SDR-Dokuments (Solution Design Reference). Beseitigung von Messlücken und Förderung einer partizipativen Datenkultur durch schrittweise Methoden.**

Endlich ist es Zeit. Sie haben eine solide Lösungs-Design-Referenz (SDR) zusammengestellt. Dies ist der Leitfaden, den Sie verwenden, um Ihre Metriken und Dimensionen zu implementieren, wie sie genannt werden, wenn sie ausgelöst werden und Ihre Entwickler es lieben. Sie haben den gesamten Bereitstellungsprozess durchlaufen, Akzeptanzkriterien geschrieben, Ihre Sprints durchlaufen, die gesamte Sache QAing, und es ist fertig! Es war eine Menge Arbeit, und jetzt ist es fertig. Ihre Adobe Analytics-Instanz sollte die Marketing- und Produktentwicklung steigern, während sie die Daten untersuchen, neue Enthüllungen über Ihre Kunden erhalten und alle Erfolgsbereiche und Bereiche mit geringerem Erfolg finden. Aber Sie hören nicht die Akoladen, die Sie erwartet haben.

Von einem Lager hören Sie Beschwerden.

&quot;Warum kann ich die Konversionsrate für diesen Trichter nicht ermitteln?&quot;

&quot;Warum gibt es dafür keine Metrik?&quot;

&quot;Ich brauche viel mehr Details dazu. Eine Metrik allein reicht nicht aus. Es gibt mindestens drei verschiedene Dimensionen, die ich für ein besseres Verständnis der Leistung benötige. Warum hast du sie nicht hineingesteckt?&quot;

Aber es ist das andere Lager, das eine noch größere Besorgnis hervorruft. Von ihnen hört man überhaupt nichts. Aber noch viel schlimmer ist, dass Sie Diagramme sehen, die sehr klar aus Ihrer alten Analyselösung übernommen wurden, die nicht mehr gepflegt wird und jeden Tag weiter in einen Sumpf von Abfall und schmutzigen Daten fällt. Ein Gefühl der Angst erfüllt Sie, wenn Sie über die Entscheidungen nachdenken, die mit diesem Chaos getroffen werden könnten.

Was ist schiefgelaufen? Warum gibt es Messlücken? Warum nehmen Ihre Teammitglieder das nicht an?

Ich beginne, indem ich dich ein wenig aus dem Haken lasse. Dort ist *always* wird eine Revision sein. Wenn Ihre Site oder App komplex genug ist, um eine Enterprise Analytics-Lösung zu benötigen, ist im Grunde garantiert, dass Sie etwas verpassen. Aber nicht genug, um die Messlücken zu erklären, über die ich hier spreche. Was schiefgelaufen ist, ist viel schwieriger in eine Tabelle einzufügen. Sie haben Ihre ersten Chancen verpasst, eine partizipative Datenkultur aufzubauen, während Sie Ihre SDR erstellt haben. Ich möchte Sie durch eine Methode führen, die ich und meine Kollegen entwickelt haben, um sowohl eine bessere SDR mit weniger Lücken zu erstellen als auch um Endanwender zu investieren und sogar gelegentlich aufgeregt über ihre neue Instanz von Adobe Analytics. Lasst uns über die Hows und die Weißen gehen.

**Die**

***Messungskonferenz:***

1. Treffen Sie Ihre Interessengruppen, entweder persönlich oder virtuell, um herauszufinden, was gemessen werden soll. Dies sollte einige ausführbare Dateien enthalten.
1. Sie haben bereits einige offensichtliche Beispiele auf der Pinnwand, um Notizen zu erstellen, Dinge wie Umsatz, Vertrieb oder Leads, die wichtigsten KPIs, die Sie kennen, werden gemessen. Wiederholen Sie diese Schritte mit Dimensionen, Elementen wie dem angemeldeten Status, Produktkategorien oder Suchbegriffen.
1. Jeder soll seine eigenen Kurznotizen hinzufügen und nach Bedarf gruppieren.
1. Lassen Sie die Menschen über die Stimmen abstimmen, die sie für wichtig halten. Dies sind unbegrenzte Abstimmungen, da vielleicht all diese Metriken und Dimensionen wichtig sind.
1. Für alle, die geringe Stimmen haben, lassen Sie die Interessengruppen, die um sie gebeten haben, erklären, wofür sie sie verwenden werden. Wenn es einen guten Anwendungsfall gibt, behalten Sie ihn bei. Wenn es einen besseren Weg gibt, diese Daten zu erhalten, können sie nicht erklären, wie sie umsetzbar sind, oder es gibt einen anderen guten Grund, sie auszuschließen, schlagen Sie sie aus der Pinnwand.
1. Fügen Sie diese Metriken und Dimensionen zu Ihrem SDR hinzu, um sie erstmals von den beteiligten Benutzern zu überprüfen, die anwesend waren.

***Trichterkarte***

1. Erstellen Sie eine Visualisierung aller Trichter, Schritt für Schritt mit jedem Status
1. Führen Sie mit den Designern und Produktmanagern jeden Schritt durch und besprechen Sie, was sie als Erfolg auf diesem Trichter betrachten. Ist es Konversionsrate? Wählt sie einen bestimmten Pfad? Verwendet sie bestimmte Funktionen?
1. Stellen Sie Fragen dazu, welche Metriken und Dimensionen erforderlich sind, um die Trichterleistung bei jedem Schritt des Trichters und insgesamt zu verstehen.
1. Fügen Sie über jedem Schritt des Trichters die Metriken und Dimensionen hinzu, die bei diesem Schritt gemessen werden, einschließlich der berechneten Metriken.
1. Schreiben Sie zu Beginn jedes Trichters die Berichte, die in das Dashboard eingehen, das der Produkt-Manager zum Tracking der Leistung verwenden wird, Dinge wie einen Fallout-Bericht, aktuelle Monate und Trend-Konversionsraten sowie alles, was für diesen Trichter spezifischer ist.
1. Fügen Sie die neuen Metriken und Dimensionen, die Sie entdeckt haben, zum SDR hinzu und senden Sie sie zur zweiten Überprüfung an die Stakeholder.

***Vorschau-Dashboards***

1. Erstellen Sie mithilfe der Trichterzuordnung als Anleitung Mapping-Dashboards.
1. Es sollte eine Gesamtansicht geben, z. B. ein Dashboard für die Zusammenfassung und Dashboards für jeden Trichter.
1. Es gibt auch einige spezifischere Aspekte für Ihre Site oder App, z. B. Produktleistung oder Inhaltsleistung.
1. Verteilen Sie diese an die relevanten Interessengruppen und erhalten Sie Feedback zum Entwurf.
1. Nehmen Sie alle erforderlichen Aktualisierungen vor und fügen Sie sie Ihrem SDR hinzu, wenn neue Metriken oder Dimensionen erforderlich sind.
1. Senden Sie die aktualisierten Vorschau-Dashboards und SDR für eine endgültige Überprüfung.

***Werkzeuge zur Datendemokratisierung***

1. Erstellen Sie ein Datenwörterbuch. Die SZR sind für Ihre Entwickler. Das Datenwörterbuch richtet sich an Ihre Endbenutzer. Machen Sie es für Endbenutzer lesbar, damit sie einfach nachschlagen können, welche Daten verfügbar sind und wie sie verwendet werden können. Ihre Endbenutzer sollten die endgültigen Genehmiger sein.
1. Anmerkungen. In jeder Organisation gibt es bestimmte Termine, die jedes Jahr wichtig sind, und andere, die sich ergeben werden. Stellen Sie sicher, dass Sie die relevanten Daten von Ihren Interessengruppen erfassen und sie als Anmerkungen hinzufügen, um das Verständnis der angezeigten Daten zu verbessern.
1. Kuratierung. Wenn Ihre SZR groß sind, könnte es überwältigend sein. Eine Lähmung der Wahl trifft nicht nur auf Ihre Kunden zu. Sehen Sie, was für die einzelnen Benutzergruppen wichtig ist, und kuratieren Sie die Elemente, die sie sehen werden.

**Der Grund**

***Anforderungen abrufen***

Dies ist offensichtlich, aber es gibt andere effektive Möglichkeiten, Anforderungen zu bekommen. Ich habe eine persönlich für ein Interview, Fragebögen und Überprüfungen bestehender Berichte verwendet. Diese werden funktionieren, obwohl ich denke, nicht so gut wie die Methoden, die ich gerade beschrieben habe. Ehrlich gesagt glaube ich nicht, dass die Lücke in der Anforderungsanalyse so groß ist. Die Methode, die ich beschrieben habe, wird Ihnen 95% des Weges dorthin bringen, und diese anderen Methoden werden Ihnen 90% des Weges bringen. Was ist also der große Grund?

***So erstellen Sie eine Datenkultur***

Mit diesem Prozess können Sie:

- Spark-Gedanken über die Erfolgsmessung
- Eigenverantwortung in Ihren Stakeholdern schaffen
- Den Stakeholdern das Verständnis ihrer Daten erleichtern

***Sparen tief gehender Gedanken über Daten***

Für viele Personen in Ihrem Unternehmen sind Daten etwas, das sie konsumieren. Sie benutzen es. Sie analysieren es. Sie denken nicht tief darüber nach. Einige von ihnen erbten Berichte und Prozesse von ihren Vorgängern, die sie aufgrund der Notwendigkeit der Kontinuität nicht verändert haben. Sie mussten nie über den Grund der Daten nachdenken.

Dieser Prozess gibt ihnen die Möglichkeit, wirklich *verstehen* Daten. Wenn man die Fragen stellt, was ist Erfolg? Woher würdest du wissen, ob du erfolgreich warst? Wie würdest du wissen, was du ändern würdest, wenn du nicht erfolgreich wärest? Dies ist eine Übung, die am Anfang der Erstellung jeder Website, App und jedes Produkt durchgeführt werden sollte, aber viel zu oft nicht. Indem Sie diese Fragen stellen, helfen Sie, das Verständnis nicht nur der Daten, sondern auch des eigenen Produkts zu vertiefen.

***Eigenverantwortlichkeitsgefühl für die Daten schaffen***

Das ist nicht etwas, das von oben herabgesetzt wurde. Das war vor drei Monaten kein Treffen mit einer halben Stunde. Dies ist nicht so lästig, dass sie eine Woche lang gejagt wurden, um zu antworten, und dass sie dies in Eile getan haben, weil sie eine Demo hatten, damit sie das Sprint-Release-Datum erreichen konnten. Das ist das Ergebnis ihres tiefen Denkens und ihrer Arbeit mit Ihnen und ihren Kollegen, der Sache, die sie mehrmals betrachtet haben, die laufendes Feedback liefert und die sie nach der Aufnahme dieses Feedbacks angenommen haben. Das sind ihre! Dass es nützlich ist, liegt an ihnen. Es ist *,* und es ist der Prozess, der sie gemacht hat.

***Einfacheres Verständnis der Daten***

Sie haben ihnen auch gezeigt, wie sie es verwenden und wie es in den Vorschau-Dashboards aussehen wird. Jede neue Lösung *hard*. Es gibt so viel zu lernen und angesichts der enormen Anpassungsfähigkeit von Adobe Analytics kann die Lernkurve ziemlich steil sein. Sie haben jedoch 80 % davon entfernt. Noch bevor die erste Codezeile geschrieben wurde, wissen Ihre Stakeholder, wie ihre Dashboards aussehen werden. Sie werden wissen, wie sie sie lesen und von ihnen Sinn bekommen. Sie werden wissen, wie Erfolg buchstäblich aussieht, weil sie Ihnen gesagt haben, welche Metriken und Dimensionen Erfolg definieren, und Sie haben ihnen gesagt, wie dies für sie visualisiert wird. Bei der Bereitstellung der eigentlichen Dashboards handelt es sich um einen Auffrischungskurs, keine beängstigende neue Lernaufgabe.

Das ist nicht der schnellste Weg, eine SZR zusammenzubekommen. Es ist eine Menge Arbeit und erfordert eine große Koordinierung der Zeitpläne, besonders da es wichtig ist, dass Sie einige Dinge in der Mischung haben. Eine Unternehmensanalyselösung ist letztlich jedoch eine enorme Investition in Zeit und Geld, und Sie wollen sicherstellen, dass die Akzeptanz und die Zufriedenheit hoch sind. Diese Methode geht weit in Richtung, dies zu erreichen.

**Autor**

Dieses Dokument wurde verfasst von:

![gitai-headshot](assets/gitai-headshot.png)

Gitai Ben-Ammi, Associate Manager für Unternehmensarchitektur in Accenture

Adobe Analytics-Expertin


