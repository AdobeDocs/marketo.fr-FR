---
unique-page-id: 2953473
description: Synchronisation SFDC - Synchronisation des Activités - Documentation sur le marketing - Documentation du produit
title: Synchronisation SFDC -Synchronisation des Activités
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Synchronisation SFDC : Synchronisation des Activités {#sfdc-sync-activity-sync}

Marketo se synchronise également sur les données des activités Salesforce. Voici quelques questions et réponses.

## Sur quels types de données d&#39;activité Marketo synchronise-t-il ? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo se synchronise sur les Événements et les Tâches associés à un prospect ou contact.

## Comment les détails des activités sont-ils synchronisés entre les deux systèmes ? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

La synchronisation est un moyen, de Salesforce à Marketo. Mais vous pouvez créer une tâche dans Salesforce à l’aide de l’étape de flux [Créer une Tâche](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) ou [Personnaliser la synchronisation des Activités](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) vers Salesforce.

## Puis-je créer une tâche à l’aide de Marketo ? {#can-i-create-a-task-using-marketo}

Oui, vous pouvez utiliser l&#39;action [Créer un flux de Tâche](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## Quels sont les déclencheurs/filtres liés à l&#39;activité ? {#what-are-the-triggers-filters-related-to-activity}

Déclencheurs

* Activité consignée
* Activité mise à jour

Filtres

* Activité consignée/Activité non consignée
* Activité mise à jour/Aucune Activité mise à jour

>[!TIP]
>
>Vous n&#39;êtes pas sûr de ce libellé &quot;Pas Activité&quot; ? Le &quot;non&quot; fait référence à un filtre d’inactivité. Pour en savoir plus, cliquez ici : [Utiliser les Filtres d&#39;inactivité dans une Liste dynamique](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

