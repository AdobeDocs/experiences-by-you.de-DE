---
title: Erstellen standardisierter Code-Vorlagen
description: Für eine Basisimplementierung (d. h. für das, was Ihr Unternehmen als unerlässliche KPIs für alle  [!DNL Adobe Analytics]  betrachtet) sollte Ihre Organisation nach Möglichkeit eine einzige Implementierungsmethode verwenden.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10532.jpg
kt: 10532
exl-id: edd3df73-6d1a-4a26-a984-810cc7dd382f
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Erstellen standardisierter Code-Vorlagen

**WAS:** Für eine „Basisimplementierung“ (d. h. für das, was Ihr Unternehmen als unerlässliche KPIs für alle [!DNL Adobe Analytics] Sites betrachtet) sollte Ihre Organisation nach Möglichkeit eine einzige Implementierungsmethode verwenden. Verwenden Sie beispielsweise dieselbe Site-übergreifende Datenschichtstruktur und nutzen Sie dieselbe Tag-Manager-Regel/denselben benutzerdefinierten Code, um Dinge wie interne Suchen oder Besucherprofilinformationen zu erfassen.

**WARUM:** Eine wiederholbare und skalierbare Basisimplementierung macht das Hinzufügen neuer Elemente oder neuer Websites/Programme zu einem rationellen, wenig aufwändigen Unterfangen und sorgt gleichzeitig für eine saubere Implementierung und einfache Fehlerbehebung. Die Verwendung einer einheitlichen Methode erleichtert es auch neuen Admins/Entwicklern, online zu gehen und zu verstehen, wormit sie arbeiten.

**WIE:** Verwenden Sie eine einzige Formatvorlage, die an Entwickler*innen übergeben werden kann, wenn eine neue Site- oder Tagging-Verbesserung online geht. In der Regel funktioniert ein Word-Dokument gut, wenn Sie die folgenden Elemente umreißen können:

* Variablen, die implementiert werden, sowie deren Zweck und Zeitpunkt der Festlegung. z. B.:

| AA-Variable | Beschreibung | Wann/wo sie festgelegt wird | Festlegen |
|--- |--- |--- |--- |
| EVAR8 | Interne Suchbegriffe | Auf der Landingpage der internen Suchergebnisse | Datenschicht |
| event8 | Anzahl der internen Suchvorgänge | Auf der Landingpage der internen Suchergebnisse | Startregel |

* Details zum Festlegen. Hier geben Sie die erforderlichen Datenschichtobjekte und deren Syntax sowie die zu konfigurierenden TMS-Regeln und die Details der Regeleinrichtung an.
* Testfälle, um sicherzustellen, dass sie in der Qualitätssicherung behandelt werden, und alle Variablen, die Sie in einem erfolgreichen Testfall erwarten. Beschreiben Sie, was eine erfolgreiche Implementierung beinhalten sollte, wenn der Entwickler diese Verbesserung testet.

Idealerweise muss dieses Dokument nur für die nächste Site optimiert werden, auf der Sie die Grundlagen wie Eigenschaftsname, Seitenbenennungskonvention usw. aktualisieren. Sie müssen das Rad nicht jedes Mal neu erfinden und Sie können mehr Zeit sparen.

## Autoren

Dieses Dokument wurde gemeinsam verfasst von:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Platform Manager bei NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, Senior Consultant bei [!DNL Adobe]
