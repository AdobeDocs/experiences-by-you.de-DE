---
title: Verwenden einer globalen Report Suite
description: Eine einzige globale Report Suite kann in vielerlei Hinsicht hilfreich sein und Ihre Implementierung erheblich vereinfachen.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10536.jpg
kt: 10536
exl-id: f133d049-9a24-4153-88c5-40ec480d1e4e
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%

---

# Verwenden einer globalen Report Suite

**WAS:** Es ist verlockend, Report Suites für jede Ihrer Sites zu erstellen, aber dies kann schnell zu Ihrem schlimmsten Albtraum werden - sowohl in Bezug auf die Kompliziertheit Ihrer Berichterstattung als auch auf Ihre Implementierung. Eine einzige globale Report Suite kann in vielerlei Hinsicht hilfreich sein und Ihre Implementierung erheblich vereinfachen.

**WARUM:** Erstellen einer globalen Report Suite ist die einzige Option, um eine einheitliche Ansicht Ihrer digitalen Eigenschaften und der Journey der Benutzenden für jede Eigenschaft zu erhalten. Wenn Sie über eine Mobile App und eine Website verfügen, sollten Sie die Mobile-App-Daten und Web-Daten immer in einer Report Suite kombinieren, um geräteübergreifende Journey zu nutzen und diejenigen zu verfolgen, die beide Eigenschaften als Einzelbesucher besuchen, im Vergleich zu separaten Report Suites, in denen Sie einen unzusammenhängenden Datensatz mit 2 Besuchern haben würden - 1 Besucher pro Eigenschaft -, ohne die Möglichkeit, die Überschneidung zu erkennen.

Im Folgenden finden Sie die Vor- und Nachteile einer einzelnen Report Suite, die Ihnen bei der Gewichtung Ihrer Optionen hilft:

* VORTEILE:
   * Ihre gesamte digitale Landschaft leicht verstehen können. Wenn Sie die Dimension „Eigenschaften“ (eVar) implementiert haben, auf die in anderen Tipps verwiesen wird, können Sie sehr einfach eine einzige Ansicht aller Ihrer Sites und Apps, Traffic und Konversionen erhalten. Dieser umfassende Überblick ist der Schlüssel zum Verständnis Ihres Geschäfts insgesamt.
   * Im gleichen Sinne können Sie jetzt sehen, wie Benutzer*innen sich durch all Ihre Eigenschaften bewegen, und ihre Journey in Ihrer digitalen Landschaft verstehen.
   * Einfachere Verwaltung. Bei Verwendung mehrerer Report Suites müssen Sie die Benutzeroberfläche an mehreren Stellen pflegen sowie mehrere Tagging-Dokumente (oder ein komplizierteres) verwalten. Alles an einem Ort zu halten bedeutet, dass es nur einen Ort gibt, an dem Updates vorgenommen werden können. Außerdem wird die Zugangsgewährung viel einfacher.
   * Bessere Benutzerfreundlichkeit in der Benutzeroberfläche. Wenn Ihre Benutzer nur einen Ort haben, müssen sie nicht darüber nachdenken, welche Report Suite sie auswählen sollen. Beachten Sie, dass Sie nicht mehrere Report Suites im selben Arbeitsbereich verwenden können. Wenn Sie mehrere davon haben, kann dies Ihre Benutzer*innen verwirren.
   * Weniger Server-Aufrufe = weniger Kosten. Wenn Sie mehrere Report Suites aufrufen, erhöhen sich Ihre Kosten. Wenn Sie Ihre Implementierung einfach halten, können Sie auch Ihre Kosten niedrig halten.
   * Sie können Virtual Report Suites (VRS) einfach nutzen, um Site-spezifische Daten innerhalb der globalen Report Suite auszuschlüsseln und Benutzerberechtigungen bei Bedarf auf der Grundlage einer VRS einzuschränken. Sobald Daten in einzelne Report Suites unterteilt sind, können Sie sie nicht mehr aggregieren. Wenn sie jedoch bereits in einem Datensatz (globale RS) zusammengefasst sind, können sie einfach aufgeschlüsselt werden.
* NACHTEILE:
   * Wenn Sie über sehr separate Eigenschaften verfügen, bei denen Benutzer nicht von einer zum anderen wechseln und dies nie erwartet wird, sollten Sie separate Report Suites beibehalten.
   * Wenn Ihre Eigenschaften sehr unterschiedliche Tagging- und Reporting-Anforderungen haben, kann es im Interesse der Variableneffizienz sinnvoll sein, separate Report Suites einzurichten. Separate Report Suites bieten Ihnen mehr Flexibilität bei der Verwendung benutzerdefinierter Variablen (mehr eVars).
   * Überschreiten eindeutiger Werte: In der [!DNL Adobe Analytics] können Sie innerhalb einer Dimension für einen bestimmten Zeitraum nur 500.000 eindeutige Werte anzeigen. Sobald Sie diesen Wert überschreiten, werden die Werte in der Benutzeroberfläche als „Eindeutige Werte überschritten“ oder „geringer Traffic“ gruppiert. Diese Werte stehen Ihnen zwar weiterhin im Backend (d. h. Data Warehouse, Daten-Feeds) zur Verfügung, können jedoch nicht über die Benutzeroberfläche visualisiert werden. Wenn Sie sehr detaillierte Daten haben (z. B. Benutzer-ID, PSN usw.), können Sie diese Ebene leicht erreichen. Separate Report Suites können bei diesem Problem hilfreich sein.

**WIE:** Mit einer neuen AA-Implementierung zu beginnen und eine globale Report Suite zu verwenden, ist einfach und unkompliziert. Sie müssen lediglich die globale Report Suite (eine für Entwicklung und eine für Produktion) in der Admin-Benutzeroberfläche von AA erstellen und dieselben Werte der Report Suite-ID (RSID) auf alle Eigenschaften anwenden.

Die Migration von einer Multi-Tagging-Strategie mit einer eindeutigen Report Suite pro Eigenschaft erfordert mehr Strategie und Planung. Beachten Sie dabei Folgendes:

* Ausrichten Ihrer Variablen (d. h. eVar1 auf Eigenschaft A muss denselben Datenpunkt erfassen wie eVar1 auf Eigenschaft B)
* Konsolidierung von Verarbeitungsregeln, Marketing-Kanalregeln, Klassifizierungen (SAINT und Rule Builder)
* Migrieren von Daten-Feeds und Datenquellen
* Auswahl eines Stichtags und Kommunikation dieses Datums mit allen Geschäftsbenutzern

## Autoren

Dieses Dokument wurde gemeinsam verfasst von:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Platform Manager bei NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, Senior Consultant bei [!DNL Adobe]
