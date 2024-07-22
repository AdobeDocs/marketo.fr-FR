---
unique-page-id: 2953473
description: Synchronisation SFDC - Synchronisation des activités - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation des activités
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 4%

---

# Synchronisation SFDC : synchronisation des activités {#sfdc-sync-activity-sync}

Marketo Engage se synchronise également sur les données des activités Salesforce. Voici quelques questions et réponses.

## Sur quels types de données d’activité Marketo se synchronise-t-il ? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo se synchronise sur les événements et les tâches associés à un prospect ou à un contact.

## Comment les détails de l’activité sont-ils synchronisés entre les deux systèmes ? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

La synchronisation est unidirectionnelle, de Salesforce à Marketo. Vous pouvez toutefois créer une tâche dans Salesforce à l’aide de l’étape de flux [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} ou [Personnaliser la synchronisation des activités](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md){target="_blank"} avec Salesforce.

## Puis-je créer une tâche à l’aide de Marketo ? {#can-i-create-a-task-using-marketo}

Oui, vous pouvez utiliser l’action [Créer un flux de tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}.

## Quels sont les déclencheurs/filtres liés à l’activité ? {#what-are-the-triggers-filters-related-to-activity}

Déclencheurs

* Activité consignée
* Activité mise à jour

Filtres

* Activité consignée/L’activité n’a pas été consignée
* Mise à jour/non de l’activité Mise à jour

>[!TIP]
>
>Vous n’êtes pas sûr de la formulation &quot;Pas d’activité&quot; ? &quot;not&quot; fait référence à un filtre d’inactivité. En savoir plus à ce sujet ici : [Utiliser les filtres d’inactivité dans une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
