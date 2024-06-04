---
title: Neue Instanz organisieren und Benennungskonventionen festlegen
description: Erfahren Sie, wie Sie eine gute Organisation in Ihrer Marketo Engage-Instanz einrichten, sodass zukünftige Marketing-Experten in Ihrem Unternehmen einfach durch die Programme navigieren, die Assets ändern und Berichte abrufen können.
role: Admin
level: Beginner
doc-type: Article
duration: 0
last-substantial-update: 2024-05-03T00:00:00Z
jira: KT-14813
thumbnail: KT-14813.jpeg
source-git-commit: 849a0022ea3a64ad964c9d2fc368b4b79b9c0cfa
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 2%

---

# Neue Instanz organisieren und Benennungskonventionen festlegen

Als Administrator, der eine neue Marketo Engage-Instanz implementiert, legen Sie die Grundlagen fest, damit zukünftige Marketing-Experten innerhalb des Unternehmens einfach durch die Instanz navigieren können. Wenn Sie sich mit der Ordnerstruktur im Baum und den Benennungskonventionen vertraut machen, bleiben Ihre Instanz aufgeräumt und für langfristigen Erfolg eingerichtet. Dieses Tutorial umfasst Beispiele, die von Adobe und Marketo Engage Champion (2019-2020), Natalie Kremer, empfohlen werden, um Ihnen zu helfen. [Ordnern organisieren und Assets konsistent benennen](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630){target="_blank"}.

## Warum sind die Strukturierung von Ordnern und die Anwendung von Benennungskonventionen erforderlich?

