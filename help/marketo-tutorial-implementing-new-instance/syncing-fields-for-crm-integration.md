---
title: Synchronisieren von Feldern für die nativen CRM-Connectoren
description: Erfahren Sie, wie Sie Ihre anfängliche CRM-Integration optimieren können, indem Sie die wesentlichen CRM-Felder für das Marketo Engage strategisch auswählen. Führen Sie die Übung zum Datenwörterbuch durch, um die Felder zu identifizieren, die Sie für eine reibungslose CRM-Synchronisierung benötigen, die den Vertriebs- und Marketing-Teams hilft, miteinander in Einklang zu bleiben.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14811
thumbnail: KT-14811.jpeg
exl-id: 42b7ca3d-e445-4c11-ad3d-d4e70c101c8e
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1567'
ht-degree: 0%

---

# Synchronisieren von Feldern für die nativen CRM-Connectoren

Verwenden Sie Salesforce oder Microsoft Dynamics in Ihrem Unternehmen? Wenn dies der Fall ist, können Sie mit nativen CRM-Connectoren von Marketo Engage (d. h. Salesforce, Microsoft Dynamics und Veeva) Marketing- und Vertriebsaktivitäten koordinieren, indem Sie relevante Informationen zwischen Marketo Engage und CRM nahtlos austauschen. Bevor Sie die anfängliche CRM-Synchronisierung konfigurieren, stellen Sie sicher, dass Sie die Felder identifizieren, die Sie zwischen den beiden Systemen synchronisieren möchten, um Ihre Marketo Engage-Datenbank sauber zu halten.

Erfahren Sie mehr darüber, wie Sie diese Übung mit den von Adobe Professional Services vorgeschlagenen Best Practices durchführen. Folgen Sie diesen Schritten, um Standardfelder und benutzerdefinierte Felder zu verstehen und ihre Beziehungen zwischen Marketo Engage und Ihrem CRM zu dokumentieren.

## Identifizieren Sie zu synchronisierende Felder, bevor Sie Ihr CRM mit Marketo Engage integrieren.

Bei der Integration Ihres CRM mit Marketo Engage müssen Sie wahrscheinlich nicht alle Ihre CRM-Felder mit Marketo Engage synchronisieren. Wenn Sie die erforderlichen Felder strategisch betrachten, kann Ihre Marketo Engage-Instanz den Datenfluss effizienter verarbeiten.

Die anfängliche Synchronisation zwischen Ihrem Marketo Engage- und CRM-System erstellt automatisch Verknüpfungen für die meisten bestehenden Standardfelder (z. B. E-Mail, Vor-/Nachname, Firma usw.). Darüber hinaus synchronisiert der Connector auch [Benutzerdefinierte Felder](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} für Ihre Leads, Kontakte, Konten und Opportunities, indem er neue Felder in Marketo Engage erstellt, die automatisch diesen Feldern aus Ihrem CRM zugeordnet werden.

Die Identifizierung und Organisation der Felder, die Sie vor der ersten Synchronisierung mit Ihrem CRM synchronisieren möchten, ist ein wichtiger Schritt im Setup-Prozess des nativen Connectors. Wir bezeichnen dies als Datenwörterbuch-Übung, mit der Sie die Anzahl der doppelten Felder, die erstellt werden, minimieren und nachfolgende Zuordnungsschritte so reibungslos wie möglich durchführen können. Für diese Übung sind in der Regel Eingaben der Marketing- und Vertriebsteams sowie Ihres CRM-Administrators erforderlich, um sicherzustellen, dass nur relevante Felder mit Ihrer Marketo Engage-Instanz synchronisiert werden.

## Datenwörterbuch erstellen

Im Allgemeinen empfiehlt es sich, nur CRM-Felder zu synchronisieren, die für Marketing-Zwecke erforderlich sind. Beginnen Sie mit dieser Übung, um die Felder aus Ihrem CRM zu organisieren, die dem Marketo Engage zugeordnet werden müssen, und führen Sie die anfängliche CRM-Synchronisierung beim ersten Mal korrekt aus.

