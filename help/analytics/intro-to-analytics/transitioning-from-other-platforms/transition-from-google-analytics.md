---
title: Umfassende Anleitung für den Wechsel von  [!DNL Adobe Analytics]  zu Google [!DNL Analytics]
description: Erfahren Sie, wo äquivalente Funktionen zu finden sind und wie Sie diese beim Wechsel von Google  [!DNL Analytics]  effizient nutzen können [!DNL Adobe Analytics]
solution: Analytics
feature: Third-party Integration
role: User
level: Beginner
kt: 9830
thumbnail: 34749.jpg
exl-id: 646bdc8f-c95e-40be-b2f7-8e4ba5653d91
source-git-commit: 02e3a6dfa59df45113242bd8e874e18e9e1efd58
workflow-type: tm+mt
source-wordcount: '3323'
ht-degree: 0%

---

# Umfassende Anleitung für den Wechsel von Google [!DNL Analytics] zu [!DNL Adobe Analytics]{#comprehensive-guide-for-transitioning-to-adobe-analytics}

## 1. Einführung

Eine der größten Herausforderungen bei der Umstellung von einem Tool auf ein anderes besteht darin, zu lernen, wo die entsprechende Funktionalität zu finden ist und wie man sie effizient nutzt. Diese Ausführungen sind Teil einer umfangreicheren Anleitung, die Benutzern den Umstieg auf [!DNL Adobe Analytics] erleichtern soll (entweder als neuer Benutzer oder als Benutzer, der aus Google [!DNL Analytics] kommt). Ein ausführlicher Vergleich mit GA, dem wahrscheinlich bekanntesten Vergleichs-Tool, wird den Benutzern helfen, ihr vorhandenes Wissen auf das neue Toolset anzuwenden. Wenn es keinen Ersatz für Übung gibt, hilft dies Ihnen, den Einstieg zu finden und Frustrationen, auf die Sie während dieser Zeit stoßen können, zu reduzieren.

Wir sollten kurz die Terminologie vergleichen:

| **Beschreibung** | **[!DNL Adobe Analytics]** | **Google-[!DNL Analytics]** |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------|
| Eine Ereignismetrik, die anzeigt, dass eine Seite (oder ein Bildschirm in einer Mobile App) angesehen wurde | Seitenansicht | Seitenansicht |
| Eine Metrik, die eine Gruppe von Interaktionen auf Ihrer Website oder App darstellt, die im selben Zeitrahmen stattfinden | Besuch | Session |
| Eine Metrik, die ein identifiziertes Gerät definiert (basierend auf mehreren Kriterien, einschließlich Cookies und anderen Verhaltensmustern, um Benutzerinformationen zusammenzufügen) | Unique Visitor | Benutzer |

## 2. Die Schnittstellen

Wenn Leute [!DNL Adobe Analytics] und Google [!DNL Analytics] vergleichen, äußern sie, dass [!DNL Adobe] Oberfläche zunächst abschreckend sei. Das stimmt, aber es ist auch - ob Sie es glauben oder nicht - eine Stärke und keine Schwäche. [!DNL Adobe] bietet eine breite Palette von Tools und Flexibilität bei der Datenvisualisierung, sodass Sie viel mehr Freiheit bei der Erstellung dessen haben, was Sie benötigen.

Beginnen wir mit dem „In-Site“-Reporting.

### 2.1. In-Site-Reporting

#### 2.1.1. Startbildschirm

Sowohl [!DNL Adobe Analytics] als auch Google [!DNL Analytics] eine Möglichkeit bieten, die erste Ansicht anzupassen, die Benutzende bei der Anmeldung sehen.

##### 2.1.1.1. Workspace / Benutzerdefinierter Startbildschirm ([!DNL Adobe Analytics])

[!DNL Adobe Analytics] erstellt keinen vordefinierten Bericht, den alle Benutzer bei der Anmeldung sehen können. Die standardmäßige Startseite bringt den Anwender zum Workspace-Startbildschirm, der jedem Anwender alle Workspace-Berichte anzeigt, die er erstellt hat oder die für ihn freigegeben wurden. Außerdem kann jeder Benutzer einen dieser Berichte als Startbildschirm festlegen, wenn er dies wünscht.

