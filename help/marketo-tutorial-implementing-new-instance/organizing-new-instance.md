---
title: Neue Instanz organisieren und Namenskonventionen festlegen
description: Erfahren Sie, wie Sie eine gute Organisation in Ihrer Marketo Engage-Instanz einrichten, sodass zukünftige Marketing-Fachleute in Ihrem Unternehmen einfach durch die Programme navigieren, die Assets ändern und Berichte abrufen können.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-03T00:00:00Z
jira: KT-14813
thumbnail: KT-14813.jpeg
exl-id: 19b3de9e-53f3-4308-b46e-7b8f756c30a0
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 2%

---

# Neue Instanz organisieren und Namenskonventionen festlegen

Als Administrator bei der Implementierung einer neuen Marketo Engage-Instanz legen Sie die Grundlagen, damit zukünftige Marketing-Experten innerhalb des Unternehmens einfach durch die Instanz navigieren können. Wenn Sie sich mit der Baumstruktur und den Benennungskonventionen vertraut machen, bleibt Ihre Instanz sauber und auf einen langfristigen Erfolg eingerichtet. Dieses Tutorial enthält Beispiele, die von Adobe und Marketo Engage Champion (2019-2020), Natalie Kremer, empfohlen wurden, um Sie bei der [Organisation der Ordner und der Benennung von Assets konsistent](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630){target="_blank"} zu unterstützen.

## Warum ist die Strukturierung von Ordnern und die Anwendung von Benennungskonventionen erforderlich?

