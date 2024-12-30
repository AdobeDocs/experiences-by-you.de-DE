---
title: Planen einer neuen Marketo Engage-Implementierung
description: Erfahren Sie mehr über die erforderliche Planung und funktionsübergreifende Team-Zusammenarbeit für die erfolgreiche Implementierung einer neuen Marketo Engage-Instanz. Dieses Tutorial bietet Beispiele für Meilensteine, Teaminteraktionen und Ressourcenzuweisungen für eine nahtlose Marketo Engage-Implementierung.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last: substantial-update- 2024-05-01
jira: KT-14808
thumbnail: KT-14808.jpeg
exl-id: 65119abd-6f13-4acc-9e99-09843369ad28
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 5%

---

# Planen einer neuen Marketo Engage-Implementierung

Die Implementierung einer neuen Marketo Engage-Instanz erfordert eine sorgfältige Planung, die Zusammenarbeit zwischen den Teams und eine kontinuierliche Optimierung. Es gibt zwar kein perfektes Rezept für die Implementierung einer neuen Instanz, aber die meisten Marketo Engage-Administratoren, die es durchlaufen haben, können zustimmen, dass eine vorausschauende Planung den Prozess viel reibungsloser gestalten wird.

In diesem Tutorial gehen wir auf die spezifischen Meilensteine, Teaminteraktionen und Ressourcenzuweisungen ein, die für einen erfolgreichen Marketo Engage-Rollout entscheidend sind.

## Wichtige Meilensteine während der neuen Marketo Engage-Implementierung

### Phase 1: Erkennung und Planung

- Marketing- und Vertriebsbedarfsbewertung durchführen
- Definieren von Zielen für Key Performance Indicators (KPIs)

### Phase 2: Technische Einrichtung und Konfiguration

- Konfigurieren von Admin-Einstellungen einschließlich CNAMEs und Munchkin-Code.
- Lead-Management-Prozesse konfigurieren
- Testen von Automatisierungs-Workflows und Datensynchronisierung

### Phase 3: Erstellung der Programmbibliothek und Einrichtung der Kampagne

- Entwickeln von E-Mail-Vorlagen und Landingpages. Beginnen Sie mit [Importieren von ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program) aus der [Programm-Importbibliothek](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview).
- Einrichten von Segmentierungs- und Personalization-Regeln
- Erstellen erster Kampagnen für die Lead-Generierung und -Pflege

### Phase 4 - Schulung und Benutzerakzeptanz

- Durchführen von Schulungssitzungen und/oder Materialien für Benutzer
- Festlegen von Richtlinien und Best Practices für die Instanzverwaltung
- Überwachen von Metriken zur Benutzerakzeptanz und Feedback von Stakeholdern

### Phase 5: Live-Schaltung und Optimierung

- Abschließende Systemtests und Qualitätssicherung
- Starten erster Kampagnen und Überwachen der Leistung
- Implementieren iterativer Verbesserungen auf der Grundlage von Reporting- und Analysefunktionen

## Interaktion mit Stakeholdern und benötigte Ressourcen

Die Implementierung einer neuen Instanz erfordert eine sorgfältige Planung und Ausführung, um ihre Vorteile zu maximieren. Wenn Sie die richtigen Stakeholder zu Beginn einbeziehen, kann die Implementierung an die allgemeinen Anforderungen Ihres Unternehmens angepasst werden. Verweisen Sie auf die Beispiele der wichtigsten Stakeholder und ihrer potenziellen Rolle(n) im folgenden Projekt, um Sie bei der Suche nach den richtigen internen Partnern für die Implementierung von Marketo Engage zu unterstützen.

