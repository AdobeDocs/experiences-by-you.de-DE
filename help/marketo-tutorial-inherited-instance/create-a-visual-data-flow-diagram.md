---
title: Erstellen Sie ein visuelles Datenflussdiagramm, um Ihren Marketing-Tech-Stack zu verstehen.
description: Erfahren Sie, wie Sie ein Diagramm mit "Lead- und Datenquellen"erstellen, um die Datenschicht zu verstehen, die Instanz effizient zu prüfen und zu bereinigen.
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
source-git-commit: b2e05ff39e065691dda530ed17762a55cf2e6778
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 2%

---

# Erstellen Sie ein visuelles Datenflussdiagramm, um Ihren Marketing-Tech-Stack zu verstehen.

Als Administrator, der eine [!DNL Marketo Engage] -Instanz, die seit Jahren live ist, ist es wie eine Mission, die unmöglich ist, die Instanz effizient zu überprüfen und zu bereinigen. Wann [!DNL Adobe] [!DNL Marketo Champion] (2019), Kelly Jo Horton, trat in eine seit langem etablierte Instanz ein und nahm diese Herausforderung an, indem sie [Erstellen eines Diagramms &quot;Lead- und Datenquellen&quot;](https://nation.marketo.com/t5/employee-blogs/understand-your-marketing-technology-and-data-create-this/ba-p/296774){target="_blank"} sich mit dem Datenuniversum vertraut zu machen. In diesem Tutorial erfahren Sie, wie Sie Ihr eigenes Datenflussdiagramm erstellen, indem Sie auf den von Kelly Jo Horton freigegebenen Beispielen aufbauen. Lernen Sie Ihr MarTech-Ökosystem kennen!

## Warum erstellen Sie ein Architekturdiagramm für Ihre geerbte Instanz?

1. **Machen Sie sich mit dem Marketing-Tech-Stack vertraut, den Sie von einer Live-Instanz übernommen haben.** Alle Marketing Operation Manager/Platform Operations Manager werden aufgefordert, diese Übung bei der Gründung eines neuen Unternehmens durchzuführen. Dieser Erstellungsprozess ermöglicht es Admin-Benutzern, das vollständige Bild der Daten und Aktivitäten anzuzeigen, die von externen Integrationen an gesendet werden. [!DNL Marketo Engage] und zur einfachen Fehlerbehebung bei API-Fehlern.
2. **Machen Sie sich mit den wichtigsten Stakeholdern vertraut, die die externen Integrationen verwalten.** Ein Tipp, den Kelly Jo Horton nutzt, um die Interessengruppen schnell zu identifizieren, ist, auf die Liste der API-Benutzer zu verweisen.
   1. **Navigieren Sie im Abschnitt &quot;Admin&quot;zur Registerkarte &quot;Integration > LaunchPoint&quot;.** Erfahren Sie mehr darüber, wie Sie zur Registerkarte &quot;LaunchPoint&quot;navigieren: [Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der REST-API](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.html){target="_blank"}.
   2. Statistiken zur API-Nutzung nach API-Benutzern finden Sie auf der Registerkarte Integration > Web-Services im Abschnitt API-Aufrufinformationen . Durch Klicken auf die API-Rufnummer können Sie die spezifischen individuellen Aufrufe der einzelnen Benutzer anzeigen.

## Anleitung zu dieser visuellen Datenflussdiagrammübung

### Schritt 1: Aktuelles Statusdiagramm

Erstellen Sie ein Diagramm zum aktuellen Status. Siehe folgendes Beispiel:

![Aktuelles Statusdiagramm](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Current_State_Lead_Data_Sources_KellyJo_Horton.png){align="center"}


### Schritt 2: Zukünftiges Statusdiagramm

Erstellen Sie ein Diagramm &quot;Zukünftiger Status&quot;, das bei der Präsentation des technischen und systembezogenen Fahrplans für nicht technische Akteure verwendet werden kann. Siehe folgendes Beispiel:

![Zukünftiges Statusdiagramm](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Future-State-Lead-Data-Sources-KellyJo-Horton.png){align="center"}

### Schritt 3: Technische Version

Erstellen Sie eine technische Version mit Details wie dem API-Benutzernamen für jede Integration und einer kurzen Beschreibung des Datentyps, an den gesendet wird. [!DNL Marketo Engage] oder von [!DNL Marketo Engage]und ein detailliertes Diagramm aller Middleware-Flüsse und -Trigger.  Siehe folgendes Beispiel:

![Technische Version](/help/marketo-tutorial-inherited-instance/_assets/data-flow-diagram/Lead-Data-Source-Diagram-KellyJo-Horton.png){align="center"}


## Wie geht es weiter?

**Erste Schritte mit Beispielen:**
Laden Sie eines der Musterdatenflussdiagramme herunter, um den aktuellen Status Ihres Marketing-Technologie-Stapels, Ihrer Person und Ihres Datenflusses abzubilden, oder erstellen Sie ein Diagramm für Ihre Datenwelt von Grund auf, während Sie die Instanz prüfen:


<table style="table-layout:fixed">
   <tr>  
      <td style="border: 0;">
      <div style="text-align: center;">
          <a href="./_assets/downloads/Current_Future_State_Lead_Data_Sources.zip">
            <strong>Aktueller Staat und zukünftiger Staat</strong>
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
           <strong>Lead- und Datenquellenfluss </strong>  
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
          <img alt="Aktuelles Status- und zukünftiges Statusdiagramm" src="./_assets/Thumbnail_Current-Future State Lead_Data Sources_KellyJo_Horton.png"/>
         </a>
      </div>
      </td>
      <td style="border: 0;">
         <div>
         <a href="./_assets/downloads/Detailed_Layers_by_Functional_Category_Stacked_Technologies.zip">
         <img alt="Detaillierte Ebenen nach Funktionskategoriendiagramm" src="./_assets/Thumbnail_Detailed_Layers_by_Functional_Category_Stacked_Technologies_KellyJo_Horton.png" />
       </a>
         </div>
      </td>
       <td style="border: 0;">
         <div>
            <a href="./_assets/downloads/Lead_Data_Source.zip">
         <img alt="Lead- und Datenquellenflussdiagramm" src="./_assets/Thumbnail_Lead-Data Source Diagram_KellyJo_Horton.png" />
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

Dies sind einige Tools, die Sie verwenden können: draw.io (Google Docs), [!DNL Adobe] XD, Figma, Gliffy (in Verbindung)

**Was ist, wenn es bereits Architekturdiagramme gibt?** Neue Teammitglieder könnten unterschiedliche Perspektiven haben. Neue [!DNL Marketo Engage] Administratoren führen diese Übung im Rahmen ihres Onboarding-Prozesses durch und teilen sie mit anderen.

## Autoren

**Kelly Jo Horton**\
[!DNL Adobe] Marketo Champion (2019)
*Senior Client Partner bei Etumos*

![Kelly Jo Horton](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Kelly_Jo_Horton.png){width="30%"}

**Amy Chiu**
*Adoption &amp; Retention Marketing Manager,[!DNL Adobe]*

(/help/marketo-tutorial-inherited-instance/_assets/authors/[!DNL Adobe]_author_amy_chiu.png){width=30%}
