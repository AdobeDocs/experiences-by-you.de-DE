---
title: Umfassende Anleitung für die Umstellung von Google [!DNL Analytics] auf  [!DNL Adobe Analytics] von
description: Erfahren Sie mehr über den Speicherort äquivalenter Funktionen und wie Sie diese beim Übergang von Google [!DNL Analytics] zu [!DNL Adobe Analytics] effizient verwenden können.
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

# Umfassende Anleitung für die Umstellung von Google [!DNL Analytics] auf [!DNL Adobe Analytics]{#comprehensive-guide-for-transitioning-to-adobe-analytics}

## 1. Einleitung

Eine der größten Herausforderungen beim Übergang zwischen verschiedenen Tools besteht darin, zu lernen, wo entsprechende Funktionen zu finden sind und zu lernen, wie sie effizient genutzt werden können. Diese Diskussion ist Teil eines umfangreicheren Handbuchs, das Benutzern den Übergang zu [!DNL Adobe Analytics] erleichtert (entweder als neuer Benutzer oder als neuer Benutzer aus Google [!DNL Analytics]). Ein tiefgehender Vergleich mit allgemein verfügbaren Informationen, da dies das wahrscheinlichste Vergleichsinstrument ist, mit dem die meisten Benutzer vertraut sind, wird bereitgestellt, um den Benutzern zu helfen, bestehende Kenntnisse mit den neuen Werkzeugen zu korrelieren. Wenn es keinen Ersatz für Übung gibt, hilft dies Ihnen, zu beginnen und Frustrationen zu reduzieren, die während dieser Zeit auftreten können.

Wir sollten einen schnellen Terminologievergleich durchführen:

| **Beschreibung** | **[!DNL Adobe Analytics]** | **Google[!DNL Analytics]** |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------|
| Eine Ereignismetrik, die eine Seite (oder einen Bildschirm in einer App) darstellt, wurde angezeigt | Seitenansicht | Seitenansicht |
| Eine Metrik, die eine Gruppe von Interaktionen auf Ihrer Website oder in Ihrer App darstellt, die im selben Zeitrahmen stattfinden | Besuch | Session |
| Eine Metrik, die ein identifiziertes Gerät definiert (basierend auf mehreren Kriterien, einschließlich Cookies und anderen Verhaltensmustern zum Zuordnen von Benutzerinformationen) | Unique Visitor | Benutzer |

## 2. Schnittstellen

Wenn man [!DNL Adobe Analytics] und Google [!DNL Analytics] vergleicht, kommentiert man, dass die Oberfläche von [!DNL Adobe] anfangs beängstigend ist. Das stimmt, aber es ist auch; glauben Sie es oder nicht; eine Stärke, keine Schwäche. [!DNL Adobe] bietet eine breite Palette von Tools und Flexibilität in Ihrer Datenvisualisierung, sodass Sie viel mehr Freiheit beim Erstellen Ihrer Daten haben.

Als Erstes betrachten wir die Berichte &quot;vor Ort&quot;.

### 2.1. In-Site-Berichte

#### 2.1.1. Startbildschirm

Sowohl [!DNL Adobe Analytics] als auch Google [!DNL Analytics] bieten eine Möglichkeit, die erste Ansicht anzupassen, die ein Benutzer bei seiner Anmeldung sieht.

##### 2.1.1.1. Workspace/Home-Bildschirm mit benutzerdefiniertem Set ([!DNL Adobe Analytics])

Bei [!DNL Adobe Analytics] wird nicht davon ausgegangen, dass ein vordefinierter Bericht erstellt wird, der allen Benutzern bei der Anmeldung angezeigt wird. Die Standard-Startseite führt den Benutzer zum Workspace-Landingscreen, auf dem alle Workspace-Berichte angezeigt werden, die er erstellt oder für ihn freigegeben hat. Außerdem kann jeder Benutzer einen dieser Berichte auf seinem Startbildschirm einrichten, sofern er dies wünscht.

![workspace-create-project](assets/ga-to-aa_1.png)

