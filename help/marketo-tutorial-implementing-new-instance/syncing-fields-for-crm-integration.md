---
title: Synchronisieren von Feldern für die nativen CRM-Connectoren
description: Erfahren Sie, wie Sie Ihre anfängliche CRM-Integration optimieren können, indem Sie strategisch die wesentlichen CRM-Felder auswählen, die für die Marketo Engage verwendet werden sollen. Führen Sie die Übung "Datenwörterbuch"aus, um die Felder zu identifizieren, die Sie für eine reibungslose CRM-Synchronisierung benötigen, die Vertriebs- und Marketingteams dabei unterstützt, sich auf dem neuesten Stand zu halten.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14811
thumbnail: KT-14811.jpeg
exl-id: 42b7ca3d-e445-4c11-ad3d-d4e70c101c8e
source-git-commit: bed599454a75159492f13aab1f802c09d92bf7ed
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Synchronisieren von Feldern für die nativen CRM-Connectoren

Verwenden Sie Salesforce oder Microsoft Dynamics in Ihrem Unternehmen? Ist dies der Fall, können Sie mit den nativen CRM-Connectoren von Marketo Engage (z. B. Salesforce, Microsoft Dynamics und Veeva) Marketing- und Verkaufsaktivitäten koordinieren, indem Sie relevante Informationen nahtlos zwischen Marketo Engage und CRM austauschen. Stellen Sie vor der Konfiguration der anfänglichen CRM-Synchronisation sicher, dass Sie die Felder identifizieren, die zwischen den beiden Systemen synchronisiert werden sollen, damit Ihre Marketo Engage-Datenbank sauber bleibt.

Erfahren Sie mehr darüber, wie Sie diese Übung mit Best Practices durchführen können, die von Adobe Professional Services empfohlen werden. Machen Sie sich mit den Standardfeldern und benutzerdefinierten Feldern vertraut und dokumentieren Sie die Beziehungen zwischen Marketo Engage und Ihrem CRM-System.

## Identifizieren Sie die zu synchronisierenden Felder, bevor Sie Ihr CRM mit Marketo Engage integrieren.

Bei der Integration Ihres CRM mit Marketo Engage müssen Sie wahrscheinlich nicht alle Ihre CRM-Felder mit Marketo Engage synchronisieren. Eine strategische Ausrichtung der benötigten Felder kann Ihrer Marketo Engage-Instanz dabei helfen, den Datenfluss effizienter zu verarbeiten.

Die anfängliche Synchronisation zwischen Ihrem Marketo Engage- und CRM-System führt automatisch Verknüpfungen für die meisten vorhandenen Standardfelder (E-Mail, Vor-/Nachname, Firma usw.) durch. Darüber hinaus synchronisiert der Connector [benutzerdefinierte Felder](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} für Ihre Leads, Kontakte, Konten und Möglichkeiten, indem neue Felder in Marketo Engage erstellt werden, die automatisch diesen Feldern aus Ihrem CRM-System zugeordnet werden.

Das Identifizieren und Organisieren der Felder, die Sie vor der ersten Synchronisierung aus Ihrem CRM-System synchronisieren möchten, ist ein wichtiger Schritt im Setup-Prozess von Native Connector. Dies wird als Datenwörterbuch bezeichnet, das Ihnen dabei hilft, die Anzahl der duplizierten Felder, die erstellt werden, zu minimieren und alle nachfolgenden Neukodifizierungsschritte so reibungslos wie möglich zu gestalten. Diese Übung umfasst in der Regel Beiträge der Marketing- und Verkaufsteams und Ihres CRM-Administrators, um sicherzustellen, dass nur relevante Felder mit Ihrer Marketo Engage-Instanz synchronisiert werden.

## Erstellen Ihres Datenwörterbuchs