![workspace-create-project](assets/ga-to-aa_1.png)

Weitere Informationen zum Arbeitsbereich finden Sie weiter unten in diesem Handbuch. Siehe Abschnitt 2.1.2.1

>[!TIP]
>
>Erstellen/Teilen Sie einige Standardberichte für Ihre Organisation, damit sie einen Ausgangspunkt haben, um Informationen zu sehen, ohne gleich ihre eigenen Berichte erstellen zu müssen.



##### 2.1.1.2. Startbildschirm-Insights (Google [!DNL Analytics])

* Auf dem Google [!DNL Analytics]-Startbildschirm sind einige Visualisierungen vorkonfiguriert. Diese umfassen u. a. Folgendes:
* Benutzer, Sitzungen, Absprungrate und Sitzungsdauer in den letzten sieben Tagen
* Benutzer nach Tageszeit in den letzten 30 Tagen
* Aktuelle Benutzer und die aktivsten Seiten
* Traffic-Kanal, Source/Medium und Empfehlungen in den letzten sieben Tagen
* Sitzungen nach Land in den letzten sieben Tagen
* Top-Seiten der letzten sieben Tage
* Trend der aktiven Benutzer für die letzten 30 Tage
* und weitere

GA4-Benutzer haben mehr Möglichkeiten, ihre eigenen Berichte anzupassen und zum Startbildschirm hinzuzufügen.

![google-analytics-interfaces](assets/ga-to-aa_2.png)

Dies ist wahrscheinlich die Sache, die Sie am meisten in [!DNL Adobe Analytics] vermissen. Es gibt keinen vorgefertigten Startbildschirm für Sie. Sie können jedoch ganz einfach eine benutzerdefinierte Workspace einrichten, um das zu replizieren, was Sie aus der obigen Liste benötigen, und es als Ihren Startbildschirm festlegen. Weitere Informationen zu diesem Thema finden Sie später (oder im Abschnitt 2.1.2.1 [!DNL Adobe] Workspace).

#### 2.1.2. Report Builder vor Ort

Zusätzlich zu den einfachen Berichten, die die Analyse-Tools bereitstellten, bietet jedes Tool auch leistungsfähigere Tools, mit denen Sie Ihre eigenen benutzerdefinierten Berichte erstellen können.

##### 2.1.2.1. [!DNL Adobe Analytics] Workspace

Dies ist das Kraftzentrale von [!DNL Adobe Analytics], seit seiner Einführung im Jahr 2017 ist es der erste Ort für [!DNL Analytics] Analysen und der Hauptgrund dafür, dass der Abschnitt „Berichte“ demnächst eingestellt wird.

Mit diesem Tool können Sie Berichte mit nahezu vollständiger Freiheit erstellen.

Der Bericht kann in Bereiche unterteilt werden, die eine beliebige Anzahl von Visualisierungen enthalten können. Bedienfelder können auf allgemeine Informationen wie Datumsbereiche und allgemeine Segmentfilter festgelegt werden.

Sowohl die Bedienfelder als auch die darin enthaltenen Visualisierungen können in der Größe verändert und verschoben werden, um Elemente nebeneinander oder übereinander anzuzeigen. Wenn Sie also zwei verschiedene Datenreihen nebeneinander vergleichen möchten, können Sie Bereiche erstellen, die in der Mitte 50/50 geteilt sind und die beiden Sites nebeneinander zeigen, um einen einfachen Vergleich zu ermöglichen.

Benutzern stehen eine Vielzahl von Visualisierungen zur Verfügung:

* Freiformtabelle
* Kohortentabelle
* Fallout
* Fluss
* Diagramme
   * Bereich (gestapelt und ungestapelt)
   * Zeile
   * Streuung
   * Balken (gestapelt und ungestapelt)
   * Horizontales Säulendiagramm
   * Ringdiagramm
   * Histogramm
   * Horizontalbalken (gestapelt und ungestapelt)
