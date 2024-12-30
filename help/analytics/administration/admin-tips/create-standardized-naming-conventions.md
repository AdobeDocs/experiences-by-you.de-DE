---
title: Erstellen standardisierter Benennungskonventionen
description: Es gelten standardisierte Benennungskonventionen sowohl für den Variablennamen selbst, wenn er in der Admin-Benutzeroberfläche von AA aktiviert ist, als auch für die Werte, die an die Dimension übergeben werden.
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

**WAS:** Es gelten standardisierte Benennungskonventionen sowohl für den Variablennamen selbst, wenn er in der Admin-Benutzeroberfläche von [!DNL Adobe Analytics] (AA) aktiviert ist, als auch für die Werte, die an die Dimension übergeben werden. (d. h. Seitennamen wären „Seitenname (v1)“ als Variablenname, und die übergebenen Seitennamenwerte sollten einheitlich sein und einer bestimmten Struktur/Hierarchie folgen, z. B. „Seitenname|Homepage“ oder „Seitenname|Suche|Suchergebnisse„).

**WARUM:** Namenskonventionen sind eine gute Möglichkeit, alles einheitlich zu halten und die Benutzeroberfläche für Ihre Benutzer*innen leicht verständlich zu gestalten. Wenn Sie diese von Anfang an erstellen und in der Plattform und im Code durchsetzen, wird die Skalierung einfacher.

**WIE:** Die Schnittstelle und das Tagging-Dokument sollten sowohl für „Name“ als auch für „Beschreibung“ übereinstimmen. Dies erspart Ihren Benutzern das Aufrufen eines Excel-Dokuments und ermöglicht es ihnen, Ihre Daten direkt in der Schnittstelle zu verstehen. Aus Gründen der Konsistenz wird außerdem empfohlen, alles klein zu schreiben.

Es ist immer am besten, auch die Seitennamen (oder Bildschirmnamen für Apps) über die gesamte Plattform hinweg konsistent zu halten. Sie können beispielsweise &quot;`property:section:sub section:sub sub section:unique page name`&quot; in eine Variable/Dimension einfügen. Wenn alle diese Felder separate Felder in Ihrer Datenschicht sind, können Sie den Seitennamen sogar direkt in Ihrer JS-Datei/in Launch erstellen. Wenn alle diese Elemente auch in ihren eigenen Dimensionen festgelegt sind, können Sie bestimmte Eigenschaften oder Bereiche Ihrer Site/App einfacher aufschlüsseln und Traffic und Flüsse besser verstehen.

Alles, was es den Benutzenden erleichtert, die Daten zu finden und zu verstehen, einschließlich so einfacher Dinge wie Namenskonventionen, erhöht die Nutzung von [!DNL Adobe Analytics] und liefert bessere Einblicke für das Unternehmen.

## Autoren

Dieses Dokument wurde gemeinsam verfasst von:

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon, Digital [!DNL Analytics] Platform Manager bei NortonLifeLock
[!DNL Adobe Analytics] Champion

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

Rachel Fenwick, Senior Consultant bei [!DNL Adobe]