Im Allgemeinen wird empfohlen, nur CRM-Felder zu synchronisieren, die für Marketing-Zwecke benötigt werden. Beginnen Sie mit dieser Übung, um die Felder aus Ihrem CRM-System zu organisieren, die der Marketo Engage zugeordnet werden müssen, und führen Sie die erste CRM-Synchronisierung korrekt aus.

>[!NOTE]
>Wenn Sie in Ihrem CRM-System benutzerdefinierte Felder haben, die bereits über ein entsprechendes benutzerdefiniertes Feld in Marketo Engage verfügen, bevor Sie mit der ersten Synchronisation beginnen, wird unter Marketo Engage ein neues Duplikat-Feld für das CRM-Feld erstellt. Sie können das CRM-Feld dem ursprünglichen Marketo Engage-Feld neu zuordnen und das doppelte Feld nach Abschluss der ersten Synchronisation ausblenden. Dazu müssen Sie sich jedoch an den [Adobe-Support](https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"} wenden. Weitere Informationen finden Sie in Schritt 7 .

**Schritt 1:** Erstellen Sie eine grobe Liste der derzeit in Ihrem CRM-System verfügbaren Felder und markieren Sie, ob sie im Marketo Engage angezeigt werden sollen.

* Nehmen Sie Feedback von Ihrem CRM-Administrator, Marketing- und Verkaufsteams in den Entscheidungsprozess auf.
* Dokumentieren Sie die API-Namen und Feldtypen für jedes Feld.
* Legen Sie fest, welche Zugriffsebene Marketo Engage für diese Felder haben sollte (d. h. Schreibgeschützt oder Lese-Schreib).


**Schritt 2:** Überprüfen Sie den Abschnitt &quot;[Admin > Feldverwaltung&quot;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} Ihrer Marketo Engage-Instanz, um alle benutzerdefinierten Felder zu identifizieren, die zuvor direkt im System erstellt wurden und die Sie in die Synchronisierung einbeziehen möchten.

* Dokumentieren Sie die API-Namen und Feldtypen für jedes Feld.
* Felder kennzeichnen, die bereits über ein entsprechendes Feld in Ihrem CRM-System verfügen.
* Felder bezeichnen, die noch kein entsprechendes Feld in Ihrem CRM-System haben.


**Schritt 3:** Beginnen Sie mit dem Erstellen des Datenwörterbuchs mit den Standardzuordnungsfeldern.

* Da Marketo Engage eine einfache Datenbank verwendet, wird empfohlen, Ihr Datenwörterbuch wie folgt zu formatieren:

   * Erste Spalte: Marketo Engage-Feldnamen
   * Zweite Spalte: Marketo Engage-API-Namen
   * Dritte Spalte: [Marketo Engage Feldtyp](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} (d. h. Boolesch, Währung, Datum usw.)
   * Wiederholen Sie in den nachfolgenden Spalten für die CRM-Objekttypen (Lead, Kontakt, Konto, Möglichkeit) eine zusätzliche Spalte für den Zugriffsgrad, den Marketo Engage haben soll (d. h. Lesen, Schreiben, Bearbeiten).
  <br>

  Hier ist ein Beispiel dafür, wie es aussehen würde:
  ![Datenwörterbuchtabelle](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* Fügen Sie zunächst die Standardfelder hinzu, die automatisch für Ihr CRM-System zugeordnet werden:

   * [Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Bestätigen Sie, dass jedes Standardfeld in Marketo Engage mit dem Feld in Ihrem CRM-System übereinstimmt, mit dem Sie synchronisieren möchten. Beispielsweise könnte das Feld &quot;Abgemeldet&quot; in Marketo Engage das Feld &quot;E-Mail-Abmeldung&quot; in Ihrem CRM-System sein.
* Passen Sie bei Bedarf den CRM-API-Namen, die Berechtigungen und den [Datentyp](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} an.

**Schritt 4:** Hinzufügen zusätzlicher Felder zum Datenwörterbuch

* Schließen Sie den Anzeigenamen, die gewünschten CRM-Berechtigungen und den Datentyp für jedes Feld ein.
* Wenn ein Feld im CRM-System vorhanden ist, aber nicht im Marketo Engage, füllen Sie die Marketo Engage- und API-Namen mit den gleichen Werten aus dem CRM-Feld aus.
* Wenn ein Feld in der Marketo Engage vorhanden ist, aber nicht im CRM, geben Sie den CRM-Anzeigenamen mit dem gewünschten Wert an, lassen Sie jedoch den CRM-API-Namen leer, bis das Feld erstellt wurde.
* Wenn in beiden Systemen gleichwertige Felder vorhanden sind, fügen Sie sie in derselben Zeile ein und weisen Sie darauf hin, dass sie im Abschnitt &quot;Hinweise&quot;ganz rechts im Datenwörterbuchblatt neu zugeordnet werden müssen.

>[!NOTE]
>Wenn Sie ein Synchronisierungsfilterfeld ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"}) erstellen möchten | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}), stellen Sie sicher, dass Sie ihn in diesen Schritt einbeziehen, lassen Sie die API-Namen jedoch leer, bis das Feld in Ihrem CRM-System erstellt wird.

**Schritt 5:** Überprüfen Sie das Datenwörterbuch mit Ihrem CRM-Administrator.

* Erstellen Sie im CRM Felder, die bereits im Marketo Engage vorhanden sind, und aktualisieren Sie das Datenwörterbuch mit den Anzeige- und API-Namen für das neue CRM-Feld.
* Führen Sie eine Feldzuordnung zwischen Lead- und Kontaktobjekten in Ihrem CRM durch ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"}) | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}). Wenn ein Lead in einen Kontakt umgewandelt wird, stellt dies sicher, dass die Felder in einem einzigen Feld im Marketo Engage zusammengefasst werden können.
* Stellen Sie sicher, dass das Marketo-Synchronisierungsprofil über die entsprechenden Berechtigungen für jedes Feld verfügt, wie im Datenwörterbuch angegeben:
   * [ Festlegen von Profilberechtigungen in Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [Festlegen von Profilberechtigungen in Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [Festlegen von Profilberechtigungen in VEEev](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}

**Schritt 6:** Ausführen der ersten Synchronisierung

* Stellen Sie sicher, dass alle Felder, die Sie mit Marketo Engage synchronisieren möchten, über die entsprechenden Berechtigungen in Ihrem CRM-System verfügen, wie im Datenwörterbuch definiert.
* Stellen Sie sicher, dass alle Felder, die ***nicht*** mit Marketo Engage synchronisieren möchten, [im Marketo-Synchronisierungsprofil ausgeblendet sind](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}. Es ist viel einfacher, der Synchronisierung später neue Felder hinzuzufügen, als unbeabsichtigt synchronisierte Felder zu entfernen.
* Verbinden Sie Ihr CRM mit dem Feld Filter synchronisieren . Wenn Sie eine Synchronisierung mit Salesforce durchführen, wenden Sie sich an den Adobe-Support, um sicherzustellen, dass die Filterfunktion aktiviert ist, bevor Sie die erste Synchronisierung starten.


**Schritt 7:** Überprüfen Sie den Abschnitt &quot;Feldverwaltung&quot;unter Marketo Engage.

* Bestätigen/aktualisieren Sie die Anzeige- und API-Namen für die neuen synchronisierten Felder.
* Identifizieren Sie alle duplizierten Felder, die möglicherweise neu zugeordnet werden müssen. Duplizierte Felder treten in einigen Szenarien auf:
   * Benutzerdefinierte Felder im CRM würden beim ersten Synchronisieren ein neues (potenziell doppeltes) Feld im Marketo Engage erstellen, wenn bereits ein entsprechendes Feld im Marketo Engage vorhanden war.
   * Benutzerdefinierte Marketo-Engage-Only-Felder (d. h. ein direkt in Marketo Engage erstelltes Feld) und ein entsprechendes Feld kann aus dem CRM synchronisiert werden.



**Schritt 8:** Wenden Sie sich an den Adobe-Support, um eine Neukodierung durchzuführen, falls duplizierte Felder angezeigt werden.

* Wenden Sie sich an den Support mit den folgenden Informationen für Felder, die neu zugeordnet werden müssen:
   * Anzeige und API-Namen für neue duplizierte Felder, die vom CRM erstellt wurden.
   * Anzeigename für das Marketo Engage-Feld, dem das CRM-Feld zugeordnet werden soll.
   * Weitere Informationen finden Sie in diesem Beispiel [HIER](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"} .
* Überprüfen Sie nach Abschluss der Neukodifizierung die API-Namen für die neu zugeordneten Felder in Marketo Engage und aktualisieren Sie die Werte in der Spalte &quot;API-Name&quot;Ihres Datenwörterbuchs, um sicherzustellen, dass sie die genauesten Informationen enthält.

## Wie geht es weiter?

* Erstellen Sie Ihr Datenwörterbuch, um Ihre Felder für die CRM-Integration zu organisieren.
* Machen Sie sich mit dem anfänglichen Synchronisierungsprozess für Ihr CRM vertraut.

>[!BEGINTABS]

>[!TAB Salesforce]

Erfahren Sie, wie Marketo Engage und Salesforce zusammenpassen, um Ihre Verkaufs- und Marketingdaten synchron zu halten.

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**Im Video verwendete Links:**

* [Erläuterungen zur Salesforce-Synchronisation](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.html){target="_blank"}

* [Marketo-Felder zu Salesforce hinzufügen (Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.html){target="_blank"}

* [Erstellen eines Marketo-Benutzers in Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.html){target="_blank"}

* [Verbinden von Marketo und Salesforce(Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.html){target="_blank"}

* [Benutzer müssen die verbundene App auf Salesforce-Seite einrichten, bevor sie mit der Synchronisierung von Marketo und Salesforce fortfahren.](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.html){target="_blank"}

* [Salesforce-Synchronisierungsstatus](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status.html){target="_blank"}

* [Ein Feld ausblenden und einblenden](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field.html){target="_blank"}

* [Tutorial: Erfahren Sie mehr über die Synchronisierung von Marketo mit Ihrem CRM](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

Erfahren Sie, wie die Synchronisierung mit Microsoft Dynamics 365 funktioniert, und konfigurieren Sie das Setup ordnungsgemäß, damit die beiden Systeme miteinander sprechen können.

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**Im Video verwendete Links:**

* [Die Synchronisierung von Microsoft Dynamics verstehen](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync.html){target="_blank"}

* [Laden Sie die Marketo-Lead-Management-Lösung herunter](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution.html){target="_blank"}

* [Aktualisieren der Marketo-Lösung für Microsoft Dynamics](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.html){target="_blank"}

* [Erteilen der Zustimmung für die Client-ID und App-Registrierung](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration.html)

* [Überprüfen der Synchronisierung von Microsoft Dynamics](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync.html){target="_blank"}

* [Synchronisierungsstatus](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status.html){target="_blank"}

* [Beheben von Synchronisierungsproblemen bei der Dynamics-Überprüfung](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues.html){target="_blank"}

* [Erstellen eines benutzerdefinierten Synchronisierungsfilters für Dynamics](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynmaics-sync-filter-details/create-a-custom-dynamics-sync-filter.html){target="_blank"}

* [Anzeigen der Organisationsdienst-URL](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url.html){target="_blank"}

* [ Bearbeiten von zu synchronisierenden Feldern vor dem Löschen in Dynamics](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics.html){target="_blank"}

* [Tutorial: Erfahren Sie mehr über die Synchronisierung von Marketo mit Ihrem CRM](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!ENDTABS]

### Autoren

{{peter-livadas}}

{{amy-chiu}}