* Zuordnung
* Zusammenfassungsblöcke
   * Zusammenfassungsänderung
   * Zusammenfassender Text
   * Text (freies Textfeld zur Eingabe zusätzlicher Informationen, um den Kontext zu verdeutlichen)
* Venn

Jeder Bereich und jede Visualisierung kann betitelt und mit einer Beschreibung versehen werden, um den Kontext der angezeigten Informationen zu verdeutlichen.
In [!DNL Adobe] gelten Segmente (im Wesentlichen Filter für Daten) rückwirkend, und diese können in Spalten Ihrer Freiformtabellen übernommen werden, um Daten nebeneinander zu vergleichen. Wenn ein Benutzer beispielsweise zwei verschiedene Kategorien auf seiner Website hinsichtlich des Traffics vergleichen möchte, kann er ein Segment für „Kategorie A“ und ein anderes Segment für „Kategorie B“ erstellen.

![analytics-page-views-report](assets/ga-to-aa_3.png)

Freiformtabellen ermöglichen mehrere Spalten und eine beliebige Segmentierung, um die Daten nach Belieben zu visualisieren.

Wenn Sie keine Aufschlüsselung nach Datum sehen möchten, ziehen Sie einfach per Drag-and-Drop eine andere Dimension oder ein Segment dorthin, um die Daten auf eine andere Weise anzuzeigen. Verwenden Sie beispielsweise Segmente für den Gerätetyp und fügen Sie dann eine Aufschlüsselung nach Betriebssystem für Ihre Mobile-/Tablet-Benutzer hinzu:

![analytics-compare-page-views-report](assets/ga-to-aa_4.png)

Mit Workspace können Sie Ihrer Kreativität freien Lauf lassen, Sie sind nicht auf „standardmäßige“ Aufschlüsselungen beschränkt. Sie können die Visualisierungen erstellen, die Sie benötigen, um tiefgehende Einblicke in die auszuführenden Vergleiche zu erhalten.

>[!TIP]
>
>Haben Sie keine Angst zu spielen und zu erkunden. Es gibt so viele Möglichkeiten, über den Tellerrand zu schauen. Überprüfen Sie außerdem, ob das, was Sie erstellt haben, auch das zeigt, was Sie vermuten. Erfahrung hilft!

Sie können ad-hoc berechnete Metriken oder Segmente erstellen, die nur innerhalb des Berichts verwendet werden, um zu verhindern, dass Ihr Segment- und Berechnungs-Repository überflutet wird. Auf diese Weise können Sie zielgerichtete Elemente erstellen, die für bestimmte Berichte benötigt werden, ohne Ihre Organisation mit Dingen zu verunsichern, die in anderen Kontexten nicht verwendbar sind.

Diese Ausführungen sind nur eine Einführung in dieses Tool. Es gibt weitere umfassende Handbücher, die Ihnen den Einstieg erleichtern. Nachdem Sie diese Handbücher durchgesehen haben, erstellen Sie umfassende Berichte wie die folgenden:

![workspace-dashboard](assets/ga-to-aa_5.png)

Arbeitsbereiche werden nicht automatisch gespeichert, sodass es einfacher ist, einen einmaligen Ad-hoc-Bericht zu erstellen, ohne das Repository Ihres Berichts zu verstopfen.

Eine weitere leistungsstarke Funktion von Arbeitsbereichen ist die Möglichkeit, interaktive Modifikatoren in Form von Dropdown-Menüs auf Ihre Berichte anzuwenden. Diese Dropdown-Menüs funktionieren nicht bei exportierten CSV- oder PDF-Dateien Ihrer Berichte. Im Live-Bericht können Sie jedoch alle Visualisierungen in einem Bedienfeld aktualisieren, um denselben Bericht unter verschiedenen Bedingungen anzuzeigen. Es können mehrere Dropdown-Listen verwendet werden. Sofern sich die Optionen nicht gegenseitig ausschließen, werden die ausgewählten Elemente gestapelt, um eine übersichtliche Darstellung der Informationen zu ermöglichen.

