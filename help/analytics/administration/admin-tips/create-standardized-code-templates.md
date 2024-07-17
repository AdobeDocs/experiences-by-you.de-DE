---
title: Erstellen standardisierter Codevorlagen
description: Für eine Basisimplementierung (d. h. was Ihr Unternehmen als die Muss-aufweist KPIs für alle [!DNL Adobe Analytics] Sites betrachtet) sollte Ihre Organisation nach Möglichkeit über eine einzige Implementierungsmethode verfügen.
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

# Erstellen standardisierter Codevorlagen

**WAS:** Für eine &quot;Grundlinien&quot;-Implementierung (d. h. was Ihr Unternehmen als die erforderlichen KPIs für alle [!DNL Adobe Analytics]-Sites betrachtet) sollte Ihre Organisation nach Möglichkeit über eine einzige Implementierungsmethode verfügen. Verwenden Sie beispielsweise die gleiche Site-übergreifende Datenschichtstruktur und nutzen Sie dieselbe Tag-Manager-Regel/denselben benutzerdefinierten Code, um Dinge wie interne Suchen oder Besucherprofilinformationen zu erfassen.

**WARUM:** Eine wiederholbare und skalierbare Basisimplementierung macht das Hinzufügen neuer Elemente oder neuer Sites/Apps zu einem optimierten, minimalen Aufwand und sorgt gleichzeitig dafür, dass Ihre Implementierung sauber und einfach zu beheben ist. Die Verwendung einer einheitlichen Methode erleichtert es auch neuen Administratoren/Entwicklern, online zu gehen und zu verstehen, wormit sie arbeiten.

**HOW:** Verwenden Sie eine Vorlage im Einzelformat, die an Entwickler übergeben wird, wenn eine neue Site- oder Tagging-Verbesserung online geht. Normalerweise funktioniert ein Word-Dokument gut, wenn Sie die folgenden Elemente umreißen können:

* Variablen, die implementiert werden, deren Zweck und Zeitpunkt der Festlegung. Beispiel:

| AA-Variable | Beschreibung | Wann/Wo wird festgelegt? | Festlegen |
|--- |--- |--- |--- |
| eVar8 | Interne Suchkeywords | Auf der Landingpage der internen Suchergebnisse | Datenschicht |
| event8 | Anzahl der internen Suchen | Auf der Landingpage der internen Suchergebnisse | Launch-Regel |

* Details zum Festlegen. Hier geben Sie die erforderlichen Datenschichtobjekte und deren Syntax sowie die zu konfigurierenden TMS-Regeln und die Details der Regeleinrichtung an.
* Testfälle, um sicherzustellen, dass sie in der Qualitätssicherung behandelt werden, sowie alle Variablen, die Sie in einem erfolgreichen Testfall erwarten. Erläutern Sie, was eine erfolgreiche Implementierung enthalten sollte, wenn der Entwickler diese Verbesserung testet.

Idealerweise muss dieses Dokument nur für die nächste Site optimiert werden, auf der Sie die Grundlagen wie Eigenschaftsname, Seitenbenennungskonvention usw. aktualisieren. Es ist nicht erforderlich, das Rad jedes Mal neu zu erfinden, und Sie können mehr Zeit sparen.

## Autoren

Dieses Dokument wurde von folgenden Personen mitgeschrieben:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Platform Manager bei NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, leitender Berater bei [!DNL Adobe]
