---
title: Erstellen eines Datenflussdiagramms, um den technischen Marketing-Stack zu verstehen
description: Erfahren Sie, wie Sie ein Diagramm mit „Lead- und Datenquellen“ erstellen, um das Datenuniversum zu verstehen, die Instanz effizient zu überprüfen und zu bereinigen.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13877
thumbnail: KT-13877.jpeg
hide: false
exl-id: 088bdcf1-4e49-44a7-ac78-a03742ff680b
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 2%

---

# Erstellen eines Datenflussdiagramms, um den technischen Stapel Ihres Marketing zu verstehen

Als Administrator, der eine [!DNL Marketo Engage] Instanz übernimmt, die seit Jahren live ist, ist es wie eine Mission unmöglich, die Instanz effizient zu überprüfen und aufzuräumen. Als [!DNL Adobe] [!DNL Marketo Champion] (2019), Kelly Jo Horton, in eine alteingesessene Instanz trat, nahm sie diese Herausforderung an, indem sie [ein Diagramm von „Lead und Datenquellen“ erstellte](https://nation.marketo.com/t5/employee-blogs/understand-your-marketing-technology-and-data-create-this/ba-p/296774){target="_blank"} um sich mit dem Datenuniversum vertraut zu machen. In diesem Tutorial erfahren Sie, wie Sie Ihr eigenes Datenflussdiagramm erstellen, indem Sie auf den Beispielen von Kelly Jo Horton aufbauen. Lernen wir Ihr MarTech-Ökosystem kennen!

## Warum sollten Sie ein Architekturdiagramm für Ihre geerbte Instanz erstellen?

1. **Machen Sie sich mit dem Marketing-Technologie-Stack vertraut, den Sie von einer Live-Instanz geerbt haben.** Alle Marketing-Vorgangs-Manager/Platform-Vorgangs-Manager werden ermutigt, diese Übung durchzuführen, wenn sie bei einem neuen Unternehmen beginnen. Dieser Erstellungsprozess ermöglicht es Admin-Benutzern, sich einen Überblick über die Daten und Aktivitäten zu verschaffen, die von externen Integrationen an [!DNL Marketo Engage] gesendet werden, und API-Fehler einfach zu beheben.
2. **Machen Sie sich mit den wichtigsten Stakeholdern vertraut, die die externen Integrationen verwalten.** Ein Tipp, den Kelly Jo Horton verwendet, um die Stakeholder schnell zu identifizieren, besteht darin, auf die Liste der API-Benutzer zu verweisen.
   1. **Navigieren Sie im Abschnitt „Admin“ zur Registerkarte „Integration>LaunchPoint“.** Erfahren Sie mehr darüber, wie Sie zur Registerkarte „LaunchPoint“ navigieren: [Erstellen eines benutzerdefinierten Services zur Verwendung mit der REST-API](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.html?lang=de){target="_blank"}.
   2. Auf der Registerkarte Integration > Web-Services im Abschnitt API-Aufrufinformationen können Sie API-Nutzungsstatistiken nach API-Benutzer finden. Durch Klicken auf die API-Aufrufnummer können Sie die spezifischen individuellen Aufrufe der einzelnen Benutzenden anzeigen.

## Wie Sie diese visuelle Datenflussdiagramm-Übung durchführen

### Schritt 1: Diagramm des aktuellen Status

Erstellen Sie ein Diagramm zum aktuellen Status. Siehe folgendes Beispiel:

![Aktuelles Zustandsdiagramm](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Current_State_Lead_Data_Sources_KellyJo_Horton.png){align="center"}


### Schritt 2: Zukünftiges Zustandsdiagramm

Erstellen Sie ein Zukunftsstatus-Diagramm, das bei der Präsentation der Technologie- und System-Roadmap für nicht-technische Stakeholder verwendet werden kann. Siehe folgendes Beispiel:

![Zukunftszustandsdiagramm](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Future-State-Lead-Data-Sources-KellyJo-Horton.png){align="center"}

### Schritt 3: Technische Version

Erstellen Sie eine technische Version, die Details wie den API-Benutzernamen für jede Integration, eine kurze Beschreibung des Datentyps, der an [!DNL Marketo Engage] gepusht oder aus [!DNL Marketo Engage] abgerufen wird, und ein detailliertes Diagramm aller Middleware-Flüsse und -Trigger anzeigt.  Siehe folgendes Beispiel:

![Technische Version](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Lead-Data-Source-Diagram-KellyJo-Horton.png){align="center"}


## Wie geht es weiter?

**Erste Schritte mit Beispielen:**
Laden Sie eines der Beispieldatenflussdiagramme herunter, um den aktuellen Status Ihres Marketing-Technologie-Stacks, Ihrer Person und Ihres Datenflusses zuzuordnen, oder erstellen Sie ein neues Diagramm für Ihr Datenuniversum, während Sie die Instanz überprüfen:


<table style="table-layout:fixed">
   <tr>  
      <td style="border: 0;">
      <div style="text-align: center;">
          <a href="./_assets/downloads/Current_Future_State_Lead_Data_Sources.zip">
            <strong>Aktueller und künftiger Status</strong>
         </a>
      </div>
      </td>
      <td style="border: 0;">
      <div style="text-align: center;">
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <strong>Detaillierte Ebenen nach Funktionskategorie </strong>   
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Lead_Data_Source.zip">
           <strong>Lead- und Daten-Source-Fluss-</strong>  
         </a>
         </div>
       </td> 
       <td style="border: 0;">
         <div style="text-align: center;">
         <a href="./_assets/downloads/Simple_World_Class_Stage_Stack.zip">
          <strong>Vereinfachtes Diagramm</strong>  
         </a>
         </div>
        </td>  
   </tr>
   <tr>
    <td style="border: 0;">
         <div>
          <img alt="Diagramm des aktuellen Status und des zukünftigen Status" src="./_assets/Thumbnail_Current-Future State Lead_Data Sources_KellyJo_Horton.png"/>
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div>
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <img alt="Detaillierte Ebenen nach funktionalen Kategorien" src="./_assets/Thumbnail_Detailed_Layers_by_Functional_Category_Stacked_Technologies_KellyJo_Horton.png" />
       </a>
         </div>
      </td>
       <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Lead_Data_Source.zip">
         <img alt="Flussdiagramm für Lead und Daten in Source" src="./_assets/Thumbnail_Lead-Data Source Diagram_KellyJo_Horton.png" />
         </a>
         </div>
      </td>
     <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Simple_World_Class_Stage_Stack.zip">
             <img alt="Vereinfachtes Diagramm" src="./_assets/Thumbnail_Simple_World_Class_Stage_Stack.png" />
         </a>
         </div>
      </td>
</table>

Dies sind einige Tools, die Sie verwenden können: draw.io (Google Docs), [!DNL Adobe] XD, Figma, Gliffy (in Confluence)

**Was ist, wenn es bereits Architekturdiagramme gibt?** neue Teammitglieder können unterschiedliche Perspektiven haben. Es ist sinnvoll, diese Übung von neuen [!DNL Marketo Engage]-Administratoren im Rahmen ihres Onboarding-Prozesses durchführen zu lassen und mit anderen zu teilen.

## Autoren

**Kelly Jo Horton**\
[!DNL Adobe] Marketo Champion (2019)
*Senior Client Partner bei Etumos*

![Kelly Jo Horton](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Kelly_Jo_Horton.png){width="30%"}

**Amy Chiu**
*Adoption &amp; Retention Marketing Manager,[!DNL Adobe]*

(/help/marketo-tutorial-inherited-instance/_assets/authors/[!DNL Adobe]_author_Amy_Chiu.png){width=30%}