>[!IMPORTANT]
>
>Weitere Informationen zur Verwendung von Dropdown-Menüs und Freiform-Aufschlüsselungen finden Sie unter <https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/the-power-of-dropdown-filters-and-dimension-breakdowns-in-adobe/td-p/434680>

##### 2.1.2.2. Google-[!DNL Analytics]: Dashboards, benutzerdefinierte Berichte und gespeicherte Berichte

Google verfügt über einige Tools zum Erstellen von Berichten innerhalb der Benutzeroberfläche, die jedoch die gleiche Anzeige und die gleichen Einschränkungen wie der Abschnitt „Berichte“ aufweisen.

Nun, für diejenigen, die sich mit Google [!DNL Analytics] auskennen, wenn Sie dies lesen, könnten Sie sagen: „Moment mal, was ist mit Google Data Studio, ist das nicht eine bessere Entsprechung zu [!DNL Adobe] Workspace?“ Ja, aber Data Studio ist technisch gesehen kein Teil des [!DNL Analytics]-Tools und ermöglicht Verbindungen zu verschiedenen Datenquellen. Dieses Tool wird später im Abschnitt „Erweiterter Zugriff auf Berichte“ behandelt, insbesondere in Abschnitt 2.2.3.

Google-Dashboards und benutzerdefinierte Berichte ermöglichen es Ihnen, mehrere Visualisierungen in einem Bericht zusammenzufassen. Im Gegensatz zu Workspace sind Sie jedoch immer noch auf einfache Korrelationen beschränkt und können nicht festlegen, welche Daten in welche Spalten eingefügt werden können.

Bei benutzerdefinierten Berichten besteht eine der größten Herausforderungen darin, dass ein Filter, den Sie erstellen, für alle Registerkarten des Berichts gilt. Es gibt keine Möglichkeit, zwei verschiedene Filter innerhalb desselben Berichts zu vergleichen.

Für Oberflächenvergleiche ist dies jedoch kein Problem. All diese Funktionen ähneln denen der [!DNL Adobe] älteren Dashboards, benutzerdefinierten Berichten und Lesezeichen. Grundlegende Tools zur Erfüllung Ihrer Anforderungen, die in der Report Suite enthalten sind.

#### 2.1.3. Berichte

Sowohl Google als auch [!DNL Adobe] verfügen über einige navigierbare Berichte, bei denen es sich um vorgefertigte Tabellen und einfache Zeitachsendiagramme handelt, die auf einer Dimension basieren.

##### 2.1.3.1. [!DNL Adobe Analytics] Berichte

[!DNL Adobe Analytics] enthält auch einen Abschnitt „Berichte“, der jedoch schrittweise zugunsten von Analysis Workspace eingestellt wird. Tatsächlich wurde das Ende der Lebensdauer für diese Benutzeroberfläche angekündigt, da Workspace ein leistungsfähigeres Tool ist. Die meisten dieser Tabellen können einfacher erstellt und geändert werden. Die Abschnitte von [!DNL Adobe] sind viel stärker unterteilt, was entmutigend wirken kann:

![analytics-site-metrics](assets/ga-to-aa_6.png)

Da die meisten der oben genannten Punkte über Arbeitsbereiche zugänglich sind, gebe ich einen kurzen Überblick über diese Abschnitte und ihre Beziehung zu Google [!DNL Analytics] und hebe die Berichte hervor, die hier noch relevant sind.

Website-Metriken sind das, was Sie erwarten würden, also die Standardmetriken (Seitenansichten, Unique Visitors, Besuche und benutzerdefinierte Ereignisse, die Sie eingerichtet haben). Dies ähnelt dem Verhaltensbericht in GA, enthält aber auch einige der Informationen, die Sie unter Zielgruppe finden würden (da [!DNL Adobe] die Metriktypen nicht aufteilt).

