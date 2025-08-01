---
description: Configuration De La Personnalisation Des Détails De L’Activité Salesforce - Documents Marketo - Documentation Du Produit
title: Configurer la personnalisation des détails de l’activité Salesforce
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 1%

---

# Configurer la personnalisation des détails de l’activité [!DNL Salesforce] {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce et les actions Sales Insight [doivent être connectées](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* La journalisation de l’activité e-mail via l’API [doit être activée](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)

La personnalisation des détails de l’activité permet aux administrateurs de configurer les informations qui seront consignées dans le champ [!DNL Salesforce] la tâche - Objet, lorsqu’une activité [!DNL Sales Insight Actions]/tâche de rappel est synchronisée avec [!DNL Salesforce].

>[!NOTE]
>
>* Les mises à jour apportées au champ objet en [!DNL Sales Insight Actions] d’une tâche de rappel sont répercutées dans le champ objet de la tâche de [!DNL Salesforce] correspondante, si vous utilisez le champ dynamique `{{activity_subject}}` dans votre personnalisation des détails de l’activité.
>* Les sauts de ligne ne sont pas pris en charge lors de la journalisation des informations dans le champ objet [!DNL Salesforce]. Tous les sauts de ligne dans l’éditeur Personnalisation des détails de l’activité sont supprimés lorsqu’un objet de tâche de vente est mis à jour.

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>Tâche de rappel InMail</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>Activité d’e-mail</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>Activité d’appel</td>
 </tr>
</table>

Cette fonctionnalité peut être utilisée pour déverrouiller les avantages suivants :

* En personnalisant les informations visibles dans le champ de l’objet, vous pouvez facilement rechercher des détails d’activité pour les ventes dans Salesforce.
* Les administrateurs peuvent baliser le champ d’objet avec un identifiant unique tel que « Mkto_sales » afin que les activités des actions Sales Insight puissent être facilement identifiées et différenciées des autres activités de messagerie, d’appel et des tâches.
* Réduire le besoin de champs d’activité personnalisés Salesforce impose des limites sur le nombre de champs d’activité personnalisés, ce qui peut restreindre les données disponibles qui peuvent être utilisées dans les rapports. En utilisant des champs dynamiques d’activité pour ajouter des données essentielles à la ligne d’objet, vous pouvez réduire le nombre de champs d’activité personnalisés à créer dans votre instance Salesforce.
* Le champ d’objet des activités et des tâches suit un modèle cohérent défini par l’administrateur des actions Sales Insight.

>[!NOTE]
>
>Si vous enregistrez les réponses aux e-mails en tant qu’activités dans [!DNL Salesforce], les paramètres de personnalisation des détails de l’activité [!DNL Salesforce] ne seront pas utilisés. Au lieu de cela, ils se connectent en tant que « Réponse : objet de l’e-mail ».

## Champs dynamiques d’activité pris en charge {#activity-dynamic-fields-supported}

Les champs dynamiques d’activité fournissent des informations de référence sur vos activités de vente pour renseigner les données. Aujourd’hui, ils peuvent être utilisés avec la personnalisation des détails de l’activité [!DNL Salesforce].

>[!NOTE]
>
>S’il n’existe aucune valeur pour renseigner le champ dynamique pour une activité/tâche spécifique, il ne renseignera aucune donnée pour ce champ dynamique lorsque le champ Tâche - Objet de Salesforce sera mis à jour.

<table>
 <tr>
  <th>Champ</th>
  <th>Description</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>Remplit le type de tâche en tant qu’e-mail, appel, courrier électronique ou personnalisé.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Renseigne l'objet de la tâche.</p>
      <p>Dans le cas d’un e-mail, il renseigne la ligne d’objet de l’e-mail.</p>
      <p>Dans le cas d’un appel, inMail ou personnalisé, il renseigne une valeur si une tâche de rappel a été créée avec une valeur dans le champ nom/objet de la tâche.</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>Si l’activité a été lancée à partir d’une campagne de vente, elle renseigne le nom de la campagne de vente.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>Si l'activité a été lancée à partir d'une campagne commerciale, elle renseigne le numéro du jour de la campagne commerciale où cette activité s'est produite.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>Si l’activité a été lancée à partir d’une campagne commerciale, le numéro d’étape est renseigné dans le jour de la campagne commerciale où cette activité a eu lieu.</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>Si l’activité est un appel et qu’un résultat d’appel est sélectionné, la valeur de résultat d’appel est renseignée.</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>Si l’activité est un appel et qu’un motif d’appel est sélectionné, la valeur de motif d’appel est renseignée.</td>
 </tr>
</table>

## Configuration de la personnalisation des détails de l’activité [!DNL Salesforce] {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Autorisations d’administrateur requises.**

Lors de la configuration des détails de votre activité, réfléchissez aux données les plus pertinentes pour les ventes lors de la révision de l’historique des tâches dans [!DNL Salesforce].

1. Cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Cliquez sur **[!UICONTROL Salesforce]**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Cliquez sur **[!UICONTROL Paramètres de synchronisation]**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. Dans l’éditeur Personnalisation des détails de l’activité , ajoutez le texte libre de votre choix. Le texte que vous ajoutez n’est pas dynamique et reste inchangé pour le champ d’objet de toutes les tâches synchronisées avec [!DNL Salesforce].

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Bien que cela ne soit pas obligatoire, placer le texte ajouté entre crochets peut faciliter la distinction entre les données lorsqu’elles sont renseignées dans un champ d’objet dans [!DNL Salesforce]. Exemple : `[Sales Insight Actions] - {{Activity_type}}`

1. Ajoutez les champs dynamiques supplémentaires de votre choix en cliquant sur le bouton **[!UICONTROL Ajouter un champ dynamique]**.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Sélectionnez le ou les champs dynamiques souhaités.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>[!DNL Salesforce] applique une limite de 255 caractères. Si le détail de votre activité est supérieur à ce nombre, il sera tronqué pour s’assurer que les informations sont stockées dans le champ d’objet [!DNL Salesforce].

>[!MORELIKETHIS]
>
>* [Synchroniser les activités de vente avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Synchronisation de la tâche de rappel avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
