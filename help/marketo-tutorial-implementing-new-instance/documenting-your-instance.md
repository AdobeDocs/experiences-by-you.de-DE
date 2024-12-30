---
title: Erste Schritte mit Instanz-Governance und Dokumentation
description: Lernen Sie die wichtigsten Strategien und Best Practices für die ersten Schritte mit der Marketo Engage-Governance und -Dokumentation kennen. Erfahren Sie, wie Sie eine skalierbare Dokumentation erstellen, die Benutzerschulung optimieren und sicherstellen können, dass Sie in Ihrer Marketo Engage-Instanz eine Struktur erstellen.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-08T00:00:00Z
jira: KT-14815
thumbnail: KT-14815.jpeg
exl-id: b3dd05e1-c522-4631-a6b4-c0c6309f25d3
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Erste Schritte mit Instanz-Governance und Dokumentation

Eine gute Dokumentation kann fast so wichtig sein wie die eigentliche Instanzimplementierung selbst. Ein Governance-Handbuch ist eine wichtige Ressource, die Details zur Einrichtung Ihrer Marketo Engage-Instanz skizziert und Themen wie Programm-/Ordnerstrukturen, Kommunikationsbeschränkungen und mehr behandelt. Dieses Live-Dokument ist eine Referenz für Ihre Marketo Engage-Admin oder Power-User und zeigt spezifische Best Practices und Steuerungsstandards auf, die auf Ihre Marketo Engage-Instanz und Ihr Unternehmen zugeschnitten sind.

Aber damit nicht genug. Ihr Team benötigt möglicherweise zusätzliche Aktivierungsdokumente oder Schulungsmaterialien, um seine Kenntnisse im Marketo Engage zu verbessern. Zu diesen Ressourcen können interaktive Übungen, Quiz-Tests für den Zugriff oder Richtlinien für zulässige Aktionen innerhalb von Marketo Engage gehören, die allen Marketo Engage-Anwendern in Ihrem Unternehmen zugute kommen. Ob es um die Erstellung eines umfassenden Governance-Handbuchs oder die anfängliche Dokumentation wichtiger Einrichtungsaspekte geht: Die Aufzeichnung von Entscheidungen, die beim Onboarding getroffen wurden, ist der Schlüssel zum Erfolg beim Marketo Engage für Ihr aktuelles Team und zukünftige Generationen neuer Mitarbeiter.