Weitere Informationen zu Workspace finden Sie weiter unten in diesem Handbuch. Siehe Abschnitt 2.1.2.1.

>[!TIP]
>
>Erstellen/teilen Sie einige Standardberichte für Ihre Organisation, sodass diese einen Ausgangspunkt haben, um Informationen anzuzeigen, ohne sofort in die Erstellung eigener Berichte eintauchen zu müssen.



##### 2.1.1.2. Home Screen Insights (Google [!DNL Analytics])

* Google [!DNL Analytics] Home Screen verfügt über einige vordefinierte Visualisierungen. Diese decken Folgendes ab:
* Benutzer, Sitzungen, Absprungrate und Sitzungsdauer in den letzten sieben Tagen
* Benutzer nach Tageszeit in den letzten 30 Tagen
* Aktuelle Benutzer jetzt und Top-aktive Seiten
* Traffic-Kanal, Source/Medium und Verweise in den letzten sieben Tagen
* Sitzungen nach Land in den letzten sieben Tagen
* Top-Seiten für die letzten sieben Tage
* Trend aktiver Benutzer für die letzten 30 Tage
* und mehr

GA4-Benutzer haben mehr Möglichkeiten, ihre eigenen Berichte anzupassen und zum Startbildschirm hinzuzufügen.

![google-analytics-interfaces](assets/ga-to-aa_2.png)

Dies ist wahrscheinlich das Einzige, was Sie am meisten in [!DNL Adobe Analytics] vermissen. Es gibt keinen Startbildschirm, der für Sie vorkonfiguriert ist. Sie können jedoch einfach eine benutzerdefinierte Workspace einrichten, um die oben genannten Elemente zu replizieren und sie als Ihren Landingscreen festzulegen. Weitere Informationen zu diesem Thema finden Sie später (oder siehe Abschnitt 2.1.2.1 [!DNL Adobe] Workspace).

#### 2.1.2. Report Builder vor Ort

Zusätzlich zu den einfachen Berichten, die von den Analysetools bereitgestellt werden, bietet jedes Tool leistungsfähigere Tools, mit denen Sie eigene benutzerdefinierte Berichte erstellen können.

##### 2.1.2.1. [!DNL Adobe Analytics] Workspace

Dies ist der Motor von [!DNL Adobe Analytics], seit seiner Einführung im Jahr 2017 ist es zum Ort für die [!DNL Analytics]-Analyse geworden und der Hauptgrund, warum der Abschnitt &quot;Berichte&quot;bald eingestellt wird.

Mit diesem Tool können Sie Berichte mit nahezu vollständiger Freiheit erstellen.

Der Bericht kann in Bedienfelder unterteilt werden, die eine beliebige Anzahl von Visualisierungen enthalten können. Bedienfelder können auf allgemeine Informationen wie Datumsbereich und allgemeine Segmentfilter festgelegt werden.

Sowohl die Bedienfelder als auch die darin enthaltenen Visualisierungen können in der Größe angepasst und verschoben werden, um Elemente nebeneinander anzuzeigen oder zu gestapeln. Wenn Sie also zwei verschiedene Datensuiten nebeneinander vergleichen möchten, können Sie Bedienfelder erstellen, die 50/50 in der Mitte unterteilen und die beiden Sites nebeneinander darstellen, um einen einfachen Vergleich zu ermöglichen.

Es stehen eine Vielzahl von Visualisierungen zur Verfügung:

* Freiformtabelle
* Kohortentabelle
* Fallout
* Fluss
* Diagramme
   * Bereich (gestapelt und nicht gestapelt)
   * Zeile
   * Streuung
   * Balken (gestapelt und nicht gestapelt)
   * Aufzählungszeichen
   * Ringdiagramm
   * Histogramm
   * Horizontalbalken (gestapelt und nicht gestapelt)
* Zuordnung
* Zusammenfassungsblöcke
   * Zusammenfassungsänderung
   * Zusammenfassungstext
   * Text (freies Textfeld zur Eingabe zusätzlicher Informationen für Kontext)
* Venn

