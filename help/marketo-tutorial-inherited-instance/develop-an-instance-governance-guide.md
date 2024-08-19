---
title: Entwickeln eines Instance Governance-Handbuchs mit Dokumentation
description: Erfahren Sie, wie Sie ein zuverlässiges Verfahren für die Erstellung und Verwaltung von Dokumentation und Änderungsprogrammen für Ihre [!DNL Marketo Engage] Instanz einrichten.
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
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '874'
ht-degree: 1%

---

# Entwickeln eines Leitfadens zur Instanz-Governance mit Dokumentation

Wenn Sie in eine veraltete [!DNL Marketo Engage] -Instanz eintreten, ist es oft schwierig, die aktuelle funktionale und technische Dokumentation zu vermissen. Als Administrator ist die Festlegung von Richtlinien zur Gewährleistung einer ordnungsgemäßen Instanzverwaltung eine zentrale Verantwortung, die Sie nicht übersehen können. Dies ist eine der wichtigsten Strategien, um die Effizienz bei der Arbeit in einer etablierten [!DNL Marketo Engage] Instanz](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582) zu steigern.[

Dieses Schritt-für-Schritt-Tutorial von [!DNL [!DNL Adobe] Marketo Champion] (2018), Nick Hajdin, führt Sie durch diesen Prozess, um die Einrichtung Ihrer Instanz zu skizzieren, Ihre primären operationellen Programme zu dokumentieren und eine [!DNL changelog] zu verwalten, um eine strikte Governance-Richtlinie durchzusetzen.

## Entwickeln Sie ein Leitfaden zur Instanz-Governance für Ihre geerbte Instanz.

Eine detaillierte Dokumentation und ein [!UICONTROL Änderungsprotokoll] sind für eine effiziente Verwaltung und den Wissenstransfer in Ihrer [!DNL Marketo Engage] -Instanz unerlässlich. Wenn Sie die Änderungen und Entscheidungen verfolgen, die Sie während der Instanzeinrichtung getroffen haben, können Sie Folgendes tun:

1. Interne Benutzer einfacher skalierbar trainieren.
2. Effizientere Erstellung in [!DNL Marketo Engage] langfristig.
3. Behalten Sie die Gesundheit und Hygiene Ihrer Instanz von vorn bei, um zu verhindern, dass Sie Stunden mit dem Ausgraben von E-Mails, dem [Audit-Protokoll](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html) und dem [Aktivitätsprotokoll](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html) verbringen, um Kontext zu erhalten.
4. Sparen Sie Zeit beim Transfer von [!DNL Marketo Engage]-Wissen an einen neuen [!DNL Marketo Engage] -Administrator, wenn Ihr Team einen Umsatz erfährt.

## [!DNL Marketo Engage] Governance-Leitfaden 101

Ein Governance-Leitfaden dient als &quot;Source of Truth&quot; für die Anforderungen an die Instanzeinrichtung und das Systemdesign. Die wichtigsten Informationen, die in dieses Dokument aufgenommen werden sollten, sind:

* Programm-/Ordnerstrukturen
* Berechtigungen für Benutzer und Rollen
* Kommunikationsbeschränkungen
* Governance-Standards
* Interne Benutzerschulung vor der Gewährung des Zugriffs auf die Plattform

## Entwickeln und Verwalten eines Governance-Handbuchs für Ihre [!DNL Marketo Engage]-Instanz

### Schritt 1: Bestimmen Sie Ihren aktuellen Zustand des Governance-Handbuchs und der Dokumentation

* **Ich kann keine Dokumentation für meine geerbte Instanz finden:** Wenn Sie kürzlich eine neue Rolle gestartet haben und keine Dokumentation für Ihre geerbte Instanz finden können, gehen Sie zu Schritt 2 **und beginnen Sie mit einer herunterladbaren Vorlage, die wir bereitgestellt haben.**
* **Ich habe eine Dokumentation zur Datei:** Herzlichen Glückwunsch, dies ist ein gutes Zeichen! Überprüfen Sie die Relevanz dieser Änderungen, um festzustellen, wann die letzte Änderung vorgenommen wurde. Wenn Ihre Team-Mitglieder diese nicht aktiv verwalten, wird empfohlen, sie zu aktualisieren und Ihre internen Benutzer darüber zu informieren, wie Sie sie auf dem neuesten Stand halten können.

### Schritt 2: Identifizieren Sie die Elemente, die in Ihrer [!DNL Marketo Engage] Dokumentation &amp; [!DNL Changelogs] enthalten sein sollen

Das Format variiert von einer Cloud-basierten Plattform zu einem freigegebenen Dokument. Sie können das Format entwerfen, das den Anforderungen Ihres Unternehmens entspricht. [Hier finden Sie eine einfache Dokumentation und eine Excel-Vorlage für changelog](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx), die die wichtigen Elemente enthält, mit denen Sie beginnen können. Dazu gehören:

* Dokumentation
   * Name der Programmvorlage
   * Kanal
   * Erstellungsdatum
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

Zunächst werden die wichtigsten operationellen Programme mit Auswirkungen auf die Abonnementebene ermittelt. Beispiele sind Data Management [!DNL Campaign]s, Lead-Lebenszyklus, Lead-Scoring, [!DNL CRM] Synchronisierung und Zustellbarkeit.

Für jedes identifizierte operationelle Programm ist der aktuelle Stand zu dokumentieren. Dazu gehören Details zum Zweck des Programms, zur Einrichtung, zu verknüpften Smart-Kampagnen und zur Integration mit anderen Tools (falls zutreffend).

### Schritt 4: Erzwingen der Wartung von [!UICONTROL Changelog]

Der nächste Schritt besteht darin, eine strikte Governance-Richtlinie für Ihre [!DNL Marketo Engage]-Instanz festzulegen, die die Wartung von &quot;[!UICONTROL Changelog]&quot;erfordert. Diese Richtlinie stellt sicher, dass alle Aktualisierungen, die an operationellen Programmen in der gesamten Instanz vorgenommen werden, gründlich dokumentiert werden.

Informieren Sie Ihr Team über die Bedeutung dieser Dokumente und wie Sie sie ordnungsgemäß aufrufen und aktualisieren können. Es könnte hilfreich sein, Zuständigkeiten für die Pflege des Änderungsprogramms zuzuweisen, sodass einige benannte Marketing-Team-Mitglieder oder -Administratoren Änderungen laufend aufzeichnen und Abmeldemöglichkeiten bereitstellen.

### Schritt 5: Zentrale Dokumentation

Richten Sie einen zentralen Speicherort oder ein zentrales Repository ein, um alle mit Ihrer [!DNL Marketo Engage]-Instanz verbundenen Dokumentationen zu speichern. Dies kann ein freigegebenes Laufwerk, ein dedizierter Ordner oder ein Cloud-basiertes System sein.

### Schritt 6: Überprüfen und aktualisieren

Planen Sie regelmäßige Überprüfungen Ihrer Dokumentation, um sicherzustellen, dass sie korrekt und aktuell ist. Man kann es während der geschäftigen Zeiten leicht übersehen. Richten Sie proaktiv Erinnerungen an Ihren Kalender ein, um sicherzustellen, dass Ihr Team regelmäßig Aktualisierungen vornimmt, um Änderungen oder Optimierungen in Ihren operationellen Programmen widerzuspiegeln.

## Wie geht es weiter?

Beginnen Sie mit dem Herunterladen dieser [einfachen Vorlage](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx).

Gehen Sie wie oben beschrieben vor, um Ihr Governance-Handbuch und Ihre Dokumentation zu entwickeln. Beachten Sie beim Durcharbeiten des Prozesses die folgenden Faustregeln:

**Aktualisieren Sie Ihre vorhandene Dokumentation:**
Es ist wichtig, Ihre Dokumentation auf dem neuesten Stand zu halten. Wenn es in den letzten drei Jahren nicht geändert wurde, sollten Sie Ihre Dokumentation bei der Prüfung Ihrer Instanz überarbeiten.

**Freigeben und Trainieren:**
Geben Sie Ihre Dokumentation und [!DNL changelog] für relevante Team-Mitglieder frei und informieren Sie sie darüber, wie diese Datensätze aktualisiert werden.

**Periodische Überprüfung:** Sie können die Zeit vorplanen, diese im Laufe des Jahres zu überprüfen und zu verwalten, um neue Änderungen, Optimierungen oder Anpassungen einzubeziehen, sobald sie auftreten.

Die Pflege einer umfassenden und aktuellen Dokumentation für Ihre [!DNL Marketo Engage] -Instanz spart Ihnen langfristig Zeit und Mühe und erleichtert eine effektive Instanzverwaltung.

### Autoren

**Nick Hajdin**
[!DNL [!DNL Adobe] Marketo Champion] (2018)
*[!DNL Digital Technology Senior Manager at Accenture]*

![Nick Hajdin](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**Amy Chiu**
*Adoption &amp; Retention Marketing Manager,[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