>[!NOTE]
>Wenn Sie in Ihrem CRM benutzerdefinierte Felder haben, die vor Beginn der ersten Synchronisierung bereits über ein entsprechendes benutzerdefiniertes Feld im Marketo Engage verfügen, wird für das CRM-Feld ein neues „Duplikat“ im Marketo Engage erstellt. Sie können das CRM-Feld dem ursprünglichen Marketo Engage-Feld neu zuordnen und das doppelte Feld ausblenden, sobald die erste Synchronisierung abgeschlossen ist. Dazu müssen Sie sich jedoch an den [Adobe-](https://experienceleague.adobe.com/de/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"} wenden. Siehe Schritt 7 für weitere Details.

**Schritt 1:** Erstellen Sie eine grobe Liste der derzeit in Ihrem CRM verfügbaren Felder und markieren Sie, ob sie auf Marketo Engage erscheinen sollen.

* Nehmen Sie Feedback von Ihren CRM-Admin-, Marketing- und Vertriebs-Teams in den Entscheidungsprozess auf.
* Dokumentieren Sie die API-Namen und Feldtypen für jedes Feld
* Legen Sie fest, welche Zugriffsebene Marketo Engage für diese Felder haben soll (d. h. schreibgeschützt oder mit Lese-/Schreibzugriff)


**Schritt 2:** Überprüfen Sie den Abschnitt [Admin > Feldverwaltung](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} Ihrer Marketo Engage-Instanz, um alle zuvor direkt im System erstellten benutzerdefinierten Felder zu identifizieren, die Sie in die Synchronisierung einbeziehen möchten.

* Dokumentieren Sie die API-Namen und Feldtypen für jedes Feld.
* Felder kennzeichnen, die bereits über ein entsprechendes Feld in Ihrem CRM verfügen.
* Felder kennzeichnen, die noch kein entsprechendes Feld in Ihrem CRM haben.


**Schritt 3:** Sie mit dem Aufbau des Datenwörterbuchs mit den Standardzuordnungsfeldern

* Da Marketo Engage eine einfache Datenbank verwendet, wird empfohlen, das Datenwörterbuch wie folgt zu formatieren:

   * Erste Spalte: Marketo Engage von Feldnamen
   * Zweite Spalte: Marketo Engage-API-Namen
   * Dritte Spalte: [Marketo Engage-Feldtyp](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} (d. h. Boolesch, Währung, Datum usw.)
   * In nachfolgenden Spalten wiederholen Sie den Vorgang für die CRM-Objekttypen (Lead, Kontakt, Konto, Opportunity) mit einer zusätzlichen Spalte für die Zugriffsebene, die Sie für das Marketo Engage haben möchten (d. h. Lesen, Schreiben, Bearbeiten)

  <br>

  Im Folgenden finden Sie ein Beispiel dafür, wie sie aussehen würde:
  ![Datenwörterbuchtabelle](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* Fügen Sie zunächst die Standardfelder hinzu, die automatisch für Ihr CRM-System zugeordnet werden:

   * [Salesforce](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [Veeva](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Bestätigen Sie, dass jedes Standardfeld im Marketo Engage mit dem Feld im CRM übereinstimmt, mit dem Sie synchronisieren möchten. Das Feld „Abgemeldet“ in Marketo Engage könnte beispielsweise das Feld „E-Mail-Abmeldung“ in Ihrem CRM sein.
* Passen Sie bei Bedarf den CRM-API[Namen, die Berechtigungen und den ](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"}Datentyp“ an.

**Schritt 4:** Hinzufügen zusätzlicher Felder zum Datenwörterbuch

* Geben Sie für jedes Feld den Anzeigenamen, die gewünschten CRM-Berechtigungen und den Datentyp an.
* Wenn ein Feld im CRM vorhanden ist, aber nicht auf dem Marketo Engage, füllen Sie die Marketo Engage-Anzeige und die API-Namen mit denselben Werten aus dem CRM-Feld aus.
* Wenn ein Feld im Marketo Engage, aber nicht im CRM vorhanden ist, füllen Sie den CRM-Anzeigenamen mit dem gewünschten Wert aus, lassen Sie jedoch den CRM-API-Namen leer, bis das Feld erstellt wurde.
* Wenn in beiden Systemen entsprechende Felder vorhanden sind, fügen Sie diese in dieselbe Zeile ein und geben Sie an, dass sie im Abschnitt „Hinweise“ ganz rechts in Ihrem Datenwörterbuchblatt neu zugeordnet werden müssen.

>[!NOTE]
>Wenn Sie ein Synchronisierungsfilterfeld ([Salesforce) erstellen ](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter){target="_blank"}), stellen Sie sicher, dass Sie sie in diesen Schritt einbeziehen, aber die API-Namen leer lassen, bis das Feld in Ihrem CRM erstellt wird.

**Schritt 5:** Überprüfen Sie das Datenwörterbuch mit Ihrem CRM-Administrator

* Erstellen Sie Felder im CRM für diejenigen, die bereits im Marketo Engage vorhanden sind, und aktualisieren Sie das Datenwörterbuch mit den Anzeige- und API-Namen für das neue CRM-Feld.
* Feldzuordnung zwischen Lead- und Kontaktobjekten in Ihrem CRM durchführen ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}). Wenn ein Lead in ein Kontaktfeld konvertiert wird, wird sichergestellt, dass die Felder in Marketo Engage zu einem einzigen Feld zusammengefasst werden können.
* Stellen Sie sicher, dass das Marketo-Synchronisierungsprofil über die entsprechenden Berechtigungen für jedes Feld verfügt, wie im Datenwörterbuch angegeben:
   * [Festlegen von Profilberechtigungen in Salesforce](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [Festlegen von Profilberechtigungen in Microsoft Dynamics](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [Festlegen von Profilberechtigungen in Veeva](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage#set-profile-permissions){target="_blank"}

**Schritt 6:** Erste Synchronisierung durchführen

* Stellen Sie sicher, dass alle Felder, die Sie mit Marketo Engage synchronisieren möchten, in Ihrem CRM die entsprechenden Berechtigungen haben, wie im Datenwörterbuch definiert.
* Stellen Sie sicher, dass alle Felder **die Sie** mit Marketo Engage synchronisieren möchten, [im Marketo-Synchronisierungsprofil ausgeblendet](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}. Es ist viel einfacher, der Synchronisierung später neue Felder hinzuzufügen, als unbeabsichtigt synchronisierte Felder zu entfernen.
* Verbinden Sie Ihr CRM mit dem Feld Synchronisierungsfilter? Wenn Sie mit Salesforce synchronisieren, wenden Sie sich an den Kunden-Support von Adobe, um sicherzustellen, dass die Filterfunktion aktiviert ist, bevor Sie mit der ersten Synchronisierung beginnen.


**Schritt 7:** Lesen Sie den Abschnitt Feldverwaltung auf Marketo Engage

* Bestätigen/aktualisieren Sie die Anzeige- und API-Namen für die neuen synchronisierten Felder.
* Identifizieren Sie alle doppelten Felder, die möglicherweise neu zugeordnet werden müssen. Duplizierte Felder treten in einigen Szenarien auf:
   * Benutzerdefinierte Felder im CRM würden bei der ersten Synchronisierung ein neues (potenziell doppeltes) Feld im Marketo Engage erstellen, wenn bereits ein entsprechendes Feld im Marketo Engage vorhanden wäre.
   * Benutzerdefinierte Felder, die nur Marketo-Engage betreffen (d. h. Felder, die direkt in Marketo Engage erstellt wurden), können mit einem entsprechenden Feld synchronisiert werden.



**Schritt 8: Wenden** sich an den Adobe-Support, um eine Neuzuordnung durchzuführen, wenn doppelte Felder angezeigt werden

* Wenden Sie sich mit den folgenden Informationen an den Support für Felder, die neu zugeordnet werden müssen:
   * Anzeige- und API-Namen für neue doppelte Felder, die vom CRM erstellt wurden.
   * Anzeigename für das Marketo Engage-Feld, dem das CRM-Feld zugeordnet werden soll.
   * Siehe dieses Beispiel [HIER](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"}.
* Sobald die Neuzuordnung abgeschlossen ist, überprüfen Sie die API-Namen für die neu zugeordneten Felder im Marketo Engage und aktualisieren Sie die Werte in der Spalte „API-Name“ Ihres Datenwörterbuchs, um sicherzustellen, dass es die genauesten Informationen enthält.

## Wie geht es weiter?

* Erstellen Sie Ihr Datenwörterbuch, um Ihre Felder für die CRM-Integration zu organisieren.
* Machen Sie sich mit dem anfänglichen Synchronisierungsprozess für Ihr CRM vertraut

>[!BEGINTABS]

>[!TAB Salesforce]

Erfahren Sie, wie Marketo Engage und Salesforce zusammenarbeiten, um Ihre Verkaufs- und Marketingdaten synchron zu halten.

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**Im Video verwendete Links:**

* [Grundlegendes zur Synchronisierung von Salesforce](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync){target="_blank"}

* [Marketo-Felder zu Salesforce hinzufügen (Enterprise/Unlimited)](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited){target="_blank"}

* [Erstellen eines Marketo-Benutzers in Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited){target="_blank"}

* [Marketo und Salesforce verbinden (Enterprise/Unlimited)](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited){target="_blank"}

* [Benutzer müssen die verbundene App auf der Salesforce-Seite einrichten, bevor sie mit der Synchronisierung von Marketo und Salesforce fortfahren können.](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0){target="_blank"}

* [Synchronisierungsstatus für Salesforce](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status){target="_blank"}

* [Ein- und Ausblenden eines Felds](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field){target="_blank"}

* [Tutorial: Erfahren Sie mehr über das Synchronisieren von Marketo mit Ihrem CRM](https://experienceleague.adobe.com/de/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

Erfahren Sie, wie die Microsoft Dynamics 365-Synchronisierung funktioniert, und konfigurieren Sie das Setup ordnungsgemäß, damit die beiden Systeme miteinander sprechen können.

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**Im Video verwendete Links:**

* [Grundlegendes zur Synchronisierung von Microsoft Dynamics](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync){target="_blank"}

* [Marketo Lead Management-Lösung herunterladen](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution){target="_blank"}

* [Aktualisieren der Marketo-Lösung für Microsoft Dynamics](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics){target="_blank"}

* [Einverständnis für Client-ID und App-Registrierung erteilen](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration)

* [Validieren der Microsoft Dynamics-Synchronisierung](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync){target="_blank"}

* [Synchronisierungsstatus](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status){target="_blank"}

* [Beheben von Synchronisationsproblemen bei der Dynamics-Validierung](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues){target="_blank"}

* [Erstellen eines benutzerdefinierten Dynamics-Synchronisierungsfilters](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynamics-sync-filter-details/create-a-custom-dynamics-sync-filter.html?lang=de){target="_blank"}

* [Anzeigen der Organisations-Service-URL](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url){target="_blank"}

* [Bearbeiten von Feldern, die vor dem Löschen in Dynamics synchronisiert werden sollen](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics){target="_blank"}

* [Tutorial: Erfahren Sie mehr über das Synchronisieren von Marketo mit Ihrem CRM](https://experienceleague.adobe.com/de/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn){target="_blank"}

+++

>[!ENDTABS]

### Autoren

{{peter-livadas}}

{{amy-chiu}}