Jedes Bedienfeld und jede Visualisierung können einen Titel erhalten und eine Beschreibung darauf angewendet werden, damit der Kontext, der die Informationen anzeigt, besser wiedergegeben wird.
In [!DNL Adobe] gelten Segmente (im Wesentlichen Filter für Daten) rückwirkend. Diese können in Spalten Ihrer Freiformtabellen gezogen werden, um Daten nebeneinander zu vergleichen. Wenn ein Benutzer beispielsweise zwei verschiedene Kategorien auf seiner Site mit Traffic vergleichen möchte, könnte er ein Segment für &quot;Kategorie A&quot;und ein anderes Segment für &quot;Kategorie B&quot;erstellen.

![analytics-page-views-report](assets/ga-to-aa_3.png)

Freiformtabellen ermöglichen nach Bedarf mehrere Spalten und Segmentierungen, um die Daten wie gewünscht zu visualisieren.

Wenn Sie keine Aufschlüsselung nach Datum sehen möchten, ziehen Sie einfach eine andere Dimension oder ein Segment dorthin, um die Daten auf eine andere Weise anzuzeigen. Verwenden Sie beispielsweise Segmente für Gerätetyp und fügen Sie dann eine Aufschlüsselung nach Betriebssystem für Ihre Mobile-/Tablet-Benutzer hinzu:

![analytics-compare-page-views-report](assets/ga-to-aa_4.png)

Workspace ermöglicht es Ihnen, Ihre Kreativität zu nutzen. Sie sind nicht auf &quot;standardmäßige&quot;Aufschlüsselungen beschränkt. Sie können die Visualisierungen erstellen, die Sie benötigen, um sich über die Vergleiche, die Sie ausführen müssen, zu informieren.

>[!TIP]
>
>Hab keine Angst zu spielen und zu erforschen. Es gibt so viele Möglichkeiten, außerhalb der Kiste zu denken. Überprüfen Sie außerdem, was Sie erstellt haben, indem Sie anzeigen, was Sie denken. Erlebnis hilft!

Sie können direkt berechnete Metriken oder Segmente erstellen, die nur im Bericht enthalten sind, um zu verhindern, dass Ihr Segment- und Berechnungsrepository überschwemmt wird. Auf diese Weise können Sie fokussierte Elemente erstellen, die für bestimmte Berichte benötigt werden, ohne Ihr Unternehmen mit Elementen zu verwechseln, die in anderen Kontexten nicht verwendet werden können.

Diese Diskussion ist nur eine Einführung in dieses Tool, es gibt weitere umfassende Anleitungen, um Ihnen den Einstieg zu erleichtern. Nachdem Sie diese Handbücher überprüft haben, erstellen Sie umfassende Berichte wie die folgenden:

![workspace-dashboard](assets/ga-to-aa_5.png)

Arbeitsbereiche werden nicht automatisch gespeichert. So ist es einfacher, einen einmaligen Ad-hoc-Bericht zu erstellen, ohne das Repository Ihres Berichts zu verstopfen.

Eine weitere leistungsstarke Funktion von Arbeitsbereichen ist die Möglichkeit, interaktive Modifikatoren in Form von Dropdown-Menüs auf Ihre Berichte anzuwenden. Diese Dropdown-Listen funktionieren nicht mit exportierten CSV- oder PDF-Dateien Ihrer Berichte. Im Live-Bericht können Sie jedoch alle Visualisierungen in einem Bedienfeld aktualisieren, um denselben Bericht unter verschiedenen Bedingungen anzuzeigen. Es können mehrere Dropdown-Listen verwendet werden. Sofern sich die Optionen nicht gegenseitig ausschließen, werden die ausgewählten Elemente stapelweise eingefügt, um eine saubere Darstellung der Informationen zu ermöglichen.

>[!IMPORTANT]
>
>Weitere Informationen zur Verwendung von Dropdown- und Freiformaufschlüsselungen finden Sie unter <https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/the-power-of-dropdown-filters-and-dimension-breakdowns-in-adobe/td-p/434680>