<table>
 <thead>
    <tr>
        <th>Stakeholder</th>
        <th>Mögliche Rollen und Zuständigkeiten  </th>
    </tr>
 </thead>    
 <tbody>
    <tr>
        <td>Marketing Operations Director/Manager</td>
        <td>
        <li>Hauptansprechpartner für das Projekt</li>
        <li>Governance-Regeln für Instanzen</li> 
        <li>Datenanalyse für Reporting und Analysen </li> 
        </td>
    </tr>
    <tr>
        <td>CRM-Administrator</td>
        <td>
        <li>CRM-Synchronisation </li>
        <li>Lead-Fluss</li> 
        </td>
    </tr>
     <tr>
        <td>IT-Administrator</td>
        <td>
        <li>Munchkin</li>
        <li>SPF/DKIM </li> 
        <li>Einrichten von Web-Domains</li> 
        <li>CNAMEs</li> 
        <li>Email Deliverability</li>
        </td>
    </tr>
    <tr>
        <td>Engineering</td>
        <td>
        <li>Entwicklung für die Integration benutzerdefinierter Services </li>
        <li>Data Engineering für die Datenzuordnung und -migration</li> 
        </td>
    </tr>
     <tr>
        <td>Marketing </td>
        <td>
        <li>Erstellung und Design von Programmvorlagen</li>
        <li>Kanäle </li>
        <li>Lead-/Personen-Scoring und -Lebenszyklus</li> 
        <li>Berichterstattung und Feedback zur Programmwirksamkeit</li> 
        </td>
    </tr>
     <tr>
        <td>Verkauf</td>
        <td>
        <li>Scoring-Modellierung für Leads/Personen</li>
        <li>Lead-Fluss/-Routing</li>  
        <li>Lebenszyklus-Service-Level-Agreements (SLAs)</li> 
        </td>
    </tr>
     <tr>
        <td>C-Suite</td>
        <td>
        <li>Gesamte Projektausrichtung  </li>
        <li>Allgemeine Implementierungsziele</li> 
        </td>
    </tr>
</table>

## Peer Perspective - Marketo Engage-Implementierung

Erfahren Sie von Marketo Engage Champion (2019), Kyle McCormick, über seine Onboarding- und Implementierungserfahrungen bei Palotos Networks. Sie erfahren mehr über die Herausforderungen, vor denen er stand, und über seine Ratschläge, wie Sie Ihren Onboarding-Prozess erfolgreich und effizient vorantreiben können.