Wenn Sie in Ihrer Instanz organisiert bleiben, ist es für Sie und Ihre Kollegen einfach, Kampagnen, Programme und Assets zu verfolgen und die Programmleistung zu berichten. Um die Navigationsstruktur in Ihrer Instanz zu organisieren und im Maßstab zu erstellen, wird empfohlen, [Ordner](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders){target="_blank"}, [Standardbenennungskonventionen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#naming-schemes){target="_blank"}, und Funktionen wie [Klonen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#cloning){target="_blank"}.

## Organisieren einer Marketo Engage-Instanz

>[!VIDEO](https://video.tv.adobe.com/v/3421577/?quality=12&learn=on)

### Schritt 1: Einrichten einer Ordnerstruktur, um Ihre Programme in die richtige Reihenfolge zu bringen

Der erste Schritt zur Organisation Ihrer Instanz besteht darin, [Ordnerstruktur einrichten](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html) Unterbringen Sie Ihr Programm und Ihre Assets in einer leicht zu findenden und geordneten Art.

Im Folgenden finden Sie einige kurze Tipps zur Strukturierung von Ordnern in der Baumstruktur:

* Behalten Sie eine flache Ordnerstruktur für die Erkennung bei.
* Strukturieren Sie Ihre Ordner entsprechend der Teamstruktur Ihres Unternehmens (z. B. Region oder Team) oder den Initiativen (z. B. Newsletter).
* Fügen Sie zeitbasierte Beschriftungen hinzu, um die Suchbarkeit und die Signalpassung für die Archivierung zu ermöglichen (z. B. 2024).
   * Administratoren werden empfohlen, Ordner mindestens einmal jährlich zu archivieren. Mithilfe eines jährlichen Ordnernamens können Sie Smart-Live-Kampagnen einfach deaktivieren und den gesamten Ordner am Ende des Jahres archivieren.

Im Folgenden finden Sie einige Beispiele für die praktische Umsetzung dieser Tipps.

**Ordnername in Struktur**

>[!BEGINTABS]

>[!TAB Marketingaktivitäten]

![Marketing-Aktivitäten für Ordner](/help/marketo-tutorial-implementing-new-instance/assets/folders-marketing-activities.png)

>[!TAB Design Studio]

![Folder Design Studio](/help/marketo-tutorial-implementing-new-instance/assets/folders-design-studio.png)

>[!TAB Datenbank]

![Ordnerdatenbank](/help/marketo-tutorial-implementing-new-instance/assets/folders-database.png)

>[!ENDTABS]

### Schritt 2: Erstellen von Ordnern innerhalb der Programme

Wenden wir nun die Ordnerstruktur auf Programmebene an. Als Best Practice wird empfohlen, die lokalen Assets in Unterordnern zu speichern, um die Programme sauber zu halten und es internen Benutzern zu ermöglichen, die Programme effizient zu ändern oder darüber zu berichten. Zu den gängigen Unterordnern gehören E-Mails, Landingpages, Smart-Kampagnen, Listen, Berichte usw.

**Ordnername in Programmen**
* Kampagnen - *Ordner für alle Kampagnen, die Interaktionen und Status-Tracking verwalten.*
* Lokale Assets - *Ordner für alle Assets, die für dieses Programm spezifisch sind.*
   * E-Mails
   * Landingpages
   * Smart-Kampagnen
   * Listen - *Nur erforderlich, wenn programmspezifische Listen vorhanden sind.*
   * FORMS - *Nur erforderlich, wenn es programmspezifische Forms gibt; die meisten Forms sind globale Assets.*
   * Berichte - *Nur erforderlich, wenn es programmspezifische Berichte gibt.*

### Schritt 3: Erstellen von Benennungskonventionen für Ihre Programme und Assets

Sobald Sie die Ordnerstruktur in Tree haben, sollten Sie die Programme und Assets konsistent benennen. Dies ist der Fall, wenn die Standardisierung von Benennungskonventionen hilfreich wäre, den Benennungsprozess intern zu skalieren. Im Folgenden finden Sie einige Komponenten, mit denen Sie eine Benennungskonvention zur Gewährleistung der Suchbarkeit einrichten können:

* Abkürzung für Programmtyp - E-Mail, Inhalt, Struktur, Webinar etc.
* Kategorie - Programmtyp - Eigenständige E-Mail, Newsletter usw.
* Datum - Startdatum des Programms
* Kurze Beschreibung - Kurze Beschreibung des Programms

Lassen Sie uns nun die Werte in die Formel aufnehmen und die Programmnamen für verschiedene Programmtypen generieren.

#### Formel zur Programmbenennung

| **Abkürzung des Programmtyps** | **YYYY** | **\-** | **MM** | **\-** | **DD(Optional)** | **Kategorie** | **\-** | **Kurze Beschreibung des Programms** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| EM - E-Mail-Versand (Email Program) | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| NL - Newsletter | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| ENG - Interaktionsprogramm | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| WBN - Webinar | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| IW - Interaktives Webinar | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| TS - Tradeshow | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| LE - Live-Ereignis (Roadshow) | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| UG - Benutzergruppe | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| WC - Website-Inhalt | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| CS - Inhaltssynchronisierung | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| LI - Listenimport | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| OA - Online-Werbung | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |
| PPC - Pay-per-Click | YYYY | \- | MM | \- | DD(Optional) | Kategorie | \- | Kurze Beschreibung des Programms |

| **Beispiele** |
| --- |
| Gated Content ES 2023-10 - XYX Whitepaper |
| WC-2023-10- Monatliches Webinar - ABC-Fallstudie |

#### Asset-Benennungsformel

Wenn Sie eine Ebene weiter gehen und Assets benennen, sollten Sie den Programmnamen nicht wiederholen und kurze und allgemeine IDs für die zukünftige Verwendung des Klonens verwenden. Im Folgenden finden Sie einige kurze Hinweise, die Sie beachten sollten:

* Die Assets werden basierend auf ihrer Sequenz im Programmprozess nummeriert.
* Verwenden Sie &quot;-&quot; (Bindestrich), um die Benennungskomponenten anstelle von &quot;.&quot;(Punkt) oder &quot;\_&quot;(Unterstrich).
   * Warum? Marketo Engage verwendet einen Punkt, um den Programmnamen vom Kampagnennamen zu trennen. Die Verwendung von &quot;\_&quot;verhindert, dass Sie es sehen, wenn das Asset per Hyperlink verknüpft ist.
* Verwenden Sie Standardabkürzungen in den Asset-Namen, um die Referenz zu verkürzen und dennoch eine einfache Erkennung zu ermöglichen.

In diesem Zusammenhang wenden wir diese Tipps auf die folgenden Assets an und erstellen Formeln zum Generieren von Namen:

##### Benennen Sie die Assets basierend auf der Sequenz im Programmprozess.

| **Sequenz im Programmprozess** | **\-** | **Beschreibung** |
| --- | --- | --- |
| 01 | \- | Beschreibung |
| 02 | \- | Beschreibung |
| 03 | \- | Beschreibung |

| **Beispiele: Smart-Liste** |
| --- |
| 01-E-Mail senden |
| 02-Geöffnet |
| 03-Angeklickt |
| 04-Ausgefülltes Formular |
| 05-Beeinflusst (Programmerfolg) |
| 06-Abgemeldet |

##### Benennen Sie die Assets mit einer Abkürzung des Asset-Typs.

| **Abkürzung des Asset-Typs** | **Asset-Typ** | **\-** | **Beschreibung des Ziels** |
| --- | --- | --- | --- |
| LP - Landingpage | LP | \- | Beschreibung des Ziels |
| E-MAIL - E-Mail (ausgehend) | E-MAIL | \- | Beschreibung des Ziels |
| WARNUNG - E-Mail-Warnhinweis | WARNUNG | \- | Beschreibung des Ziels |
| WF - Webformular | WF | \- | Beschreibung des Ziels |
| EXCL - Ausschlussliste | EXCL | \- | Beschreibung des Ziels |
| SLST - Smart List | SLST | \- | Beschreibung des Ziels |
| LST - Statische Liste | LST | \- | Beschreibung des Ziels |

| **Beispiele** |
| --- |
| LP-Registrierung |
| LP-Vielen Dank |
| E-MAIL-Outbound |
| EMAIL-Newsletter |
| E-MAIL-Einladung |
| EMAIL-Reminder |
| EXCL-Wettbewerber |

##### Benennen Sie die herunterladbaren Dateien (.pdf) mit der Abkürzung des Asset-Typs.

| **Asset-Typ** | **Inhaltsbeschreibung** | **\-** | **Abkürzung des Asset-Typs** | **.** | **PDF** |
| --- | --- | --- | --- | --- | --- |
| WP - Weißbuch | Inhaltsbeschreibung | \- | WP | . | pdf |
| CS - Fallstudie | Inhaltsbeschreibung | \- | CS | . | pdf |
| DS - Datenblatt | Inhaltsbeschreibung | \- | DS | . | pdf |

| **Beispiele: herunterladbare PDF-Dateien** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

>[!CAUTION]
>
>Verwenden Sie beim Benennen von Dateien in den oben genannten Beispielen keine Leerzeichen und vermeiden Sie die Verwendung von Unterstrichen &quot;\_&quot;.

## Wie geht es weiter?

* Laden Sie das Arbeitsblatt herunter: [Marketo Engage-Organisations- und Namenskonventionen](./assets/adobe-marketo-engage-organization-and-naming-conventions.xlsx){target="_blank"} , um die Erstellung der Ordnerstruktur und Benennungskonventionen zu unterstützen.
* Sobald Sie die erforderlichen Komponenten in Ihrer standardmäßigen Namenskonvention festgelegt haben, sollten Sie in Erwägung ziehen, Formeln in einem Google Tabellenblatt oder Microsoft Excel zu erstellen. Geben Sie einfach Ihre Werte in die Tabelle ein, um Ihre Programmnamen zu generieren.
* Wenn Sie sich an einer allgemeinen Ordnerstruktur orientieren, ist es an der Zeit, anhand der häufigsten Anwendungsfälle und der häufigsten Anforderungen, die Ihr Team erhält, die benötigten Vorlagen zu durchdenken. Erstellen Sie dann Ihre erste Programmvorlage. Lesen Sie für die ersten Schritte mit [Adobe Marketo Engage-Programmvorlagen](https://business.adobe.com/blog/how-to/get-started-with-marketo-engage-program-templates){target="_blank"}.

### Autoren

{{natalie-kremer}}

{{amy-chiu}}