##### 2.1.2.2. Google [!DNL Analytics]: Dashboards, benutzerdefinierte Berichte und gespeicherte Berichte

Google verfügt über einige Tools zum Erstellen von Berichten auf der Benutzeroberfläche, die jedoch weiterhin den gleichen Anzeigeparametern und Einschränkungen des Berichtabschnitts entsprechen.

Für diejenigen, die in Google [!DNL Analytics] versiert sind, wie Sie das lesen, könnten Sie sagen: &quot;Warte mal kurz, was ist mit Google Data Studio, ist das nicht besser mit dem Workspace von [!DNL Adobe]?&quot; Ja, aber Data Studio ist technisch nicht Teil des [!DNL Analytics]-Tools und ermöglicht Verbindungen zu verschiedenen Datenquellen. Dieses Tool wird später im Abschnitt &quot;Erweiterter Zugriff auf Berichte&quot;behandelt, insbesondere Abschnitt 2.2.3.

Google-Dashboards und benutzerspezifische Berichte ermöglichen es Ihnen, mehrere Visualisierungen in einem Bericht zusammenzuführen. Im Gegensatz zu Workspace sind Sie jedoch weiterhin in einfache Korrelationen eingeschlossen und erfahren, welche Daten in welche Spalten eingefügt werden können.

Eine der größten Herausforderungen in benutzerspezifischen Berichten besteht darin, einen Filter zu erstellen. Dieser gilt für alle Tabs des Berichts. Es gibt keine Möglichkeit, zwei verschiedene Filter im selben Bericht zu vergleichen.

Bei Oberflächenvergleichen wird der Vorgang ausgeführt. Diese ähneln den [!DNL Adobe] alten Dashboards, benutzerspezifischen Berichten und Lesezeichen. Grundlegende Tools zur Unterstützung Ihrer Anforderungen, die sich in der Report Suite befinden.

#### 2.1.3. Berichte

Sowohl Google als auch [!DNL Adobe] verfügen über einige navigierbare Berichte, bei denen es sich um pro-erstellte Tabellen und grundlegende Timeline-Diagramme handelt, die auf einer Dimension basieren.

##### 2.1.3.1. [!DNL Adobe Analytics] Berichte

[!DNL Adobe Analytics] verfügt auch über einen Abschnitt &quot;Berichte&quot;, der jedoch schrittweise zugunsten von Analysis Workspace eingestellt wird. Tatsächlich wurde für diese Schnittstelle das Ende des Lebenszyklus angekündigt, da Workspace ein leistungsfähigeres Werkzeug ist. Die meisten dieser Tabellen können einfacher erstellt und geändert werden. Die Abschnitte von [!DNL Adobe] sind weitaus zersplittert, und dies kann beängstigend sein:

![analytics-site-metrics](assets/ga-to-aa_6.png)

Da der Zugriff auf die meisten der oben genannten Elemente über Arbeitsbereiche erfolgt, gebe ich einen kurzen Überblick über diese Abschnitte und ihre Beziehung zu Google [!DNL Analytics]. Außerdem möchte ich hier die noch relevanten Berichte hervorheben.

Site-Metriken sind die Erwartungen, die Sie erwarten würden. Sie decken die Standardmetriken ab (Seitenansichten, Unique Visitors, Besuche und benutzerspezifische Ereignisse, die Sie eingerichtet haben). Dies ähnelt dem Verhaltensbericht allgemein, enthält jedoch auch einige der Informationen, die Sie in Audience finden würden (da [!DNL Adobe] die Metriktypen nicht aufteilt).

Hier finden Sie &quot;Bot&quot;-Berichte. Traffic von Bots wird aus allen Standardberichten ausgeschlossen. Es gibt jedoch zwei Berichte, die Aufschluss darüber geben, was passiert und welche Bots zu Ihrer Site gelangen. Dies ist besonders gut, wenn Sie benutzerdefinierte Bot-Regeln einrichten, um bekannte Spammer-Bots auszuschließen, die häufig auf Ihre Site treffen. Sie können Einblicke in die Aktivitäten dieser Bots erhalten, ohne dass Ihre Hauptberichte überflutet werden, aber dieser Traffic. Bot-Berichte sind derzeit nicht über Workspace verfügbar (aber neue Berichterstellungsfunktionen, die in Kürze verfügbar sind, ermöglichen es Benutzern, diese Informationen auch dort zu erhalten).

