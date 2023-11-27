---
title: Entwickeln eines Leitfadens zur Instanz-Governance mit Dokumentation
description: Erfahren Sie, wie Sie ein zuverlässiges Verfahren für die Erstellung und Verwaltung von Dokumentation und Änderungsliste für Ihre [!DNL Marketo Engage] -Instanz. Dies spart nicht nur Zeit für den Austausch von Wissen in Ihrem Team, sondern erhöht auch die Gesundheit und Effizienz Ihrer Instanz.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-14103
thumbnail: KT-14103.jpeg
hide: false
exl-id: e127b84d-ef92-4527-a0e6-a36af35b7ee0
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 1%

---

# Entwickeln eines Leitfadens zur Instanz-Governance mit Dokumentation

Wenn Sie in ein veraltetes [!DNL] eintreten [!DNL Marketo Engage]], ist es oft schwierig, die aktuelle funktionale und technische Dokumentation zu vermissen. Als Administrator ist die Festlegung von Richtlinien zur Gewährleistung einer ordnungsgemäßen Instanzverwaltung eine zentrale Verantwortung, die Sie nicht übersehen können. Es ist eine der wichtigsten Strategien, [Steigerung der Effizienz bei der Arbeit in einem etablierten [!DNL Marketo Engage] instance](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582).

Dieses Schritt-für-Schritt-Tutorial stammt von [!DNL [!DNL Adobe] Marketo Champion] (2018), Nick Hajdin, führt Sie durch diesen Prozess, um die Einrichtung Ihrer Instanz zu skizzieren, Ihre primären operationellen Programme zu dokumentieren und eine [!DNL changelog] eine strenge Governance-Politik durchzusetzen.

## Warum sollten Sie eine Anleitung zur Verwaltung von Instanzen und Dokumentation für Ihre geerbte Instanz entwickeln?

Detaillierte Dokumentation und eine [!DNL changelog] sind für effizientes Management und den Wissenstransfer in Ihrem [!DNL [!DNL Marketo Engage]] -Instanz. Wenn Sie die Änderungen und Entscheidungen verfolgen, die Sie während der Instanzeinrichtung getroffen haben, können Sie Folgendes tun:

1. Interne Benutzer einfacher skalierbar trainieren.
2. Effizientere Erstellung in [!DNL [!DNL Marketo Engage]] auf lange Sicht.
3. Sichern Sie sich die Gesundheit und Hygiene Ihrer Instanz, sodass Sie keine Stunden am Ausgraben von E-Mails verbringen können. [Audit-Protokoll](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html), und [Aktivitätsprotokoll](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html) um Kontext zu erhalten.
4. Sparen Sie Zeit beim Transfer von [!DNL [!DNL Marketo Engage]] Wissen zu einem neuen [!DNL [!DNL Marketo Engage]] -Administrator, wenn Ihr Team einen Umsatz erfährt.

## [!DNL [!DNL Marketo Engage]] Governance-Handbuch 101

Ein Governance-Leitfaden dient als &quot;Source of Truth&quot; für die Anforderungen an die Instanzeinrichtung und das Systemdesign. Die wichtigsten Informationen, die in dieses Dokument aufgenommen werden sollten, sind:

* Programm-/Ordnerstrukturen
* Berechtigungen für Benutzer und Rollen
* Kommunikationsbeschränkungen
* Governance-Standards
* Interne Benutzerschulung vor der Gewährung des Zugriffs auf die Plattform

## Entwicklung und Pflege eines Governance-Leitfadens für [!DNL] [!DNL Marketo Engage]] instance

### Schritt 1: Bestimmen Sie Ihren aktuellen Zustand des Governance-Handbuchs und der Dokumentation

* **Ich kann keine Dokumentation für meine geerbte Instanz finden:** Wenn Sie kürzlich eine neue Rolle gestartet haben und keine Dokumentation für Ihre geerbte Instanz finden können, **Schritt 2** und beginnen Sie mit einer herunterladbaren Vorlage, die wir bereitgestellt haben.
* **Ich habe eine Dokumentation zur Datei:** Herzlichen Glückwunsch! Das ist ein gutes Zeichen! Überprüfen Sie die Relevanz dieser Änderungen, um festzustellen, wann die letzte Änderung vorgenommen wurde. Wenn Ihre Team-Mitglieder diese nicht aktiv verwalten, wird empfohlen, sie zu aktualisieren und Ihre internen Benutzer darüber zu informieren, wie Sie sie auf dem neuesten Stand halten können.

### Schritt 2: Identifizieren Sie die Elemente, die in Ihre [!DNL] aufgenommen werden sollen. [!DNL Marketo Engage]] Dokumentation und [!DNL Changelogs]

Das Format variiert von einer Cloud-basierten Plattform zu einem freigegebenen Dokument. Sie können das Format entwerfen, das den Anforderungen Ihres Unternehmens entspricht. [Hier finden Sie eine einfache Vorlage für Dokumentation und changelog-Excel.](/help/marketo-tutorial-inherited-instance/_assets/downloads/[!DNL Adobe]_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx), die die wichtigen Elemente abdecken, mit denen Sie beginnen können. Dazu gehören:

* Dokumentation
   * Name der Programmvorlage
   * Kanal
   * Erstellt am
   * Erstellt von
   * Zweck des Programms
   * Status
   * Link zur Programmvorlage
   * Hinweis
* Änderungsprotokoll
   * Name der Programmvorlage
   * Änderungsdatum
   * Aktualisiert von
   * Zweck der Aktualisierung
   * Erlebnis vor Änderung (Links/Screenshots einschließen)
   * Erlebnis nach Änderung (einschließlich Links/Screenshots)
   * URL zum Programm

### Schritt 3: Ermittlung und Dokumentierung des aktuellen Status der primären operationellen Programme

Zunächst werden die wichtigsten operationellen Programme mit Auswirkungen auf die Abonnementebene ermittelt. Beispiele sind Data Management [!DNL Campaign]s, Lead-Lebenszyklus, Lead-Bewertung, [!DNL CRM] Synchronisierung und Zustellbarkeit

Für jedes identifizierte operationelle Programm ist der aktuelle Stand zu dokumentieren. Dazu gehören Details zum Zweck des Programms, zur Einrichtung, zu verknüpften Smart-Kampagnen und zur Integration mit anderen Tools (falls zutreffend).

### Schritt 4: Erzwingen [!DNL Changelog] Wartung

Der nächste Schritt besteht darin, eine strikte Governance-Politik für Ihre [!DNL] festzulegen [!DNL Marketo Engage]] -Instanz, die &quot;[!DNL Changelog] Wartung.&quot; Diese Richtlinie stellt sicher, dass alle Aktualisierungen, die an operationellen Programmen in der gesamten Instanz vorgenommen werden, gründlich dokumentiert werden.

Informieren Sie Ihr Team über die Bedeutung dieser Dokumente und wie Sie sie ordnungsgemäß aufrufen und aktualisieren können. Es könnte hilfreich sein, Zuständigkeiten für die Pflege des changelog zuzuweisen, sodass einige benannte Marketing-Team-Mitglieder oder -Administratoren Änderungen laufend aufzeichnen und Unterschriften bereitstellen.

### Schritt 5: Zentralisierung der Dokumentation

Erstellen Sie einen zentralen Speicherort oder ein zentrales Repository zum Speichern aller Dokumentationen im Zusammenhang mit Ihrer [!DNL [!DNL Marketo Engage]] -Instanz. Dies kann ein freigegebenes Laufwerk, ein dedizierter Ordner oder ein Cloud-basiertes System sein.

### Schritt 6: Regelmäßige Überprüfung und Aktualisierung

Planen Sie regelmäßige Überprüfungen Ihrer Dokumentation, um sicherzustellen, dass sie korrekt und aktuell ist. Man kann es während der geschäftigen Zeiten leicht übersehen. Richten Sie proaktiv Erinnerungen an Ihren Kalender ein, um sicherzustellen, dass Ihr Team regelmäßig Aktualisierungen vornimmt, um Änderungen oder Optimierungen in Ihren operationellen Programmen widerzuspiegeln.

## Wie geht es weiter?

Erste Schritte - Herunterladen [einfache Vorlage](/help/marketo-tutorial-inherited-instance/_assets/downloads/[!DNL Adobe]_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx).

Gehen Sie wie oben beschrieben vor, um Ihr Governance-Handbuch und Ihre Dokumentation zu entwickeln. Beachten Sie beim Durcharbeiten des Prozesses die folgenden Faustregeln:

**Aktualisieren Sie Ihre vorhandene Dokumentation:**
Es ist wichtig, Ihre Dokumentation auf dem neuesten Stand zu halten. Wenn es in den letzten drei Jahren nicht geändert wurde, sollten Sie Ihre Dokumentation bei der Prüfung Ihrer Instanz überarbeiten.

**Freigabe und Schulung:**
Freigeben der Dokumentation und [!DNL changelog] mit relevanten Teammitgliedern und ihnen erklären, wie diese Datensätze aktualisiert werden können.

**Regelmäßige Überprüfung:** Sie können Zeit vorab planen, um sie im Laufe des Jahres zu überprüfen und zu verwalten und neue Änderungen, Optimierungen oder Anpassungen bei deren Eintreten einzubeziehen.

Pflegen einer umfassenden und aktuellen Dokumentation für Ihre [!DNL Marketo Engage] -Instanz spart Ihnen langfristig Zeit und Mühe und erleichtert eine effektive Instanzverwaltung.

### Autoren

**Nick Hajdin**
[!DNL [!DNL Adobe] Marketo Champion] (2018)
*[!DNL Digital Technology Senior Manager at Accenture]*

![Nick Hajdin](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**Amy Chiu**
*Adoption &amp; Retention Marketing Manager,[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
