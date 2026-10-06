---
title: Warten Sie jetzt einfach auf ein Segment… Verwenden Sie die Segmentierung, um neue Einblicke in Analysis Workspace zu erhalten
description: Erfahren Sie, wie Sie Segmente in [!DNL Adobe Analytics] verwenden, um neue Einblicke aus Ihren Analysis Workspace-Visualisierungen und Freiformtabellen zu erhalten.
feature-set: Analytics
feature: Segmentation
role: User
level: Beginner
doc-type: Article
last-substantial-update: 2023-05-16T00:00:00.000Z
jira: KT-13268
thumbnail: KT-13268.jpeg
exl-id: 3496b6ff-f8d6-48a1-92f4-442a792663e7
product_v2:
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
    internal-label: Experience Manager
  - id: c68cd75e-5bca-4bc3-a60e-9e183f816441
    internal-label: Experience Manager Cloud Manager
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
    internal-label: Segmentation
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 749b293ab38b8ea5a5f72517bd5c3455399137c2
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 2%
---
# Warten Sie jetzt einfach auf ein Segment… Verwenden Sie Segmente, um neue Einblicke in Analysis Workspace zu erhalten

Unabhängig davon, ob Sie ein neuer [!DNL Adobe Analytics] oder ein erfahrener Profi sind, nutzen Sie Segmente in Ihren Analysis Workspace-Projekten recht häufig. Wie [[!DNL Adobe] Experience League](https://experienceleague.adobe.com/docs/analytics/components/segmentation/seg-overview.html?lang=de) beschreibt, „ermöglichen Segmente es Ihnen, Untergruppen von Besuchern anhand von Merkmalen oder Website-Interaktionen zu identifizieren.“ Während das grundlegende Ergebnis dieser Funktion die Isolierung von Benutzergruppen, Besuchen oder Treffern auf Ihrer Site bedeutet, kann ein scharfsinniger Analyst wie Sie mit diesem Tool kreativ werden und neue Wege finden, um Einblicke in Ihre Site-Aktivität zu erhalten. Die Liste der möglichen Optionen ist umfangreich. Zögern Sie nicht, eine eigene zu erstellen und sie für andere in Ihrem Unternehmen oder online in Communities wie der [[!DNL Adobe Analytics] Community](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics/ct-p/adobe-analytics-community?profile.language=de) auf Experience League oder der [#Measure Slack](https://www.measure.chat/)-Community freizugeben.

Wenn Sie das Erstellen eines Segments schnell auffrischen müssen, lesen Sie die Experience League-Dokumentation zur Verwendung von [Segment Builder](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-build.html?lang=de) in Analysis Workspace.

## Vergleichen und Abgleichen von Segmenten

In Analysis Workspace können Sie zwei Segmente mithilfe von &quot;[Segmentvergleich“ &#x200B;](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/panels/segment-comparison/segment-comparison.html?lang=de). Einen Segmentvergleich finden Sie im Abschnitt Bedienfelder der linken Navigationsleiste:

![SEG 01](assets/seg01.png)

Manchmal benötigen Sie jedoch kein vollständiges Vergleichsfenster, um Ihren Endbenutzern wichtige Erkenntnisse zu vermitteln. Glücklicherweise können einige Funktionen auch in einem Standard-Panel verglichen werden.

Die [Venn-Diagrammvisualisierung](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/visualizations/venn.html?lang=de) kann Ihnen dabei helfen, einen schnellen Vergleich zu erstellen, sodass Sie den Mauszeiger über die sich überschneidenden Sitzungen, Bestellungen, Benutzer usw. bewegen und die sich überschneidenden Segmente sehen können, die zwischen zwei bis drei benutzerdefinierten Segmenten vorhanden sind. Sie können auch schnell Segmente erstellen, indem Sie mit der rechten Maustaste auf einen der überlappenden Abschnitte klicken:

![SEG 02](assets/s02.png)

Manchmal sind die wichtigen Informationen nicht in den sich überschneidenden Daten enthalten, sondern die Daten, die sich nicht überschneiden. Eine schnelle Möglichkeit, dies anzuzeigen, besteht darin, eine Kopie eines Segments zu erstellen und es zu einem „Ausschließen“-Segment zu machen:

![SEG 03](assets/s03.png)

Indem Sie Ihr „Ausschließen“-Segment mit dem anderen Segment in Ihrem Vergleich stapeln, können Sie jetzt schnell berechnen, wie viele Besuche Ihre Menüseite erreichen, ohne auch die Startseite in derselben Sitzung anzuzeigen:

![SEG 04](assets/s04.png)

## Stack-Angriff

Ebenso können Sie die sich überschneidenden Daten eines Venn-Diagramms erstellen, indem Sie einfach beliebige Segmente stapeln. Die Anzahl der Segmente oder einzelnen Dimensionen, die Sie stapeln, ist unbegrenzt. Wenn ich zum Beispiel schnell herausfinden wollte, an welchen Wochentagen meine Website im letzten Monat ein Mobiltelefon besucht hat, insbesondere ein Samsung Galaxy A52, das meine Speisekarten- und Ernährungsseiten gesehen hat, aber meine Startseite NICHT gesehen hat, kann ich sie schnell so erstellen:

![SEG 05](assets/s05.png)

Aber noch besser: Sobald ich die perfekte Untergruppe meines Benutzers oder meiner Besucherbasis gefunden habe, kann ich all diese Werte auswählen, mit der rechten Maustaste klicken und sofort ein Segment erstellen:

![SEG 06](assets/s06.png)

![SEG 07](assets/s07.png)

![SEG 08](assets/s08.png)

Das ist eine Menge Macht in einem Segment.

## Ein Zahlensegment für mehrere Segmente

Viele Benutzende betrachten beim Erstellen von Segmenten häufig Nominal-, Ordinal- oder Intervallwerte - Dinge wie eine besuchte Seite, einen Altersbereich von Benutzenden oder die Anzahl der Besuche, die eine Benutzerin oder ein Benutzer in der Vergangenheit gemacht hat. Sie können jedoch auch Verhältnisdaten beim Erstellen eines Segments verwenden, indem Sie diese Werte zu Buckets zusammenfassen - egal, ob es sich um Standarddimensionen, Standardmetriken oder benutzerdefinierte Variablen und Metriken für Ihre Organisation handelt.

Beispielsweise stehen für „Zeit auf Seite“ oder „Zeit pro Besuch“ vordefinierte Buckets zur Verfügung:

![SEG 09](assets/s09.png)

Diese entsprechen jedoch möglicherweise nicht immer den Anforderungen Ihres Unternehmens - vielleicht laufen die meisten Besuche auf der Website unter 10 Minuten. Sie können granulare Messungen verwenden, um Behälter unterschiedlicher Größe zu erstellen. Im Folgenden finden Sie eine erstellte Ansicht über Besuche, die zwischen 1 Minute, 1 Sekunde und 1 Minute bzw. 30 Sekunden dauern:

![SEG 10](assets/s10.png)

Nach der Erstellung kann ich jetzt meine Besuche, Bestellungen und andere Ereignisse nach den verschiedenen von mir angepassten Zeitgruppen anzeigen:

![SEG 11](assets/s11.png)

Sie können sogar mit der Untersuchung beginnen, wie sich Ihre Key Performance Indicators (KPIs) ändern, und zwar als Faktor dafür, wie viel Zeit ein Benutzer aufwendet, wie viele Seiten er bei einem Besuch aufruft, wie oft er in der Vergangenheit besucht hat oder einen anderen numerischen Wert. Dies ermöglicht es Ihnen, eine Metrik als Faktor einer anderen Metrik anzusehen:

![SEG 12](assets/s12.png)

Die Möglichkeiten, Segmente zu nutzen, um neue Einblicke zu finden, sind unbegrenzt! Dies ist lediglich ein Ausgangspunkt. Probieren Sie selbst ein paar aus und teilen Sie der Community mit, was Sie entdecken[[!DNL Adobe Analytics]  „Community](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics/ct-p/adobe-analytics-community?profile.language=de) auf Experience League oder die [#Measure Slack](https://www.measure.chat/)-Community.

Frohes Segmentieren!

## Autor

Dieses Dokument wurde verfasst von:

![Dan Cummings](assets/seg13.png)

**Dan Cummings**, Sr. Product Engineering [!DNL Analytics] Manager bei McDonald&#39;s Corporation

[!DNL Adobe Analytics] Champion
