---
unique-page-id: 2953473
description: Découvrez comment les activités et tâches Salesforce se synchronisent avec Marketo. Créez des tâches à partir de Marketo et utilisez des déclencheurs d’activité et des filtres dans les campagnes intelligentes.
title: Synchronisation SFDC - Synchronisation des activités
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/N-pw1q0NXaJGKW1J1R4iqhgXhA42sX5nP0OWPXCuaBc'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 6%
---
# Synchronisation SFDC : synchronisation des activités {#sfdc-sync-activity-sync}

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
