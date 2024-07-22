---
description: Synchronisation des tâches de rappel avec Salesforce - Documents Marketo - Documentation du produit
title: Synchronisation de la tâche de rappel avec Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 2%

---

# Synchronisation de la tâche de rappel avec Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Pour savoir comment activer la synchronisation des tâches, consultez [Synchroniser les tâches/rappels des actions d’aperçu des ventes avec les tâches Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Une fois les paramètres de synchronisation des tâches activés, les utilisateurs verront leurs tâches de rappel synchronisées de manière bidirectionnelle avec Salesforce. Cela signifie que les utilisateurs peuvent gérer les tâches à partir des actions Salesforce ou Sales Insight et se fier à l’alignement des systèmes.

## Synchronisation des champs de tâche de rappel {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Vous trouverez ci-dessous une liste des champs de tâche de rappel dans les actions Sales Insight et les champs Salesforce correspondants pris en charge par le biais de la synchronisation bidirectionnelle des tâches.

<table>
 <tr>
  <th>Champ de tâche des actions de Sales Insight</th>
  <th>Champ de tâche Salesforce</th>
  <th>Tâche Salesforce</th>
 </tr>
 <tr>
  <td>Nom de la tâche</td>
  <td>Objet</td>
  <td>Champ de résumé court destiné à afficher le titre de la tâche.</td>
 </tr>
 <tr>
  <td>Statut</td>
  <td>Statut de tâche</td>
  <td><p>Affiche l’état de la tâche. Les tâches des actions d’aperçu des ventes ont deux états qui correspondent à deux des valeurs de la liste de sélection d’état des tâches Salesforce.</p>
  <p>Ouvrir dans les actions Sales Insight = Not Started dans Salesforce.</p>
  <p>Terminé dans les actions Sales Insight = Terminé dans Salesforce.</p>
  <p>Les autres valeurs d’état de Salesforce ne sont pas synchronisées avec les actions de statistiques sur les ventes.</p></td>
 </tr>
 <tr>
  <td>Priorité</td>
  <td>Priorité</td>
  <td><p>La priorité des actions d’aperçu des ventes peut être Normale ou Élevée, ce qui correspond aux valeurs de priorité normale et élevée de Salesforce.</p>
  <p>La valeur de priorité basse dans Salesforce ne sera pas synchronisée aux actions Sales Insight.</p></td>
 </tr>
 <tr>
  <td>Échéance</td>
  <td>Échéance</td>
  <td>Date à laquelle la tâche doit être effectuée.</td>
 </tr>
 <tr>
  <td>Détails</td>
  <td>Commentaires</td>
  <td>Affiche des informations plus détaillées sur ce qui devait être effectué avec la tâche de rappel.</td>
 </tr>
</table>

## Synchronisation des tâches d’actions Sales Insight avec Salesforce pour la première fois {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Lorsque vous activez la synchronisation pour la première fois entre les actions Sales Insight et les tâches Salesforce, nous importons vos tâches Salesforce. Nous **n’allons pas** passer en revue toutes les tâches en cours dans les actions Sales Insight à Salesforce. Pour réduire l’encombrement et les doublons, les seules tâches qui sont synchronisées des actions Sales Insight dans Salesforce sont les tâches créées *après* que vous synchronisez les actions Sales Insight avec SFDC.

Voici ce qui se passe lorsque vous synchronisez les actions Sales Insight et les tâches SFDC :

* Dès que vous cliquez sur Enregistrer lors de la synchronisation des tâches, elles commencent à se synchroniser. Cela prendra du temps au départ.

* Les rappels qui ont été mis à jour ou créés au cours des dernières 24 heures seront transférés de SFDC aux actions Sales Insight . La synchronisation est basée sur l’échéance et toutes ces tâches seront synchronisées sur le serveur principal. Toutefois, dans le Centre de commandes, seules les tâches prévues aujourd’hui et demain seront visibles.

* Si la synchronisation a été activée précédemment et que vous supprimez des tâches dans SFDC, tout ce qui a été supprimé au cours des 15 derniers jours sera supprimé du Centre de commandes.

* Nous synchroniserons constamment les tâches entre les actions Sales Insight et SFDC tant que la synchronisation est activée.

Après la synchronisation initiale, toutes les tâches que vous créez, modifiez, terminez ou supprimez dans les actions Sales Insight se synchronisent avec votre liste de tâches dans Salesforce. De plus, tout élément créé, modifié, terminé ou supprimé dans Salesforce mettra à jour votre liste de tâches dans les actions Sales Insight.

Pour activer cette synchronisation, cochez simplement la case de synchronisation dans la [page Paramètres](https://toutapp.com/login) de l’application web.

>[!NOTE]
>
>Le champ d’objet d’une tâche peut être mis à jour dans les actions d’aperçu des ventes et cette mise à jour sera synchronisée dans le champ d’objet Salesforce pour la tâche synchronisée correspondante, si vous utilisez le champ dynamique `{{activity_subject}}` dans vos paramètres de [personnalisation des détails de l’activité](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). Inversement, toutes les mises à jour apportées au champ d’objet dans Salesforce se synchronisent _et non_ dans le champ d’objet de la tâche de rappel des actions de statistiques sur les ventes .