Um die Bedeutung der Dokumentation und Governance zu verstehen, werden in diesem Tutorial die Best Practices behandelt, die von [ stammen (Erste Schritte mit Ihrer Marketo Engage-Governance- und Schulungsdokumentation](https://nation.marketo.com/t5/product-blogs/getting-started-on-your-marketo-governance-and-training/ba-p/242421){target="_blank} und [Wie dokumentieren Sie Ihre Instanz?](https://nation.marketo.com/t5/product-discussions/how-do-you-document-your-instance/td-p/72877){target="_blank}, um Sie bei der Einrichtung eines Prozesses zu unterstützen und die Dokumentation zu führen, die für Ihre internen Benutzer relevant ist.

## Warum die Dokumentation von Änderungen und Entscheidungen während der Implementierung der Instanz wichtig ist

Wenden Sie sich an Ihre Marketo Engage-Dokumentation, als würden Sie einen neuen Mitarbeiter, der mit der Technologie nicht vertraut ist, zum Onboarding in die Instanz leiten. Es ist leicht, Grundlagenkenntnisse zu übersehen, sobald Sie Erfahrung mit Marketo Engage gesammelt haben. Als Administrator sollten Sie sicherstellen, dass Ihre Aktivierungs- und Governance-Dokumente für Anfänger geeignet sind. Um das Lernen neuer Benutzer zu erleichtern, ist es eine praktische Methode, Definitionen und Best Practices direkt in Ihre Schulungsmaterialien zu integrieren.

Das Erstellen der Instanzdokumentation während der Instanzeinrichtung bietet mehrere Vorteile:

* Optimieren Sie den Schulungsprozess für neue Benutzer auf skalierbare Weise.
* Fördern Sie die langfristige Programmentwicklung in Marketo Engage, indem Sie auf einer soliden Dokumentationsgrundlage aufbauen.
* Pflegen Sie den Zustand und die Organisation Ihrer Instanz im Laufe der Zeit.
* Reibungsloser Übergang für neue Marketo Engage-Administratoren bei Teamwechsel.

Letztendlich hilft Ihnen das Aufschreiben der Entscheidungen, die Sie während der Implementierung treffen, und Ihrem Team, mit Marketo Engage erfolgreich zu sein, ohne auf ein oder eine Handvoll von Personen angewiesen zu sein, um die Prozesse durchzusetzen.

## So erstellen Sie die Governance Ihrer Marketo Engage-Instanz und Dokumentation

### Schritt 1: Skizzieren Sie wichtige Themen in Ihrer Instanzdokumentation.

Definieren Sie eine Reihe von Standards dafür, was dokumentiert werden soll und was nicht dokumentiert werden muss. Dadurch kann die Organisation den Prozess übernehmen. Beim Erweitern des Dokuments ist es wichtig, die Gründe für die Einrichtung zu dokumentieren. Dies hilft anderen Admins ebenso wie Ihnen, keine Zeit mit Entscheidungen zu verschwenden, die keine Ergebnisse gebracht haben.

Beginnen Sie Ihren Governance- und Dokumentationsplan, indem Sie mit dem folgenden Beispiel beginnen:

1. Der Zweck des Marketo Engage für unser Unternehmen
1. Zweck dieser Dokumentation
1. Der Prozess zur Pflege/Vornahme von Änderungen am Governance-Handbuch
1. Administrative Einrichtung
   * Abonnement(s)
   * Arbeitsbereiche und Partitionen (falls zutreffend)
   * Technische Einrichtung (DKIM/SPF/Munchkin)
   * Rollen und Zuständigkeiten*
   * Benutzer*
   * Smart Campaign/Email/Program Settings
   * Kommunikationsbeschränkungen
   * Sicherheit
   * Kanäle*
   * Tags
1. Datenstruktur
   * Feldstruktur
   * Benutzerdefinierte Objekte
1. Operationelle Programme
   * Personenbewertung
   * Lebenszyklus von Personen
   * Daten-Management
1. Erstellen in der Marketo Engage-Instanz
   * [Kompetenzzentrum (COE)](https://business.adobe.com/blog/perspectives/center-of-excellence-top-10-questions-to-ask-yourself){target="_blank}
   * Ordnerstruktur
   * Benennungskonventionen
   * Programmorganisation
   * Programmvorlagen*
   * Design Studio Assets (E-Mail-Vorlagen, Landingpage-Vorlagen, Snippets, Formulare)
   * Standardisierte Prozesse
   * Checklisten
   * Segmentierung
   * Archivierungsrichtlinien
   * Abonnementzentrum
1. CRM-Integration
   * Funktionsweise der Synchronisierung
   * Kampagnensynchronisierung
   * Datenwörterbuch
1. Andere Integrationen
1. DSGVO und Compliance

\* Ihre Dokumentation sollte mindestens Details zu Benutzern und Rollen, Programmvorlagen und Kanälen enthalten, sobald die Einrichtung abgeschlossen ist.

### Schritt 2: Erstellen eines Änderungsprotokolls

Eine weitere wichtige Methode zur Verwaltung von Instanzen besteht darin, ein Änderungsprotokoll zu erstellen und dessen Verwendung zu erzwingen. Jedes Mal, wenn Sie eine Einstellung im Bereich „Admin“ oder in einem operationellen Programm ändern, sollte Ihr Team sie an einem zentralen Ort notieren, z. B. in einer gemeinsamen Tabelle. Dies kann Ihnen dabei helfen, sich daran zu erinnern, warum Sie eine Änderung vorgenommen haben und wie sie zuvor aussah. Zu den Feldern, die Sie im Änderungsprotokoll dokumentieren sollten, gehören:

1. Datum
1. Programmname
1. Programmlink
1. Smart Campaign-Name
1. Smart Campaign-Link
1. Änderung vorgenommen
1. Grund für die Änderung
1. Wer hat die Änderung vorgenommen?

## Wie geht es weiter?

* Laden Sie die [Beispieldokumentation und das Änderungsprotokoll](/help/marketo-tutorial-implementing-new-instance/assets/template-adobe-marketo-engage-instance-documentation.xlsx) herunter und passen Sie sie an die Anforderungen Ihres Unternehmens an.
* Speichern Sie die Dokumentation auf einer barrierefreien Plattform, auf der Ihr Unternehmen gerne verweist und regelmäßig aktualisiert. Einige Marketo Engage-Champions verwenden beispielsweise Confluence (von Atlassian) oder Excel Spreadsheet.
* Stellen Sie sicher, dass jede Regel, die Sie für Governance erstellen, einen Eigentümer hat, der sie durchsetzt, und passen Sie die Dokumentation an, sodass sie im Laufe der Zeit auf dem neuesten Stand bleibt.

### Autor

{{amy-chiu}}