Hier finden Sie Bot-Berichte. Der Traffic von Bots wird aus allen Standardberichten ausgeschlossen. Es gibt jedoch zwei Berichte, die Aufschluss darüber geben, was passiert und welche Bots auf Ihre Site kommen. Dies ist besonders nützlich, wenn Sie benutzerdefinierte Bot-Regeln eingerichtet haben, um bekannte Spam-Bots auszuschließen, die häufig Ihre Website besuchen. Sie können einen Einblick in die Aktivitäten dieser Bots erhalten, ohne dass Ihre Hauptberichte überflutet werden, aber dieser Traffic. Bot-Berichte sind derzeit nicht über Workspace verfügbar (aber neue Berichtsfunktionen, die in Kürze verfügbar sein werden, ermöglichen es Benutzenden, diese Informationen auch dort abzurufen).

Site-Content ist eine Gruppierung [!DNL Adobe] Standarddimensionen: Seitenname, Site-Bereiche, Hierarchien, Server und mehr. Alle diese Dimensionen sind in Workspace verfügbar.

Mobile ist eine Gruppierung mobilgerätespezifischer Daten, einschließlich Geräten, Gerätetypen und mehr. Diese sind in Workspace verfügbar.

Pfade sind in Workspace nicht verfügbar. Workspace verfügt über ein Flussdiagramm, in dem Sie die Ein- und Ausflüsse für eine einzelne Seite/einen einzelnen Wert sehen können. Im Gegensatz dazu können Sie mit „Pfade“ die am häufigsten verwendeten Pfade auf Ihrer Website anzeigen. Standardmäßig ist „Seiten“ der erste Pfadbericht, der für Sie eingerichtet wird. Sie können dies jedoch für benutzerdefinierte Eigenschaften wie den Wert „Seitentyp“ aktivieren. Sie können sich die Pfade innerhalb der Seitentypen ansehen. Ein weiterer Punkt, der mir persönlich an der Funktion „Pfade“ gefällt, ist die einfache Art und Weise, in der die Informationen präsentiert werden … Das Flussdiagramm in Workspace kann (abhängig von der angezeigten Datenmenge) schnell überwältigend werden. Ich empfehle, beide auszuprobieren… beide haben ihren Nutzen und Wert, je nachdem, was Sie erreichen möchten. Beachten Sie, dass in Flüssen jede Dimension verwendet werden kann, während die Pfadbestimmung in einer Prop im Admin-Bedienfeld eingerichtet werden muss.

Die Berichte zu Traffic-Quellen, [!DNL Campaign]s und Marketing-Kanälen ähneln alle dem Akquisebericht bei Google. Der Bericht über Traffic-Quellen konzentriert sich auf die tatsächlichen Referrer, [!DNL Campaign]s konzentriert sich auf Ihre [!DNL Campaign]-Codes, und der Bericht über Marketing-Kanäle konzentriert sich ebenfalls auf [!DNL Campaign]-Codes, wendet aber zusätzlich eine von Ihnen festgelegte Logik an, wie die Informationen zu verarbeiten sind. [!DNL Adobe] bietet mehr Freiheit beim Einrichten Ihrer Regeln. Im Gegensatz dazu erledigt Google viele Dinge für Sie, und das ist ein Umdenken. Standardmäßig beträgt die Attribution für [!DNL Campaign]-Codes in Google sechs Monate. Die Attribution von [!DNL Adobe] ist standardmäßig auf eine Woche eingestellt. Dies kann in Ihren Admin-Einstellungen geändert werden, aber in Workspace können Sie tatsächlich eine benutzerdefinierte Attribution auf jede Dimension anwenden, was Ihnen viel mehr spontane Flexibilität bietet.

Die Berichte zur Besucherbindung und zum Besucherprofil ähneln den Zielgruppenberichten in Google [!DNL Analytics]. Die Kundenbindung konzentriert sich eher auf die Häufigkeit der Wiederkehr, während das Besucherprofil eher auf die Geografie und Technologie der Benutzer ausgerichtet ist.

Benutzerspezifische Konversions- und Traffic-Berichte sind beide benutzerspezifische Dimensionsberichte. Konversionen sind eVars. Sie können für einen benutzerdefinierten Ablauf den Wert festlegen, z. B. Treffer, Besuch, Monat und Jahr. Dieser Wert bleibt für einen Benutzer für den konfigurierten Zeitrahmen persistent, es sei denn, er wurde überschrieben. Traffic-Variablen sind Props. Sie können diese auch für Pfadberichte oder als Listenelemente einrichten, die mehrere Werte basierend auf einem Trennzeichen Ihrer Wahl aufteilen.

