---
title: Entwickeln eines Instanz-Governance-Handbuchs mit Dokumentation
description: Erfahren Sie, wie Sie ein robustes Verfahren für das Erstellen und Verwalten der Dokumentation und des Änderungsprotokolls für Ihre Instanz  [!DNL Marketo Engage] .
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

# Entwickeln eines Instanz-Governance-Handbuchs mit Dokumentation

Wenn Sie eine ältere [!DNL Marketo Engage]-Instanz betreten, ist dies oft mit der Herausforderung verbunden, dass es an aktueller funktionaler und technischer Dokumentation fehlt. Als Administrator ist das Erstellen von Richtlinien zur Sicherstellung einer ordnungsgemäßen Instanz-Governance eine zentrale Aufgabe, die nicht übersehen werden darf. Dies ist eine der kritischen Strategien zur [ der Effizienz während der Arbeit in einer etablierten  [!DNL Marketo Engage] Instanz](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582).

Dieses Schritt-für-Schritt-Tutorial von [!DNL [!DNL Adobe] Marketo Champion] (2018), Nick Hajdin, führt Sie durch diesen Prozess, um die Einrichtung Ihrer Instanz zu umreißen, Ihre wichtigsten operativen Programme zu dokumentieren und eine [!DNL changelog] zur Durchsetzung einer strikten Governance-Richtlinie zu pflegen.

## Entwickeln eines Instanz-Governance-Handbuchs für die geerbte Instanz

Detaillierte Dokumentationen und ein [!UICONTROL Änderungsprotokoll] sind für eine effiziente Verwaltung und den Wissenstransfer innerhalb Ihrer [!DNL Marketo Engage]-Instanz von entscheidender Bedeutung. Die Nachverfolgung von Änderungen und Entscheidungen, die Sie während der Einrichtung Ihrer Instanz getroffen haben, kann Ihnen dabei helfen:

1. Schulung interner Benutzer einfacher und skalierbar.
2. Langfristig effizienter in [!DNL Marketo Engage] aufbauen.
3. Pflegen Sie den Zustand und die Hygiene Ihrer Instanz, um künftig Zeit zu sparen, damit Sie nicht stundenlang E-Mails, [Audit-Protokoll](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html?lang=de) und [Aktivitätsprotokoll](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html?lang=de) durchforsten müssen.
4. Sparen Sie Zeit bei der Übertragung [!DNL Marketo Engage] Wissens an einen neuen [!DNL Marketo Engage], wenn Ihr Team Fluktuation erlebt.

## [!DNL Marketo Engage]-Governance-Handbuch 101

Ein Governance-Handbuch dient als Quell der Wahrheit über die Einrichtung der Instanz und die Anforderungen an das System-Design. Es wird empfohlen, folgende wichtige Informationen in dieses Dokument aufzunehmen:

* Programm-/Ordnerstrukturen
* Berechtigung für Benutzer und Rolle
* Kommunikationsbeschränkungen
* Governance-Standards
* Interne Benutzerschulung, bevor ihnen Zugriff auf die Plattform gewährt wird

## Wie man ein Governance-Handbuch für die [!DNL Marketo Engage]-Instanz entwickelt und pflegt

### Schritt 1: Identifizieren Sie Ihr aktuelles Handbuch und Ihre Dokumentation zum Stand der Governance

* **Ich kann keine Dokumentation für meine geerbte Instanz finden:** Wenn Sie kürzlich eine neue Rolle gestartet haben und keine Dokumentation für Ihre geerbte Instanz finden können, **gehen Sie zu Schritt 2** und beginnen Sie mit einer herunterladbaren Vorlage, die wir bereitgestellt haben.
* **Ich habe Dokumentation zu Datei:** Glückwunsch, das ist ein gutes Zeichen! Überprüfen Sie ihre Relevanz, um zu sehen, wann die letzte Änderung vorgenommen wird. Wenn es von Ihren Team-Mitgliedern nicht aktiv gepflegt wird, wird empfohlen, es zu aktualisieren und Ihre internen Benutzer darüber zu informieren, wie es auf dem neuesten Stand gehalten werden kann.

### Schritt 2: Identifizieren Sie die Elemente, die in Ihre [!DNL Marketo Engage] Dokumentation und [!DNL Changelogs] aufgenommen werden sollen

Das Format variiert von einer Cloud-basierten Plattform zu einem freigegebenen Dokument. Sie können das Format entwerfen, das den Anforderungen Ihres Unternehmens entspricht. [Hier finden Sie eine einfache Dokumentation und eine Excel](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx)Änderungsprotokollvorlage, die die wichtigen Elemente abdeckt, mit denen Sie beginnen können. Dazu gehören:

* Dokumentation
   * Name der Programmvorlage
   * Kanal
   * Erstellt am
   * Erstellt von
   * Zweck des Programms
   * Status
   * Verknüpfung zu Programmvorlage
   * Hinweis
* Änderungsprotokoll
   * Name der Programmvorlage
   * Änderungsdatum
   * Aktualisiert von
   * Zweck der Aktualisierung
   * Erlebnis vor Änderung (einschließlich Links/Screenshots)
   * Erlebnis nach Änderung (einschließlich Links/Screenshots)
   * URL für Programm

### Schritt 3: Identifizieren und dokumentieren Sie den aktuellen Stand der primären operationellen Programme

Ermitteln Sie zunächst die wichtigsten operationellen Programme mit Auswirkungen auf der Abonnementebene. Beispiele sind Daten-[!DNL Campaign], Lead-Lebenszyklus, Lead-Bewertung, [!DNL CRM] und Zustellbarkeit.

Dokumentieren Sie für jedes ermittelte operationelle Programm seinen aktuellen Stand. Dazu gehören Details über den Zweck des Programms, die Einrichtung, zugehörige intelligente Kampagnen und die Integration mit anderen Tools (falls zutreffend).

### Schritt 4: [!UICONTROL &#x200B; der &#x200B;] erzwingen

Der nächste Schritt besteht darin, eine strikte Governance-Richtlinie für Ihre [!DNL Marketo Engage]-Instanz festzulegen, die die Wartung [!UICONTROL Änderungsprotokolls] erfordert. Diese Richtlinie stellt sicher, dass alle Aktualisierungen an operationellen Programmen in der gesamten Instanz sorgfältig dokumentiert werden.

Informieren Sie Ihr Team über die Wichtigkeit dieser Dokumente und darüber, wie Sie ordnungsgemäß auf sie zugreifen und sie aktualisieren können. Es könnte hilfreich sein, Verantwortlichkeiten für die Pflege des Änderungsprotokolls zuzuweisen, sodass einige designierte Mitglieder des Marketing-Vorgangs-Teams oder Administratoren Änderungen konsistent aufzeichnen und Genehmigungen erteilen.

### Schritt 5: Dokumentation zentralisieren

Erstellen Sie einen zentralen Speicherort oder ein Repository zum Speichern der gesamten Dokumentation im Zusammenhang mit Ihrer [!DNL Marketo Engage]. Dabei kann es sich um ein freigegebenes Laufwerk, einen dedizierten Ordner oder ein Cloud-basiertes System handeln.

### Schritt 6: Überprüfen und aktualisieren

Planen Sie regelmäßige Überprüfungen Ihrer Dokumentation, um sicherzustellen, dass sie korrekt und auf dem neuesten Stand bleibt. Man kann ihn leicht übersehen, wenn man viel beschäftigt ist. Richten Sie proaktiv Erinnerungen in Ihrem Kalender ein, um sicherzustellen, dass Ihr Team regelmäßig Aktualisierungen vornimmt, um Änderungen oder Optimierungen in Ihren betrieblichen Programmen widerzuspiegeln.

## Wie geht es weiter?

Laden Sie zunächst diese [einfache Vorlage](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx) herunter.

Führen Sie die oben genannten Schritte aus, um Ihr Governance-Handbuch und Ihre Dokumentation zu entwickeln. Beachten Sie bei der Arbeit im Prozess die folgenden Faustregeln:

**Aktualisieren der vorhandenen Dokumentation:**
Es ist wichtig, dass Sie Ihre Dokumentation auf dem neuesten Stand halten. Wenn es in den letzten 3 Jahren nicht geändert wurde, verpflichten Sie sich, die Dokumentation zu überarbeiten, während Sie Ihre Instanz überprüfen.

**Freigeben und Trainieren:**
Geben Sie Ihre Dokumentation und Ihre [!DNL changelog] für relevante Team-Mitglieder frei und schulen Sie diese in der Aktualisierung dieser Datensätze.

**Periodische Überprüfung:** Sie einen Zeitplan vor, um sie das ganze Jahr über zu überprüfen und zu pflegen, um alle neuen Änderungen, Optimierungen oder Anpassungen einzuschließen, sobald sie auftreten.

Die Pflege einer umfassenden und aktuellen Dokumentation für Ihre [!DNL Marketo Engage]-Instanz spart Ihnen langfristig Zeit und Mühe und erleichtert eine effektive Instanzverwaltung.

### Autoren

**Nick Hajdin**
[!DNL [!DNL Adobe] Marketo Champion] (2018)
*[!DNL Digital Technology Senior Manager at Accenture]*

![Nick Hajdin](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**Amy Chiu**
*Adoption &amp; Retention Marketing Manager,[!DNL Adobe]*

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