Wenn Sie in Ihrer Instanz organisiert bleiben, können Sie und Ihre Kollegen Kampagnen, Programme und Assets einfach verfolgen und die Programmleistung melden. Um den Navigationsbaum in Ihrer Instanz zu organisieren und in großem Maßstab zu erstellen, wird empfohlen, [Ordner](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders){target="_blank"}, [Standardnamenskonventionen](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#naming-schemes){target="_blank"} und Funktionen wie [Klonen](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#cloning){target="_blank"} zu verwenden.

## Organisieren einer Marketo Engage-Instanz

>[!VIDEO](https://video.tv.adobe.com/v/3422763/?quality=12&learn=on&captions=ger)

### Schritt 1: Einrichten einer Ordnerstruktur, um Ihre Programme zu ordnen

Der erste Schritt zum Organisieren Ihrer Instanz besteht darin, [eine Ordnerstruktur einzurichten](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html?lang=de) Ihr Programm und Ihre Assets einfach und geordnet zu speichern.

Im Folgenden finden Sie einige Tipps zur Strukturierung von Ordnern in einer Baumstruktur:

* Eine flache Ordnerstruktur für Auffindbarkeit beibehalten.
* Strukturieren Sie Ihre Ordner entsprechend der Team-Struktur Ihrer Organisation (z. B. Region oder Team) oder Ihrer Initiativen (z. B. Newsletter).
* Fügen Sie zeitbasierte Kennzeichnungen hinzu, um die Durchsuchbarkeit zu ermöglichen und einen angemessenen Zeitpunkt für die Archivierung anzugeben (z. B. 2024).
   * Admins wird empfohlen, Ordner mindestens einmal jährlich zu archivieren. Mit einem jährlichen Ordnernamen können Sie Live-Smart-Kampagnen einfach deaktivieren und den gesamten Ordner am Ende des Jahres archivieren.

Im Folgenden finden Sie Ordnerbeispiele für die praktische Umsetzung dieser Tipps.

**Ordnername im Baum**

>[!BEGINTABS]

>[!TAB Marketing-Aktivitäten]

![Ordner - Marketing-Aktivitäten](/help/marketo-tutorial-implementing-new-instance/assets/folders-marketing-activities.png)

>[!TAB Design Studio]

![Ordner-Design-Studio](/help/marketo-tutorial-implementing-new-instance/assets/folders-design-studio.png)

>[!TAB Datenbank]

![Ordnerdatenbank](/help/marketo-tutorial-implementing-new-instance/assets/folders-database.png)

>[!ENDTABS]

### Schritt 2: Erstellen von Ordnern in den Programmen

Wenden wir nun die Ordnerstruktur auf Programmebene an. Als Best Practice hat es sich bewährt, die lokalen Assets in Unterordnern zu unterbringen, damit Sie die Programme ordentlich halten und interne Benutzer die Programme effizient ändern oder Berichte darüber erstellen können. Zu den gebräuchlichen Unterordnern gehören E-Mails, Landingpages, Smart-Kampagnen, Listen, Berichte usw.

**Ordnername in Programmen**
* Kampagnen - *Ordner für alle Kampagnen, die Interaktionen und Status-Tracking verwalten.*
* Lokale Assets - *Ordner für alle Assets, die für dieses Programm spezifisch sind.*
   * E-Mails
   * Landingpages
   * Intelligente Kampagnen
   * Listen - *Nur erforderlich, wenn programmspezifische Listen vorhanden sind.*
   * Forms - *Nur erforderlich, wenn programmspezifische Forms vorhanden sind. Die meisten Forms sind globale Assets.*
   * Berichte - *Nur erforderlich, wenn programmspezifische Berichte vorhanden sind.*

### Schritt 3: Erstellen von Benennungskonventionen für Programme und Assets

Sobald Sie die Ordnerstruktur im Baum haben, sollten Sie die Programme und Assets konsistent benennen. Dies ist der Fall, wenn eine Standardisierung der Benennungskonventionen hilfreich wäre, um den Benennungsprozess intern zu skalieren. Im Folgenden finden Sie einige Komponenten, mit denen Sie Benennungskonventionen festlegen können, um die Durchsuchbarkeit sicherzustellen:

* Abkürzung für Programmtyp - E-Mail, Inhalt, Pflege, Webinar usw.
* Kategorie - Programmtyp - Eigenständige E-Mail, Newsletter usw.
* Termine - Startdatum des Programms
* Kurzbeschreibung - Kurze Beschreibung des Programms

Fügen wir nun die Werte in die Formel ein und generieren wir die Programmnamen für verschiedene Programmtypen.

#### Benennungsformel des Programms

| **Abkürzung für Programmtyp** | **JJJJ** | **\-** | **MM** | **\-** | **TT(optional)** | **Kategorie** | **\-** | **Kurze Beschreibung des Programms** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| AEM - E-Mail senden (E-Mail-Programm) | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| NL - Newsletter | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| ENG - Interaktionsprogramm | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| WBN - Webinar | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| IW - Interaktives Webinar | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| TS - Fachmesse | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| LE - Live-Veranstaltung (Roadshow) | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| UG - Benutzergruppe | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| WCM - Website-Inhalt | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| CS - Content Syndication | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| li - Import von Listen | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| OA - Online-Advertising | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| PPC - Pay Per Click | JJJJ | \- | MM | \- | DD(optional) | Kategorie | \- | Kurze Beschreibung des Programms |

| **Beispiele** |
| --- |
| ES 2023-10 Gated Content - XYX Whitepaper |
| WC-2023-10- Monatliches Webinar - ABC-Fallstudie |

#### Asset-Benennungsformel

Es empfiehlt sich, den Programmnamen nicht zu wiederholen und für die zukünftige Verwendung des Klonens kurze und generische Bezeichner zu verwenden. Hier sind einige Tipps, die Sie beachten sollten:

* Nummerieren Sie die Assets basierend auf ihrer Sequenz im Programmprozess.
* Trennen Sie die Benennungskomponenten mit &quot;-&quot; (Bindestrich) anstelle von &quot;.“(Punkt) oder &quot;\_“ (Unterstrich).
   * Warum? Marketo Engage verwendet einen Punkt, um den Programmnamen vom Kampagnennamen zu trennen. Die Verwendung von &quot;\_“ verhindert, dass es angezeigt wird, wenn das Asset mit einem Hyperlink versehen ist.
* Verwenden Sie Standardakronyme in den Asset-Namen, um die Referenz zu verkürzen und dennoch eine einfache Erkennung zu ermöglichen.

Vor diesem Hintergrund wenden wir diese Tipps auf die folgenden Assets an und erstellen Formeln, um Namen zu generieren:

##### Benennen der Assets basierend auf der Sequenz im Programmprozess

| **Sequenz im Programmprozess** | **\-** | **Beschreibung** |
| --- | --- | --- |
| 01 | \- | Beschreibung |
| 02 | \- | Beschreibung |
| 03 | \- | Beschreibung |

| **Beispiele: Smart-Liste** |
| --- |
| 01-E-Mail senden |
| 02-geöffnet |
| 03-geklickt |
| 04 Ausgefülltes Formular |
| 05-beeinflusst (Programmerfolg) |
| 06-unsubscribed |

##### Benennen Sie die Assets mit der Abkürzung für den Asset-Typ

| **Abkürzung für Asset-Typ** | **Asset-Typ** | **\-** | **Beschreibung des Ziels** |
| --- | --- | --- | --- |
| LP - Landingpage | LP | \- | Beschreibung des Ziels |
| E-MAIL - E-MAIL (AUSGEHEND) | E-MAIL | \- | Beschreibung des Ziels |
| WARNHINWEIS - E-Mail-Warnhinweis | ALARM | \- | Beschreibung des Ziels |
| WF - Web-Formular | WF | \- | Beschreibung des Ziels |
| EXCL - Ausschlussliste | EXKL | \- | Beschreibung des Ziels |
| SLST - Smart-Liste | SLST | \- | Beschreibung des Ziels |
| LST - Statische Liste | LIST | \- | Beschreibung des Ziels |

| **Beispiele** |
| --- |
| LP-Registrierung |
| LP-Danke |
| EMAIL-Outbound |
| EMAIL-Newsletter |
| EMAIL-Invitation |
| EMAIL-Reminder |
| EXCL-Mitbewerber |

##### Benennen Sie die herunterladbaren Dateien (.pdf) mit der Abkürzung Asset-Typ

| **Asset-Typ** | **Inhaltsbeschreibung** | **\-** | **Abkürzung für Asset-Typ** | **,** | **PDF** |
| --- | --- | --- | --- | --- | --- |
| WP - Whitepaper | Inhaltsbeschreibung | \- | WP | . | PDF |
| CS - Fallstudie | Inhaltsbeschreibung | \- | CS | . | PDF |
| DS - Datenblatt | Inhaltsbeschreibung | \- | DS | . | PDF |

| **Beispiele: Herunterladbare PDF-Dateien** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

>[!CAUTION]
>
>Verwenden Sie beim Benennen von Dateien in den oben genannten Beispielen keine Leerzeichen und vermeiden Sie die Verwendung von Unterstrichen &quot;\_“

## Wie geht es weiter?

* Laden Sie das Arbeitsblatt herunter: [Marketo Engage-Organisations- und Benennungskonventionen](./assets/adobe-marketo-engage-organization-and-naming-conventions.xlsx){target="_blank"} um die Erstellung der Ordnerstruktur und der Benennungskonventionen zu unterstützen.
* Nachdem Sie die erforderlichen Komponenten in Ihrer Standardnamenskonvention festgelegt haben, sollten Sie Formeln in ein Google-Blatt oder in Microsoft Excel integrieren. Zur späteren Verwendung geben Sie einfach Ihre Werte in die Tabelle ein, um Ihre Programmnamen zu generieren.
* Sobald Sie sich an einer allgemeinen Ordnerstruktur orientiert haben, ist es an der Zeit, die Vorlagen zu durchdenken, die Sie benötigen, basierend auf den häufigsten Anwendungsfällen und den häufigsten Anfragen, die Ihr Team erhält. Beginnen Sie dann mit dem Erstellen Ihrer ersten Programmvorlage. Lesen Sie weiter, um mit [Adobe Marketo Engage-Programmvorlagen zu &#x200B;](https://business.adobe.com/de/blog/how-to/get-started-with-marketo-engage-program-templates){target="_blank"}.

### Autoren

{{natalie-kremer}}

{{amy-chiu}}