„Medien“ ist für Dinge wie Videos oder Audiodateien, für die Sie ein spezielles Medien-Tracking eingerichtet haben.

Benutzerdefinierte Berichte ist ein Abschnitt, in dem ein Benutzer die Spalten und Aufschlüsselungen, die er in der Berichtsschnittstelle erstellt hat, anpassen und als benutzerdefinierten Bericht speichern kann. Da Workspace jedoch, wie oben erwähnt, so viel leistungsfähigere Aufschlüsselungen und Korrelationen ermöglicht, sollten alle benutzerdefinierten Anpassungen dort vorgenommen werden. Dies war eine gute Lösung, bevor Workspace existierte.

Der Abschnitt „Lesezeichen“ ähnelt den benutzerdefinierten Berichten, wo häufig verwendete Berichte in der Berichtsschnittstelle mit Lesezeichen versehen werden können, damit sie leichter gefunden werden können.

Dashboard war ein älteres Produkt, das es ermöglichte, Reportlets von Daten in einer Visualisierung zu kombinieren. Die Funktionalität in Workspace (Abschnitt 2.1.2.1) ist jedoch so viel einfacher zu handhaben, dass es nur noch als Zugangspunkt zu veralteten Berichten existiert, die neu erstellt werden sollten, bevor diese Funktion eingestellt wird.

Zielvorgaben ermöglichen es, einen Bericht zu erstellen, der auf einer Zielvorgabe innerhalb eines bestimmten Zeitraums basiert. Teams überwachen Kampagnen, um festzustellen, ob sie auf dem richtigen Weg sind, um ihre Traffic-Ziele zu erreichen.

Alle Berichte in diesem Bereich können nach mehreren Metrikspalten und Dimensionen aufgeschlüsselt werden. Die Einfachheit der Visualisierungen und die Logik, die sich hinter den möglichen Korrelationen verbirgt, können jedoch manchmal frustrierend sein.

##### 2.1.3.2. Google [!DNL Analytics] Berichte

Google [!DNL Analytics] unterteilt diese Berichte in die folgenden Abschnitte: Echtzeit, Zielgruppe, Akquise, Verhalten und Gespräche (in GA3) und in Lebenszyklus (mit den Unterabschnitten Akquise, Interaktion, Monetarisierung, Kundenbindung) und Benutzer (mit den Unterabschnitten Demografie und Technik).

![google-analytics-interface-compare](assets/ga-to-aa_7.png)

Sie können diese Visualisierungen geringfügig anpassen, eine sekundäre Dimensionsaufschlüsselung hinzufügen, die Visualisierung ändern, einen Filter für die Daten erstellen und vieles mehr. Sie können Ihre Anpassungen als gespeicherten Bericht speichern.

So erhalten Sie schnell und einfach Einblicke in Ihre Daten. Sie können jedoch nicht Dinge wie Benutzer mit Seitenansichten für eine Seite in derselben Tabelle vergleichen und Sie können nicht mehr als eine zusätzliche Dimension hinzufügen, um zusätzliche Daten anzuzeigen.

Diese sind gut für schnelle analytische Daten, aber wenn Sie wirklich tief graben müssen, leiden sie unter den Einschränkungen.

### 2.2. Erweiterter Zugriff auf Berichte

Zusätzlich zum „In-Site-Reporting“ bieten die meisten Tools erweiterte Funktionen, mit denen Sie Ihre Analyse außerhalb der Tools durchführen und etwas Individuelleres erstellen können.

#### 2.2.1. [!DNL Adobe Analytics] Report Builder (Microsoft® Excel-Erweiterung)

Workspace ist ein großartiges Tool, aber manchmal müssen Sie Ihre Daten in eine benutzerdefinierte Kalkulationstabelle übertragen, möglicherweise damit Sie mehrere Datenquellen zusammenfügen können. An dieser Stelle kommt der Report Builder ins Spiel.