Site-Content ist eine Gruppierung von [!DNL Adobe] Standarddimensionen: Seitenname, Sitebereiche, Hierarchien, Server und mehr. Alle diese Dimensionen sind in Workspace verfügbar.

Mobile ist eine Gruppierung mobilgerätespezifischer Daten, einschließlich Geräten, Gerätetypen und mehr. Diese sind in Workspace verfügbar.

Pfade sind in Workspace nicht verfügbar. Workspace verfügt über ein Flussdiagramm, in dem Sie die Ein- und Ausgänge für eine einzelne Seite/einen einzelnen Wert sehen können. Im Gegensatz dazu können Sie mit Pfaden die gängigsten Pfade sehen, die auf Ihrer Website verwendet werden. Standardmäßig ist &quot;Seiten&quot;der erste Pfadbericht, der für Sie eingerichtet wurde. Sie können dies jedoch für benutzerdefinierte Eigenschaften wie den Wert &quot;Seitentyp&quot;aktivieren. Sie können sich die Pfade innerhalb von Seitentypen ansehen. Die andere Sache, die ich persönlich über Pfade mag, ist die einfache Art und Weise, wie die Informationen präsentiert werden... Das Flussdiagramm im Arbeitsbereich (je nachdem, wie viel Sie sich anschauen wollen) kann überwältigend werden. Ich empfehle, beide auszuprobieren... sie haben jeweils einen Nutzen und einen Wert, je nachdem, was Sie versuchen zu erreichen. Beachten Sie, dass jede Dimension in &quot;Fluss&quot;verwendet werden kann, während Pfade in einer Eigenschaft im Admin-Bereich eingerichtet werden müssen.

Die Berichte zu Traffic-Quellen, [!DNL Campaign]s und Marketingkanälen ähneln allesamt dem Akquisebericht des Google-Produkts. Traffic-Quellen konzentrieren sich auf tatsächliche Referrer, [!DNL Campaign]s Fokus auf Ihre [!DNL Campaign]-Codes und Marketing-Kanäle konzentrieren sich ebenfalls auf [!DNL Campaign]-Codes, wenden aber auch zusätzliche Logik an, die von Ihnen für die Verarbeitung der Informationen festgelegt wird. [!DNL Adobe] gibt mehr Freiheit beim Einrichten Ihrer Regeln. Im Gegensatz dazu macht Google viele Dinge für Sie, und das ist ein Denkwechsel. Standardmäßig beträgt die Attribution von Google für [!DNL Campaign]-Codes sechs Monate. Die Attribution von [!DNL Adobe] ist standardmäßig auf eine Woche festgelegt. Dies kann in Ihren Admin-Einstellungen geändert werden. In Workspace können Sie jedoch zusätzlich zu jeder Dimension eine benutzerdefinierte Attribution anwenden, wodurch Sie eine wesentlich größere Flexibilität &quot;direkt&quot;erhalten.

Die Berichte zur Besuchertreue und zum Besucherprofil ähneln den Zielgruppenberichten in Google [!DNL Analytics]. Die Treue konzentriert sich stärker auf die Rückkehrhäufigkeit, während sich das Besucherprofil mehr auf die Geografie und Technologie der Benutzer konzentriert.

Benutzerspezifische Konversions- und benutzerspezifische Traffic-Berichte sind beide benutzerspezifische Dimensionsberichte. Konversionen sind eVars. Sie können für einen benutzerdefinierten Ablauf den Wert festlegen, z. B. Treffer, Besuch, Monat und Jahr. Dieser Wert bleibt für einen Benutzer für den konfigurierten Zeitraum persistent, es sei denn, er wurde überschrieben. Traffic-Variablen sind Props. Sie können diese auch für Pfadsetzungsberichte oder als Listenelemente einrichten, die mehrere Werte basierend auf einem Trennzeichen Ihrer Wahl aufteilen.