>[!VIDEO](https://video.tv.adobe.com/v/3428771/?quality=12&learn=on)

## Wie geht es weiter?

Erstellen Sie einen neuen Implementierungsprojektplan und einen neuen Zeitplan. Nachfolgend finden Sie eine Beispiel-Projekt-Zeitleiste mit Abschnitten für Beispiel-Meilensteine, Aufgaben, verantwortliche Teams, Fristen und Abhängigkeiten. Verwenden Sie diese Option, um Ihre Marketo Engage-Implementierungs-Journey zu optimieren und einen erfolgreichen Rollout im gesamten Unternehmen sicherzustellen.

Sie können auch das Beispiel zum Bearbeiten und Tracking bestimmter Meilensteinaufgaben ([) ](/help/marketo-tutorial-implementing-new-instance/assets/adobe-marketo-engage-implementation-milestones-project-management-template.xlsx).

<table>
 <thead>
    <tr>
        <th>Thema</th>
        <th>Meilenstein</th>
        <th>Status</th>
        <th>Voraussichtliches Datum</th>
        <th>Tatsächliches Datum</th>
        <th>Benötigte Ressourcen</th>
    </tr>
 </thead>    
 <tbody>
    <tr>
        <td><em>Verwenden Sie diese allgemeinen Onboarding-Themen, um die Stadien Ihrer Meilensteine zu organisieren.</em></td>
        <td><em>Schreiben Sie Ihre spezifischen Meilensteinaufgaben auf.</em></td>
        <td><em>Wie ist der aktuelle Status Ihrer Aufgabe?</em></td>
        <td><em>Bis wann soll diese Aufgabe abgeschlossen sein?</em></td>
        <td><em>Wann wurde diese Aufgabe tatsächlich abgeschlossen?</em></td>
        <td><em>Welche Ressourcen benötigen Sie, um diese Aufgabe zu erfüllen, und von welchen Teams benötigen Sie sie?</em></td>
    </tr>
    <tr>
        <td rowspan="2">Technische Einrichtung</td>
        <td><em>Beispiel -</em> Installieren von MunchkinID auf der Unternehmens-Website</td>
        <td bgcolor="c6f0cf">Abgeschlossen</td>
        <td>9/5/24</td>
        <td>9/12/24</td>
        <td>Web-Entwicklungs-Team</td>
    </tr>
    <tr>
        <td><em>Beispiel - </em> Sie Domain Keys Identified Mail (DKIM) und zwei separate CNAMEs für Zustellbarkeits- und E-Mail-Tracking-Links ein.</td>
        <td bgcolor="c6f0cf">Abgeschlossen</td>
        <td>9/15/24</td>
        <td>9/18/24</td>
        <td>Support und Einrichtung durch das IT-Team</td>
    </tr>
    <tr>
        <td rowspan="4">Adobe Admin Console- und Admin-Setup</td>
        <td><em>Beispiel -</em> Erstellen von Marketo Engage-Benutzern und -Rollen</td>
        <td bgcolor="c6f0cf">Abgeschlossen</td>
        <td>8/27/24</td>
        <td>9/15/24</td>
        <td>Informationen von Marketing-Teams darüber, wer Zugriff auf Marketo Engage benötigt.</td>
    </tr>
    <tr>
        <td><em>BEISPIEL -</em> Erstellen eines zusätzlichen Marketo Engage-Produktadministrators in Adobe Admin Console</td>
        <td bgcolor="c6f0cf">Abgeschlossen</td>
        <td>8/27/24</td>
        <td>9/15/24</td>
        <td>Informationen des Marketing-Vorgangs-Teams dazu, wer Administratorzugriff auf Marketo Engage benötigt.</td>
    </tr>
    <tr>
        <td><em>Beispiel -</em> Einrichten von Support-Administratoren</td>
        <td bgcolor="c6f0cf">Abgeschlossen</td>
        <td>8/27/24</td>
        <td>9/15/24</td>
        <td>Informationen vom Marketing-Operations-Team zur Bestätigung der wichtigsten Kontakte für Support. Unterstützung von Systemadmin bei der Zuweisung von Support-Admin-Benutzern.</td>
    </tr>
    <tr>
        <td><em>Beispiel -</em> Definieren der Ordnerstruktur und von Benennungskonventionen</td>
        <td bgcolor="c6f0cf">Abgeschlossen</td>
        <td>9/7/24</td>
        <td>9/12/24</td>
        <td>Eingaben von jedem Team mithilfe von Marketo Engage zu Programmtypen und Organisationsanforderungen.</td>
    </tr>
    <tr>
        <td rowspan="2">CRM-Integration (falls zutreffend)</td>
        <td><em>Beispiel -</em> Ermitteln der Feldzuordnung vor der Synchronisierung</td>
        <td bgcolor="ffeb9c">Bearbeitung läuft</td>
        <td>10/22/24</td>
        <td>K. A.</td>
        <td>Unterstützung durch den CRM-Administrator zum Verständnis der verfügbaren Felder.</td>
    </tr>
    <tr>
        <td><em>BEISPIEL - </em> eines Daten-Audits</td>
        <td bgcolor="ffeb9c">Bearbeitung läuft</td>
        <td>10/26/24</td>
        <td>K. A.</td>
        <td>Unterstützung durch CRM-Admin oder -Budget.</td>
    </tr>
    <tr>
        <td rowspan="2">Erstellung des operationellen Programms</td>
        <td><em>BEISPIEL -</em> Erstellen eines Programms zur Standardisierung eingehender Daten</td>
        <td bgcolor="ffc7cf">Nicht gestartet</td>
        <td>11/9/24</td>
        <td>K. A.</td>
        <td>Unterstützung durch die Vertriebs-, Ops- und CRM-Teams bei der Ermittlung einer Datenverwaltungsstrategie.</td>
    </tr>
    <tr>
        <td><em>BEISPIEL -</em> Erstellen eines E-Mail-Abonnementzentrums</td>
        <td bgcolor="ffc7cf">Nicht gestartet</td>
        <td>11/19/24</td>
        <td>K. A.</td>
        <td>Beiträge der Marketing-Teams zu Inhaltstypen und zur Segmentierung für Mailing-Listen.</td>
    <tr>
        <td rowspan="2">Erstes Marketing-Programm erstellen</td>
        <td><em>BEISPIEL -</em> Einrichten eines einfachen E-Mail-Programms</td>
        <td bgcolor="ffeb9c">Bearbeitung läuft</td>
        <td>11/12/24</td>
        <td>K. A.</td>
        <td>Kreativ-Assets des digitalen Teams für E-Mails und Landingpages.</td>
    </tr>
    <tr>    
        <td><em>BEISPIEL -</em> Programm für vierteljährlichen Newsletter erstellen</td>
        <td bgcolor="ffc7cf">Nicht gestartet</td>
        <td>11/30/24</td>
        <td>K. A.</td>
        <td>Inhalte aus dem Marketing-Team für Newsletter-E-Mails und Kreativ-Assets/Inhalte aus dem Design-Team.</td>
    </tr>
    <tr>
        <td rowspan="2">LaunchPoint-Integrationseinrichtung</td>
        <td><em>BEISPIEL -</em> Nur API-Benutzer und -Rollen erstellen</td>
        <td bgcolor="ffc7cf">Nicht gestartet</td>
        <td>11/23/24</td>
        <td>   </td>
        <td>Ermitteln Sie mit den Marketing-Teams den Umfang der für die neue Instanz erforderlichen Services.</td>
    </tr>
    <tr>
        <td><em>BEISPIEL -</em> Erstellen eines benutzerdefinierten Services für Google Ads</td>
        <td bgcolor="ffc7cf">Nicht gestartet</td>
        <td>12/7/24</td>
        <td>   </td>
        <td>Unterstützung durch Web- und Paid-Media-Teams zur Authentifizierung von Marketo Engage für den Zugriff auf Google Ads.</td>
        <td>
    </tr>
    <tr>
        <td rowspan="2">Benutzerschulung und Dokumentation</td>
        <td><em>BEISPIEL -</em> Erstellen eines Governance-Handbuchs für interne Benutzer</td>
        <td bgcolor="ffc7cf">Nicht gestartet</td>
        <td>12/2/24</td>
        <td>K. A.</td>
        <td>Erstellen Sie ein Marketo Engage-Governance-Team, um unterstützende Governance-Dokumentationen oder Budgets zu erstellen, um das Governance-Projekt abzuschließen.</td>
    <tr>
        <td><em>BEISPIEL -</em> Schulung von 4 Benutzern und Bereitstellung des standardmäßigen Marketo-Benutzerzugriffs</td>
        <td bgcolor="ffc7cf">Nicht gestartet</td>
        <td>12/13/24</td>
        <td>K. A.</td>
        <td>Unterstützung durch VP Marketing, um Schulungen für den Zugriff auf Marketo Engage verpflichtend zu machen.</td>
    <tr>
        <td rowspan="2">Live-Schaltung</td>
        <td><em>BEISPIEL -</em> Ersten Newsletter senden</td>
        <td bgcolor="ffc7cf">Nicht gestartet</td>
        <td>12/9/24</td>
        <td>K. A.</td>
        <td>Marketing Operations-Team für Qualitätssicherung, Planung und Versand.</td>
    </tr>
    <tr>
        <td><em>Beispiel - </em> den ersten E-Mail-Leistungsbericht abrufen.</td>
        <td bgcolor="ffc7cf">Nicht gestartet</td>
        <td>12/16/24</td>
        <td>K. A.</td>
        <td>Marketing Operations-Team für Qualitätssicherung, Planung und Versand.</td>
    </tr>
 </tbody>    
</table>

>[!NOTE]
>Die angegebenen Beispiele basieren nicht auf einem echten Implementierungszeitplan. Nutzen Sie diese nicht als Standardzeitplan für Ihr Onboarding mit Marketo Engage, da jede Implementierung mit unterschiedlichen Meilensteinen und Anforderungen entsprechend den Anforderungen Ihres Unternehmens einzigartig ist.

Wenn Sie Unterstützung bei der Implementierung und Anpassung Ihrer Marketo Engage für Ihre Instanz benötigen, wenden Sie sich an das Adobe-Account-Team oder wenden Sie sich an [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

### Autor

{{amy-chiu}}
