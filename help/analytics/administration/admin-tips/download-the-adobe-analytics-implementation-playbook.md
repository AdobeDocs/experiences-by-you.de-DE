---
title: Playbook  [!DNL Adobe Analytics]  Implementierung herunterladen
description: Ein Business Requirements Doc (allgemein als BRD bezeichnet) ist eine sehr wichtige Dokumentation, an der wesentliche Stakeholder, Geschäftsbenutzer und technische Anwender zusammenarbeiten sollten. Hier können Sie alle gewünschten KPIs, Reporting-Anforderungen und jeden Datenpunkt dokumentieren, den Sie nach Abschluss Ihrer AA-Implementierung sehen möchten.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10530.jpg
kt: 10530
exl-id: 42679c86-e08f-4dda-8e47-f9880409bad6
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '1779'
ht-degree: 0%

---

# Herunterladen des Playbooks für die [!DNL Adobe Analytics]-Implementierung

Bevor Sie beginnen, [&#x200B; Sie das Playbook &#x200B;](assets/aa-implementation-playbook.xlsx).

## Registerkarte „Geschäftsanforderungen“

**WAS:** Ein Business Requirements Doc (allgemein als BRD bezeichnet) ist eine sehr wichtige Dokumentation, an der wesentliche Stakeholder, Geschäftsbenutzer und technische Anwender zusammenarbeiten sollten. Hier können Sie alle gewünschten KPIs, Reporting-Anforderungen und jeden Datenpunkt dokumentieren, den Sie nach Abschluss der Implementierung Ihrer [!DNL Adobe Analytics] (AA) sehen möchten.

**WARUM:** Dies dient als Ausgangspunkt für die nachfolgende Dokumentation (SDR, technische Spezifikationen usw.) und ist eine gemeinsame Datenquelle für einen vereinbarten Endzustand von AA. Dieses Dokument fasst die Gedanken der verschiedenen Teams innerhalb der Organisation zusammen, um eine einheitliche Richtung für den Aufbau oder die Verbesserung Ihrer Implementierung festzulegen.

**WIE:** Die Dokumentation der Geschäftsanforderungen wird in der Regel von den geschäftlichen Endbenutzern von AA durchgeführt. Es ist jedoch wichtig, Feedback von technischen Anwendern zu erhalten, da technische Herausforderungen zu beachten sind und bestimmte Datenpunkte möglicherweise mehr Aufwand erfordern als andere, was wiederum zu einer Priorisierung führen sollte.

Fragen Sie sich: „Welche Dinge möchten wir auf unserer Website nachverfolgen?“, „Welche Datenpunkte sind für mich beim Reporting wichtig?“ und vor allem: „Wie werden diese Datenpunkte in Entscheidungen einfließen?“ Es ist wichtig sicherzustellen, dass sich jede Ihrer Geschäftsanforderungen auf einen Datenpunkt bezieht, der als Grundlage für geschäftliche Entscheidungen verwendet werden kann. Es kann zum Beispiel verlockend sein, jeden Klick auf Ihrer Site zu verfolgen, aber welche Erkenntnisse gewinnen Sie letztendlich aus diesen Berichten?

Füllen Sie zunächst Spalte C im folgenden Screenshot aus (Geschäftsanforderung). Dabei sollte es sich um Fragen handeln wie „Wie viele interne Suchvorgänge werden auf unserer Website durchgeführt?“ oder „Welcher interne Kampagnenspot ist in Bezug auf die Impressionen am effektivsten?“. Nachdem Sie diesen Detaillierungsgrad angegeben haben, können Sie die Spalte B (Kategorie) ausfüllen und die Anforderungen in Kategorien wie „Suche“ oder „Interne Promotion“ gruppieren, die gut zu Ihren technischen Spezifikationen passen sollten.

Sie geben auch an, ob Sie glauben, dass die Verwendung einer eVar, eines Ereignisses, einer Prop oder einer Kombination das gewünschte Nachverfolgungsziel erreicht.

Und schließlich dient die Spalte „Implementierungsstatus“ als Statusprüfung, wenn Sie beginnen, Dinge zu Ihrer Site hinzuzufügen.

![Dokument zu Geschäftsanforderungen](assets/brd-template.png)

## Registerkarte „Variablenzuordnung“ (Tagging von Dokumenten/SDR)

**WAS:** Ein Tagging-Dokument (häufig als SDR bezeichnet) ist eine wichtige Dokumentation, die sowohl für technische als auch für Geschäftsbenutzer von AA nützlich ist. Sie listet jede Variable auf, die von Report Suites verwendet wird, zusammen mit allen relevanten Details für die Variableneinstellungen, wie die Variable implementiert ist und welchen Zweck sie im Reporting erfüllt. Wie Ihr Eigenschaftendokument sollte auch dieses Dokument ein lebendiges, gut verwaltetes Excel-Dokument sein, das von einer verantwortlichen Person auf dem neuesten Stand gehalten wird, wenn Verbesserungen beim Tagging oder Änderungen bei der Implementierung eingeführt werden.

**WARUM:** Dieses Dokument dient vielen Zwecken, die wichtigsten sind jedoch die folgenden:

* Für alle, die mit Ihrer Implementierung noch nicht vertraut sind (neue Mitarbeiter, Geschäftsinhaber, die die verfügbaren Berichte besser verstehen möchten usw.), bietet dieses Dokument den besten Überblick über alle implementierten Variablen und deren Zweck, damit sich Einzelpersonen selbst mit der Einrichtung Ihrer AA vertraut machen können.
* Für den AA-Produkteigentümer/technischen Benutzer dient dieses Dokument als Erinnerung daran, wie andere Variablen eingerichtet werden und welche Variablen beim Hinzufügen einer neuen Dimension verwendet werden können.

**WIE:** Beginnen Sie damit, alle [!DNL Adobe] vordefinierten Variablen (Seite, Produkt, Geografie usw.) sowie eVars, Props, Ereignisse und Listenvariablen in einem Excel-Dokument aufzulisten. Dieses sollte pro Site/Report Suite über eine Registerkarte verfügen.
Für jede dieser Dimensionen werden die folgenden Spalten hinzugefügt:
* **Name:** Geben Sie einen einfachen und kurzen Namen an, der von den meisten verstanden wird. Dieser sollte so intuitiv sein, dass ein neuer Benutzer ihn erfassen und verstehen kann, was die Variable erfassen soll.
* **Beschreibung:** Genauere Angaben darüber, wofür die Variable verwendet wird und welche Daten sie nachverfolgt. Ich halte dies kurz und einfach und passe es an die in der Benutzeroberfläche verwendete Beschreibung an. Idealerweise möchte ich nicht, dass meine Benutzer jemals das Tagging-Dokument konsultieren müssen. Wenn also eine neue Dimension im Admin-Backend eingerichtet wird, füge ich dort dieselbe Beschreibung hinzu. Auf diese Weise kann der Benutzer direkt in Workspace auf das Informationssymbol klicken, um zu verstehen, was eine Dimension ist - ohne ein Excel-Dokument aufrufen zu müssen!

![Vereinfachte Seiten-URL](assets/page-url-simplified.png)

* **Code:** Der Code aus dem Backend, der den Wert festlegt. Dies kann das Feld aus der Datenschicht auf der Seite sein, oder Sie können darauf hinweisen, dass dies mit einer Launch-Regel, einer Verarbeitungsregel usw. geschieht.
* **Klassifizierungsberichte:** Rufen alle Klassifizierungsberichte auf, die entweder mit dem Klassifizierungs-Importer oder dem Classification Rule Builder erstellt wurden
* **Lösungsumfang:** Ich finde es nützlich, alle Eigenschaften (zumindest die, die mehr als Standardvariablen verwenden) in kleinen Spalten aufzulisten und ein Häkchen für jede Dimension hinzuzufügen, die für diese Eigenschaft festgelegt wurde. Auf diese Weise können Sie einfach nach einer bestimmten Eigenschaft filtern und schnell erkennen, wo eine bestimmte Dimension festgelegt wird.
* **Konfiguration:** Admin-Benutzeroberflächeneinstellungen für jede Variable (z. B. für eVars - Ablauf, Zuordnung, Merchandising usw.)

Screenshot der Beispiel-SDR:
![Beispiel-SDR](assets/sample-sdr.png)

Es wird außerdem empfohlen, dieses Tagging-Dokument zu verwenden, um alle freien Variablen und alle „Junk“-Variablen im Auge zu behalten. Wenn eine Dimension nicht mehr nützlich ist, benötigt die Entwicklung normalerweise eine Weile, um sie zu löschen. Selbst danach kann es zum Caching kommen, oder Sie stellen fest, dass die Dimension auch an anderer Stelle festgelegt wurde. Das Bereinigen von Dimensionen ist nicht einfach und erfordert oft Geduld. Im Folgenden finden Sie einige Tipps, wie Sie Ihren Müll unter dem Bett verstecken können, damit Ihre Benutzer nicht den Überblick verlieren.

* Alle nicht verwendeten Dimensionen/Ereignisse sind entweder „frei“ oder „werden gelöscht“
   * Wenn die Dimension in den letzten 90 Tagen Junk-Werte hatte, ist der Status „wird gelöscht“
   * Wenn die Dimension mindestens in den letzten 90 Tagen frei und klar war, ist sie „frei“.
   * Markieren Sie diese als solche unter „Name“ im Tagging-Dokument, damit Sie leicht nach ihnen filtern können. Ich lasse diese im Tagging-Dokument (Excel-Datenfilter) deaktiviert, damit die Benutzer sie nicht sehen
   * Markieren Sie diese als eVar-Namen in der Benutzeroberfläche, damit die Benutzer sie bei einer Suche nicht finden (z. B. „(v6)„), und entfernen Sie die Beschreibung in der Benutzeroberfläche
* Auf diese Weise können Sie, wenn eine neue Dimension benötigt wird, in der Spalte „Name“ einfach nach „frei“ filtern, um eine saubere Dimension zu finden
* Für die Dimensionen und Ereignisse im Status „wird gelöscht“ empfehle ich, diese mit Workspace zu verfolgen:
   * Erstellen Sie ein Projekt, das nur für Administratoren sichtbar ist, mit 3 Tabellen: eVars, Props und Ereignisse. Ich verwende „Instanzen“ für die spezifischen eVars, und für Props erstelle ich HIT-Segmente, zum Beispiel mit „prop5 existiert“.
   * Datum auf „Letzte 90 Tage“ festlegen
   * Verwenden Sie die obigen Angaben als Zeilen in den 3 Tabellen, zusammen mit ihren Vorkommen.
   * Sobald etwas den Wert „0“ erreicht, markiere ich es im Tagging-Dokument als „frei“ und entferne es aus dem Workspace-Projekt

Auf diese Weise sind Ihre Daten immer sauber und Sie haben eine klare Vorstellung von Ihrem Junk.

![Übersicht über Variablen und Ereignisse](assets/variables-and-events-overview.png)

## Registerkarte „Eigenschaften“

**WAS:** In einem Eigenschaftendokument sollten all Ihre digitalen Eigenschaften - Websites, mobile Apps, andere Tools (Chat, Feedback usw.) aufgelistet werden, unabhängig davon, ob diese Eigenschaften mit [!DNL Adobe Analytics] getaggt sind oder nicht. Dies sollte als zentralisiertes, lebendiges Dokument für geschäftliche und technische Benutzer dienen.

**WARUM:** Auf diese Weise erhalten Sie einen klaren Überblick über den Journey Ihres Benutzers in all Ihren digitalen Objekten und darüber, was [!DNL Adobe Analytics] abdeckt und was nicht, sodass Sie damit beginnen können, das Hinzufügen von Tags für alle Objekte zu priorisieren, in denen sie fehlen. Indem Sie Ihr digitales Ökosystem auf diese Weise gestalten, können Sie potenzielle Möglichkeiten für eine Tagging-Strategie identifizieren, um einen vollständigen Überblick über den Journey Ihres Benutzers zu erhalten. Benötigen Sie beispielsweise eine globale Report Suite, um die Verfolgung über mehrere Domains/Sites hinweg durchzuführen? Ist eine Übergabe der Besucher-ID zwischen den Domains oder der App an das hybride Erlebnis erforderlich? Müssen interne URL-Filter für domänenübergreifendes Tracking aktualisiert werden?

**WIE:** Bestimmen Sie einen Verantwortlichen für das Dokument, um die Governance zu gewährleisten und die Verantwortung für die Verwaltung der Aktualisierungen in einer Hand zu haben.
Führen Sie auf der Registerkarte „Eigenschaften“ Folgendes auf:
* **Eigenschaftsname:** Dabei kann es sich um eine Domain, Subdomain, einen App-Namen usw. handeln. Selbst innerhalb derselben Domain sollten einige Teile getrennt verwaltet werden, wenn sie getrennt verwaltet werden (z. B. durch ein anderes Team oder eine andere Technologie).
* **Link (URL)** zur Eigenschaft, sofern verfügbar
* **Verantwortlicher und Ansprechpartner:** Führt den Hauptverantwortlichen oder die Hauptkontakte für die Eigenschaft auf.
* **Tag-Methode:** Viele von uns haben verschiedene Codemethoden und Implementierungen im Einsatz (Launch, JS-Dateien, AEP usw.). Sie können dies bei Bedarf weiter aufschlüsseln (z. B. nach Codeversion oder Tag-Management-System), aber dies ist dazu gedacht, den Überblick über all Ihre verschiedenen Codemethoden und Versionen zu behalten, wo der Code aktualisiert werden muss und wie er gepflegt werden muss. Wenn Sie [!DNL Adobe] Launch verwenden, listen Sie den Namen der Launch-Eigenschaft auf.

Denken Sie daran, alle digitalen Eigenschaften einzuschließen, auch wenn sie nicht mit [!DNL Adobe Analytics] getaggt sind. Dies hilft Ihnen, Ihre digitale Landschaft zu verstehen und zu verstehen, wie Ihre Benutzer mit all Ihren Eigenschaften interagieren.

Es wird empfohlen, dieses Dokument so einfach wie möglich zu halten und es nicht mit zu vielen Informationen zu überfrachten, damit es für verschiedene Teile des Unternehmens einfach zu interpretieren ist. [!DNL Analytics] Teams verstehen die digitale Landschaft oft besser als jedes andere Team, daher wird dieses Dokument häufig von anderen Teams und Führungskräften verwendet, um einen umfassenden Überblick zu geben.

>[!TIP]
>
>Erstellen Sie eine Dimension für den Site-Namen/die Eigenschaft in [!DNL Adobe Analytics]. Eine dedizierte Dimension (in der Regel eine eVar) in [!DNL Adobe Analytics], die den Site-/App-Namen identifiziert, ermöglicht die Segmentierung, Fehlerbehebung, Erstellung virtueller Report Suites usw. Die Vorteile sind endlos, insbesondere wenn mehrere Sites in einer (globalen) Report Suite kombiniert werden. Entscheidend ist, sicherzustellen, dass Ihre Entwicklungs-Teams diesen Wert immer in der Dimension „Eigenschaften“ festlegen, einschließlich aller Seitenladevorgänge (s.tl-Aufrufe/trackState) und aller benutzerdefinierten Ereignisse (s.tl-Aufrufe/trackAction). Verarbeitungsregeln können ein wertvolles Tool sein, das Ihnen dabei hilft, diese Werte richtig und konsistent festzulegen.

[Sehen Sie sich dieses Video von Doug &#x200B;](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/implementation/implementation-basics/creating-a-business-requirements-document.html?lang=de){target="_blank"} an, um weitere Informationen zum Ausfüllen des Implementierungs-Playbooks zu erhalten.

## Autoren

Dieses Dokument wurde gemeinsam verfasst von:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Platform Manager bei NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, Senior Consultant bei [!DNL Adobe]