Medien eignen sich für Videos oder Audiodateien, für die Sie spezielle Medien-Tracking eingerichtet haben.

Benutzerspezifische Berichte ist ein Abschnitt, in dem Benutzer die Spalten und Aufschlüsselungen anpassen können, die sie in der Berichtsoberfläche erstellt haben, und sie als benutzerspezifischen Bericht speichern können. Da Workspace jedoch, wie oben erwähnt, so leistungsstarke Aufschlüsselungen und Korrelationen ermöglicht, sollten dort alle angepassten Elemente vorgenommen werden. Das war eine gute Lösung, bevor Workspace existierte.

Der Abschnitt &quot;Lesezeichen&quot;ähnelt dem Abschnitt &quot;Benutzerspezifische Berichte&quot;, in dem häufig verwendete Berichte mit Lesezeichen in der Berichtsoberfläche versehen werden können, damit sie leichter zu finden sind.

Dashboard war ein veraltetes Produkt, mit dem Reportlets von Daten zu einer Visualisierung kombiniert werden konnten. Die Funktionalität in Workspace (Abschnitt 2.1.2.1) ist jedoch so viel einfacher zu verwenden, dass sie nur als Zugriffspunkt für veraltete Berichte existiert, die neu erstellt werden sollten, bevor diese Funktion eingestellt wird.

Mit Zielgruppen können Benutzer innerhalb eines bestimmten Zeitraums einen Bericht erstellen, der auf einem Ziel basiert. Teams überwachen Kampagnen, um festzustellen, ob sie auf dem richtigen Weg sind, um ihre Traffic-Ziele zu erreichen.

Alle hier enthaltenen Berichte waren für mehrere Metrikspalten und Dimensionsaufschlüsselungen zulässig. Die Einfachheit der Visualisierungen und einige der Logik, hinter denen Elemente korreliert werden können, könnten jedoch manchmal frustrierend sein.

##### 2.1.3.2. Google [!DNL Analytics]-Berichte

Google [!DNL Analytics] teilt diese Berichte in die folgenden Abschnitte auf: Echtzeit, Zielgruppe, Akquise, Verhalten und Konversationen (in GA3) und in den Lebenszyklus (mit den Unterabschnitten Akquise, Interaktion, Monetarisierung, Bindung) und Benutzer (mit den Unterabschnitten Demografie und Technik).

![google-analytics-interface-compare](assets/ga-to-aa_7.png)

Sie können kleinere Änderungen an diesen Visualisierungen vornehmen, eine sekundäre Dimensionsaufschlüsselung hinzufügen, die Visualisierung ändern, einen Filter für die Daten erstellen und vieles mehr. Sie können Ihre Anpassungen als gespeicherten Bericht speichern.

Diese bieten schnelle und einfache Einblicke in Ihre Daten. Sie können jedoch Dinge wie Benutzer nicht mit Seitenansichten einer Seite in derselben Tabelle vergleichen und nicht mehr als eine zusätzliche Dimension hinzufügen, um zusätzliche Daten anzuzeigen.

Diese sind gut für schnelle analytische Daten, aber wenn man wirklich tief graben muss, leiden sie unter den Einschränkungen.

### 2.2. Erweiterter Zugriff auf Berichte

Neben der &quot;In-Site-Berichterstellung&quot;bieten die meisten Tools erweiterte Funktionen, mit denen Sie Ihre Analyse außerhalb der Tools durchführen und etwas kundenspezifischer erstellen können.

#### 2.2.1. [!DNL Adobe Analytics] Report Builder (Microsoft® Excel-Erweiterung)

Workspace ist ein großartiges Tool, aber manchmal müssen Sie Ihre Daten in eine benutzerdefinierte Tabelle übertragen, um mehrere Datenquellen zusammenfügen zu können. Hier kommt Report Builder ins Spiel.