Report Builder ist ein Plug-in für Microsoft® Excel, mit dem Sie Verbindungen zu Ihren [!DNL Adobe Analytics] erstellen können, um tabellarische Daten zu erhalten, die Sie in Excel bearbeiten können. Um dies effizient zu nutzen, würden Sie im Allgemeinen die Daten in einige Rohdaten-Registerkarten einlesen und dann Zellverweise in Excel verwenden, um die Daten aus diesen Registerkarten in einen einzigen konsolidierten Bericht einzufügen und dann Diagramme und Visualisierungen zu erstellen.

>[!NOTE]
>
>Der Report Builder verfügt über eine spezielle Berechtigung, die auf Ihre Benutzenden angewendet werden muss, um auf dieses Plug-in zuzugreifen. Diese Berechtigung sollte Benutzern erteilt werden, die gelernt haben, wie man das Tool richtig verwendet.

#### 2.2.2. [!DNL Adobe Analytics] API-Verbindung

Wenn Sie [!DNL Adobe Analytics] Daten mit etwas anderem als Excel verarbeiten müssen und die verarbeiteten Daten einschließlich der Bot-Regel-Ausschlüsse benötigen, verwenden Sie die API von [!DNL Adobe], um die Daten direkt abzurufen. Verarbeiten Sie dann die Daten mithilfe eines Skripts oder fügen Sie sie einer Datenbank hinzu, um sie mit einem anderen System zu verwenden.

Es sollte beachtet werden, dass die API nach wie vor Korrelationsdaten abruft, wobei die in der Abrufanfrage angegebenen Aufschlüsselungen und Segmente angewendet werden.

[!DNL Adobe]s Workspace (Abschnitt 2.1.2.1) verwendet die API zum Erstellen der Berichte. Wenn Sie in Workspace den Debugging-Modus aktivieren, werden die verwendeten API-Aufrufe genau angezeigt. Auf diese Weise können Sie Ihre API-Aufrufe schnell erstellen. Wenn Sie die Daten, die Sie abrufen möchten, mit Workspace erstellen und validieren, verwenden Sie diese API-Aufrufe, um die Daten an Ihre eigene Verarbeitung weiterzuleiten.


#### 2.2.3. Google [!DNL Analytics] Data Studio

Wenn Sie weitergelesen haben, wissen Sie bereits von oben, dass ich Data Studio als Äquivalent zu Workspace von [!DNL Adobe] erwähnt habe. Mit Data Studio können Sie Google-[!DNL Analytics], aber auch Daten aus anderen Quellen abrufen. Dies ist hilfreich, wenn Sie Ihre Analysedaten mit anderen erfassten Daten zusammenführen möchten. Bei Google [!DNL Analytics] gibt es jedoch die gleichen Einschränkungen bei der Visualisierung. Die Art und Weise, wie die Zeilen und Spalten gebildet werden, ist immer noch begrenzt.

Es ist immer noch ein leistungsstarkes Tool, und ich würde niemanden davon abraten, es zu verwenden. Meine persönliche Erfahrung ist, dass ich das starre Verhalten ziemlich einschränkend finde.


#### 2.2.4. Google-Tabellenerweiterung

Für meine eigenen Zwecke, wenn ich erweiterte Daten aus Google [!DNL Analytics] abrufen muss, ist mein persönliches Tool der Wahl die Google-Tabellenerweiterung. Obwohl ich mehrere Verbindungen zu meinen GA-Tabellen herstellen muss, kann ich auf die Zellen der Rohdaten verweisen und die benötigten Berichte erstellen. Anschließend visualisiere ich sie mithilfe der Diagrammfunktionen von Google Spreadsheet.


## 3. Exporte von Rohdaten

Wenn Sie wirklich Rohdaten benötigen, bieten sowohl [!DNL Adobe] als auch Google die Möglichkeit, Informationen auf diese Weise abzurufen.

### 3.1. [!DNL Adobe] Daten-Feed

