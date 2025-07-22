---
unique-page-id: 2953473
description: Synchronisation de SFDC - Synchronisation des activités - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation des activités
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 5%

---

# Synchronisation SFDC : synchronisation des activités {#sfdc-sync-activity-sync}

Marketo effectue également une synchronisation sur les données des activités [!DNL Salesforce]. Voici quelques questions et réponses.

## Quels types de données d’activité Marketo synchronise-t-il ? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo se synchronise sur les événements et les tâches associés à un prospect ou à un contact.

## Comment les détails des activités sont-ils synchronisés entre les deux systèmes ? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

La synchronisation fonctionne dans un sens, de [!DNL Salesforce] à Marketo. Cependant, vous pouvez créer une tâche dans [!DNL Salesforce] à l’aide de l’étape de flux [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) ou [Personnaliser la synchronisation des activités](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) pour [!DNL Salesforce].

## Puis-je créer une tâche à l’aide de Marketo ? {#can-i-create-a-task-using-marketo}

Oui, vous pouvez utiliser l’action [ Créer un flux de tâches ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}.

## Quels sont les déclencheurs/filtres liés à l’activité ? {#what-are-the-triggers-filters-related-to-activity}

Déclencheurs

* Activité consignée
* Activité mise à jour

Filtres

* L’activité était consignée/non l’activité était consignée
* L’activité a été mise à jour/pas l’activité a été mise à jour

>[!TIP]
>
>Vous n&#39;êtes pas sûr de la formulation « Pas d&#39;activité » ? Le terme « not » fait référence à un filtre d’inactivité. Pour en savoir plus à leur sujet, cliquez ici : [Utiliser des filtres d’inactivité dans une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