Report Builder ist ein Plug-in für Microsoft® Excel, mit dem Sie Verbindungen zu Ihren [!DNL Adobe Analytics] -Daten erstellen können, um Tabellendaten abzurufen, die Sie in Excel bearbeiten können. Um dies effizient zu nutzen, ziehen Sie die Daten in einige Rohdaten-Tabs, verwenden Sie dann Excel-Zellreferenzen, um Daten aus diesen Registerkarten in einen einzigen konsolidierten Bericht zu ziehen, und erstellen Sie dann Diagramme und Visualisierungen.

>[!NOTE]
>
>Report Builder verfügt über eine spezielle Berechtigung, die auf Ihre Benutzer angewendet werden muss, um auf dieses Plug-in zugreifen zu können. Dies sollte Benutzern gewährt werden, die gelernt haben, das Tool ordnungsgemäß zu verwenden.

#### 2.2.2. [!DNL Adobe Analytics] API-Verbindung

Wenn Sie [!DNL Adobe Analytics] -Daten von anderen Daten als Excel verarbeiten möchten und die verarbeiteten Daten einschließlich der Bot-Regelausschlüsse benötigen, verwenden Sie die API von [!DNL Adobe], um die Daten direkt abzurufen. Verarbeiten Sie dann die Daten mithilfe eines Skripts oder fügen Sie sie einer Datenbank hinzu, um sie mit einem anderen System zu verwenden.

Beachten Sie, dass die API weiterhin Korrelationsdaten abruft und dabei die Aufschlüsselungen und Segmente anwendet, wie in der Pull-Anforderung angegeben.

Die Workspace von [!DNL Adobe] (Abschnitt 2.1.2.1) verwendet die API zum Erstellen der Berichte. Wenn Sie den Debug-Modus in Workspace aktivieren, werden die genauen verwendeten API-Aufrufe angezeigt. Auf diese Weise können Sie Ihre API-Aufrufe schnell erstellen. Indem Sie Workspace zum Erstellen und Überprüfen der Daten verwenden, die Sie abrufen möchten, verwenden Sie diese API-Aufrufe, um die Daten für Ihre eigene Verarbeitung zu übertragen.


#### 2.2.3. Google [!DNL Analytics] Data Studio

Wenn Sie schon gelesen haben, wissen Sie bereits von oben, dass ich Data Studio als eine Entsprechung zu [!DNL Adobe] Workspace erwähnt habe. Mit Data Studio können Sie Google [!DNL Analytics]-Daten abrufen, aber auch Daten aus anderen Quellen. Dies ist hilfreich, wenn Sie Ihre Analysedaten mit anderen erfassten Daten zusammenführen möchten. Bei Google [!DNL Analytics] gibt es jedoch dieselben Visualisierungsbeschränkungen. Die Form der Zeilen und Spalten ist weiterhin eingeschränkt.

Es ist immer noch ein mächtiges Werkzeug, und ich würde die Leute nicht davon abhalten, es in irgendeiner Weise zu verwenden. Meine persönliche Erfahrung ist, dass ich das starre Verhalten ziemlich begrenzt finde.


#### 2.2.4. Google Spreadsheet-Erweiterung

Wenn ich Daten für meine Zwecke erweitert von Google [!DNL Analytics] abrufen muss, ist mein persönliches Tool die Google-Tabellenkalkulationserweiterung. Obwohl ich mehrere Verbindungen zu meinen GA-Tabellen herstellen muss, kann ich die Zellen aus den Rohdaten referenzieren und die benötigten Berichte erstellen. Dann visualisieren Sie sie mit den Diagrammfunktionen des Google-Arbeitsblatts.


## 3. Rohdatenexporte

Wenn Sie Rohdaten wirklich benötigen, bieten sowohl [!DNL Adobe] als auch Google die Möglichkeit, Informationen auf diese Weise abzurufen.

### 3.1. [!DNL Adobe] Daten-Feed

