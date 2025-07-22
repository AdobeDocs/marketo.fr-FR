---
description: Synchronisation de la tâche de rappel avec Salesforce - Documents Marketo - Documentation du produit
title: Synchronisation de la tâche de rappel avec Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Synchronisation de la tâche de rappel avec [!DNL Salesforce] {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Pour savoir comment activer la synchronisation des tâches, consultez la section [Synchroniser les tâches/rappels des actions Insight Sales avec les tâches Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Une fois que les paramètres de synchronisation des tâches sont activés, les utilisateurs voient leurs tâches de rappel synchronisées de manière bidirectionnelle avec [!DNL Salesforce]. Cela signifie que les utilisateurs peuvent gérer les tâches à partir de [!DNL Salesforce] ou de [!DNL Sales Insight Actions] et qu’ils sont convaincus que les systèmes resteront alignés.

## Synchronisation du champ de tâche de rappel {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Vous trouverez ci-dessous la liste des champs de tâche de rappel dans [!DNL Sales Insight Actions] et leurs champs de [!DNL Salesforce] correspondants pris en charge par la synchronisation bidirectionnelle des tâches.

<table>
 <tr>
  <th>[!DNL Sales Insight Actions] Champ de la tâche</th>
  <th>[!DNL Salesforce] Champ de la tâche</th>
  <th>[!DNL Salesforce] Tâche</th>
 </tr>
 <tr>
  <td>[!UICONTROL Task Name]</td>
  <td>[!UICONTROL Subject Field]</td>
  <td>Champ de résumé court destiné à afficher le titre de la tâche.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Status]</td>
  <td>[!UICONTROL Task Status]</td>
  <td><p>Affiche le statut de la tâche. [!DNL Sales Insight Actions] tâches comportent deux statuts qui correspondent à deux des valeurs de la liste de sélection du statut de la tâche [!DNL Salesforce].</p>
  <p>Ouvrir dans [!DNL Sales Insight Actions] = Non démarré dans [!DNL Salesforce].</p>
  <p>Terminé en [!DNL Sales Insight Actions] = Terminé en [!DNL Salesforce].</p>
  <p>Les autres valeurs de statut dans [!DNL Salesforce] ne seront pas synchronisées avec [!DNL Sales Insight Actions].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Priority]</td>
  <td>[!UICONTROL Priority]</td>
  <td><p>[!DNL Sales Insight Actions] La priorité peut être Normale ou Élevée, ce qui correspond aux valeurs de priorité Normale et Élevée dans [!DNL Salesforce].</p>
  <p>La valeur de priorité basse dans [!DNL Salesforce] ne sera pas synchronisée avec [!DNL Sales Insight Actions].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Due Date]</td>
  <td>[!UICONTROL Due Date]</td>
  <td>Date d’échéance de la tâche.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Details]</td>
  <td>[!UICONTROL Comments]</td>
  <td>Affiche des informations plus détaillées sur ce qui était censé être terminé avec la tâche de rappel.</td>
 </tr>
</table>

## Première synchronisation de tâches [!DNL Sales Insight Actions] avec [!DNL Salesforce] {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Lorsque vous activez pour la première fois la synchronisation entre les tâches [!DNL Sales Insight Actions] et [!DNL Salesforce], nous importons vos tâches [!DNL Salesforce]. Nous **transmettrons pas** tâches en cours que vous avez en [!DNL Sales Insight Actions] à [!DNL Salesforce]. Pour réduire l’encombrement et les doublons, les seules tâches synchronisées à partir de [!DNL Sales Insight Actions] dans [!DNL Salesforce] sont les tâches créées *après* vous synchronisez [!DNL Sales Insight Actions] avec SFDC.

Voici ce qui se produit lorsque vous synchronisez des tâches [!DNL Sales Insight Actions] et SFDC :

* Dès que vous cliquez sur Enregistrer sur les tâches en cours de synchronisation, elles commencent à se synchroniser. Cela prendra un certain temps au début.

* Tous les rappels qui ont été mis à jour ou créés au cours des dernières 24 heures seront extraits de SFDC vers [!DNL Sales Insight Actions]. La synchronisation est basée sur la date d’échéance et toutes ces tâches seront synchronisées en arrière-plan, mais dans le centre de commande, vous ne verrez que les tâches dues aujourd’hui et demain.

* Si la synchronisation a été activée précédemment et que vous supprimez des tâches dans SFDC, tout ce qui a été supprimé au cours des 15 derniers jours sera supprimé du Centre de commande.

* Nous synchroniserons constamment les tâches entre [!DNL Sales Insight Actions] et SFDC tant que la synchronisation sera activée.

Après la synchronisation initiale, toutes les tâches que vous créez, modifiez, terminez ou supprimez dans [!DNL Sales Insight Actions] seront synchronisées avec votre liste de tâches dans [!DNL Salesforce]. Et tout ce qui sera créé, modifié, terminé ou supprimé dans [!DNL Salesforce] mettra à jour votre liste de tâches dans [!DNL Sales Insight Actions].

Pour activer cette synchronisation, cochez simplement la case de synchronisation dans la page [Paramètres](https://toutapp.com/login) de l’application web.

>[!NOTE]
>
>Le champ d’objet d’une tâche peut être mis à jour en [!DNL Sales Insight Actions] et cette mise à jour sera synchronisée dans le champ d’objet [!DNL Salesforce] de la tâche synchronisée correspondante, si vous utilisez le champ dynamique `{{activity_subject}}` dans vos paramètres [Personnalisation des détails de l’activité](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). À l’inverse, les mises à jour apportées au champ d’objet dans [!DNL Salesforce] ne seront _pas_ synchronisées avec le champ d’objet de la tâche de rappel de [!DNL Sales Insight Actions].