In Abschnitt 2.2.2 habe ich erwähnt, dass die [!DNL Adobe Analytics]-API aus „verarbeiteten Daten“ stammt. Der Rohdaten-Feed ruft Daten ab, die durch die „Verarbeitungsregeln“ verarbeitet wurden, die im Admin-Bedienfeld eingerichtet wurden, aber diese Rohdaten enthalten alle Daten, die überall sonst ausgeschlossen sind.

Das bedeutet, dass alle Ihre Bot-Ausschlüsse, intern gefilterten IP-Daten und anderen ausgeschlossenen Daten in den Rohdaten-Feeds enthalten sind. Es gibt Flags zur Kennzeichnung dieser Daten. Wenn Sie also einen Data Lake erstellen, kann das Engineering-Team eine Logik zur entsprechenden Verarbeitung dieser Daten erstellen.

Die Rohdaten-Feeds können so angepasst werden, dass alle Datenspalten oder nur bestimmte Spalten gesendet werden, wenn Sie einen spezifischeren Feed benötigen.

Die Feeds können direkt an FTP, SFTP oder S3 gesendet werden.


### 3.2. Google Big Query

Leider ist dies ein Google-Tool, mit dem ich keine Erfahrung habe. Theoretisch sollte er dem Daten-Feed von [!DNL Adobe] ähneln, sodass Ihr Entwicklungsteam auf Rohdaten aus Ihrem Google-[!DNL Analytics] zugreifen kann.

Statt jedoch einen vollständigen Dump der Rohdaten bereitzustellen, ermöglicht es Ihren Ingenieuren, über SQL-Abfragen auf die Daten zuzugreifen, um gezielte Rohdaten oder alle Spalten der Rohdaten abzurufen.

## 4. Schlussfolgerung

Wie bei jedem System ist Übung erforderlich, um sich mit dem Tool vertraut zu machen. Wir hoffen, dieses Handbuch hilft Ihnen bei den ersten Schritten oder gibt Ihnen Tipps, wie Sie [!DNL Adobe Analytics] besser nutzen können.

Ich möchte jedoch betonen, dass ich empfehlen würde, in Ihrer Implementierungsstrategie sowohl [!DNL Adobe Analytics] als auch Google-[!DNL Analytics] zu verwenden (auch wenn die Google-[!DNL Analytics] nur die kostenlose Version ist). Auf diese Weise können Sie über ein Backup-System verfügen, um sicherzustellen, dass Sie über Daten verfügen, da kein System unfehlbar ist.

Neben diesem Handbuch stehen Ihnen viele weitere Ressourcen zur Verfügung, die Sie bei der Verbesserung Ihrer Strategie unterstützen können:

* [[!DNL Adobe] Experience League](https://experienceleague.adobe.com/de#home) - Enthält Tutorials, Videos, Dokumentation und Community-Foren
* [[!DNL Adobe] Benutzergruppen](https://analytics-augs.adobe.com/) - Ein zentraler Treffpunkt für von der Community organisierte Events, die den Benutzern helfen, miteinander in Kontakt zu treten und ihre Implementierungen zu verbessern.
* [[!DNL Adobe Analytics] YouTube-Kanal für Benutzergruppen](https://www.youtube.com/channel/UCQOHnCs7KZgsuFHVzwboQuA) - Konnten Sie keine [!DNL Adobe Analytics] Benutzergruppensitzung erstellen? Sehen Sie sich frühere Benutzergruppensitzungen auf der ganzen Welt an, um mehr darüber zu erfahren, wie Ihre Kollegen das Tool verwenden.
* [Measure Chat Slack Channel](https://www.measure.chat/) - Treten Sie mit [!DNL Adobe Analytics] Anwendern in der ganzen Welt in Kontakt und tauschen Sie Branchenkenntnisse aus, stellen Sie Fragen an Ihre Kollegen und schließen Sie sich Interessengruppen an.
* und vieles mehr!

## Autor

Dieses Dokument wurde verfasst von:

![Jennifer Dungan](assets/Jennifer_Dungan_Headshot150.png)

Jennifer Dungan, Optimization Manager [!DNL Analytics] bei Torstar

[!DNL Adobe Analytics] Champion