In Abschnitt 2.2.2 erwähnte ich, dass die [!DNL Adobe Analytics]-API aus &quot;verarbeiteten Daten&quot;abgerufen wurde. Der Rohdaten-Feed ruft Daten ab, die von den &quot;Verarbeitungsregeln&quot;verarbeitet werden, die im Admin-Bereich eingerichtet wurden. Diese Rohdaten enthalten jedoch alle Daten, die überall sonst ausgeschlossen sind.

Das bedeutet, dass sich all Ihre Bot-Ausschlüsse, internen IP-gefilterten Daten und anderen ausgeschlossenen Daten in den Rohdaten-Feeds befinden. Es gibt Flags, die diese Daten identifizieren. Wenn Sie also einen Data Lake erstellen, kann das Technikerteam eine Logik zur entsprechenden Verarbeitung dieser Daten erstellen.

Die Rohdaten-Feeds können angepasst werden, um alle Datenspalten oder nur bestimmte Spalten zu senden, wenn Sie einen zielgerichteteren Feed benötigen.

Die Feeds können direkt an FTP, SFTP oder S3 gesendet werden.


### 3.2. Google Big Query

Leider ist dies ein Google-Tool, mit dem ich keine Erfahrung gemacht habe. Theoretisch sollte sie dem Daten-Feed von [!DNL Adobe] ähneln und Ihrem Technikerteam den Zugriff auf Rohdaten aus Ihrem Google [!DNL Analytics]-Konto ermöglichen.

Anstatt jedoch eine vollständige Ablage von Rohdaten bereitzustellen, können Ihre Ingenieure über SQL-Abfragen auf die Daten zugreifen, um gezielte Rohdaten oder alle Spalten von Rohdaten abzurufen.

## 4. Schlussfolgerung

Wie jedes System ist Übung erforderlich, um sich mit dem Werkzeug vertraut zu machen. Hoffentlich hilft Ihnen dieses Handbuch bei den ersten Schritten oder bietet Tipps, wie Sie die Verwendung von [!DNL Adobe Analytics] verbessern können.

Ich möchte jedoch betonen, dass ich empfehlen würde, sowohl [!DNL Adobe Analytics] als auch Google [!DNL Analytics] in Ihrer Implementierungsstrategie zu verwenden (auch wenn die Google [!DNL Analytics] nur die freie Version ist). Dadurch können Sie über ein Backup-System verfügen, um sicherzustellen, dass Sie über Daten verfügen, da kein System unfehlbar ist.

Neben diesem Handbuch stehen Ihnen viele Ressourcen zur Verfügung, die Ihnen helfen, Ihre Strategie zu verbessern:

* [[!DNL Adobe] Experience League](https://experienceleague.adobe.com/de#home) - Enthält Tutorials, Videos, Dokumentationen und Community-Foren
* [[!DNL Adobe] Benutzergruppen](https://analytics-augs.adobe.com/) - Ein Hub von Community-ausgeführten Ereignissen, die Benutzern dabei helfen, miteinander zu kommunizieren und ihre Implementierungen zu verbessern.
* [[!DNL Adobe Analytics] Benutzergruppen YouTube Channel](https://www.youtube.com/channel/UCQOHnCs7KZgsuFHVzwboQuA) - Kann keine [!DNL Adobe Analytics] Benutzergruppensitzung durchführen? Sehen Sie sich frühere Benutzergruppensitzungen auf der ganzen Welt an, um mehr darüber zu erfahren, wie Ihre Kollegen das Tool verwenden.
* [Chat-Slack-Kanal messen](https://www.measure.chat/) - Stellen Sie eine Verbindung zu [!DNL Adobe Analytics] -Benutzern weltweit her und tauschen Sie Branchenkenntnisse aus, stellen Sie Fragen an Ihre Kollegen und schließen Sie sich messorientierten Interessengruppen an.
* und mehr!

## Autor

Dieses Dokument wurde geschrieben von:

![Jennifer Dungan](assets/Jennifer_Dungan_Headshot150.png)

Jennifer Dungan, Optimierungs-Manager [!DNL Analytics] in Torstar

[!DNL Adobe Analytics] Champion
