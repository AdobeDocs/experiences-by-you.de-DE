---
title: Erstellen standardisierter Benennungskonventionen
description: Standardisierte Namenskonventionen gelten sowohl für den Variablennamen selbst, wenn er in der Admin-Benutzeroberfläche aktiviert ist, als auch für die Werte, die an die Dimension übergeben werden.
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10531.jpg
kt: 10531
exl-id: 79cec21e-2b52-4e7b-88ad-db137a8cef4e
source-git-commit: c568ed0a06551d910b6f533698ec47c15adecf6c
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Erstellen standardisierter Benennungskonventionen

**WAS:** Die standardisierten Benennungskonventionen gelten sowohl für den Variablennamen selbst, wenn sie in der Administrator-Benutzeroberfläche von [!DNL Adobe Analytics] (AA) aktiviert sind, als auch für die Werte, die an die Dimension übergeben werden. (d. h. Seitennamen wären &quot;Seitenname (v1)&quot;als Variablenname und die übergebenen Seitennamenwerte sollten einheitlich sein und einer bestimmten Struktur/Hierarchie wie &quot;sitename|homepage&quot;oder &quot;sitename|search|searchresults&quot; folgen).

**WARUM:** Namenskonventionen eignen sich hervorragend, um alles einheitlich zu halten und die Benutzeroberfläche für Ihre Benutzer leicht zu verstehen. Wenn Sie diese von Anfang an erstellen und in der Plattform und im Code durchsetzen, ist die Skalierung einfacher.

**HOW:** Die Benutzeroberfläche und das Tagging-Dokument sollten sowohl für &quot;Name&quot;als auch für &quot;Beschreibung&quot;übereinstimmen. Dies verhindert, dass Ihre Benutzer ein Excel-Dokument abrufen müssen, damit sie Ihre Daten direkt in der Benutzeroberfläche verstehen können. Es wird außerdem empfohlen, alles Kleinbuchstaben für Konsistenz zu verwenden.

Es ist immer am besten, die Seitennamen auch auf der gesamten Plattform (oder den Bildschirmnamen für Apps) konsistent zu halten. Sie können beispielsweise &quot;`property:section:sub section:sub sub section:unique page name`&quot; in eine Variable/Dimension setzen. Wenn alle diese Felder separate Felder in Ihrer Datenschicht sind, können Sie den Seitennamen sogar direkt in Ihrer JS-Datei/in Launch erstellen. Die Festlegung aller Elemente in ihren eigenen Dimensionen kann Ihnen dabei helfen, bestimmte Eigenschaften oder Bereiche Ihrer Site/App einfacher aufzuschlüsseln und Traffic und Flüsse besser zu verstehen.

Alles, was es Benutzern erleichtert, die Daten zu finden und zu verstehen, einschließlich so einfacher Namenskonventionen, erhöht die Verwendung von [!DNL Adobe Analytics] und liefert bessere Einblicke für das Unternehmen.

## Autoren

Dieses Dokument wurde von folgenden Personen mitgeschrieben:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Platform Manager bei NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, leitender Berater bei [!DNL Adobe]
