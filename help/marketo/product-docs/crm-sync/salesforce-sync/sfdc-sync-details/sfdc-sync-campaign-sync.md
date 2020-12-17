---
unique-page-id: 2953469
description: Synchronisation SFDC - Campaign Sync - Documentation sur le marketing - Documentation sur le produit
title: Synchronisation SFDC - Campaign Sync
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---


# Synchronisation SFDC : Campaign Sync {#sfdc-sync-campaign-sync}

Les Programmes du marketing peuvent être synchronisés avec les campagnes Salesforce. Voici un aperçu de la façon dont cela fonctionne.

## Pourquoi synchroniser les programmes de marketing avec les campagnes Salesforce ? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilisez les puissantes fonctionnalités d&#39;un Programme de marketing.
* Maintenez les membres et leur statut synchronisés entre un programme Marketo et un Campaign Salesforce.
* Appuyez sur les fonctionnalités de rapports de Marketo et Salesforce.

## Comment synchroniser un Programme Marketo et une campagne Salesforce ? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

Dans Marketo, vous avez la possibilité de créer un mappage un-à-un entre un programme et une campagne Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

Le ** [canal](../../../../product-docs/administration/tags/create-a-program-channel.md) **et ** [coût de la période](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** dans Marketo se synchronise avec Salesforce en tant que **type de campagne** et **coût réel**. Cette synchronisation est **sens unique**, de Marketo à Salesforce.

Les membres du programme **Marketo** et leurs statuts de progression ** [](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** sont synchronisés avec les **membres de la campagne Salesforce** et **statues des membres de la campagne**. Il s’agit d’une **synchronisation bidirectionnelle** **synchronisée**, de sorte que toutes les modifications apportées dans Marketo ou Salesforce sont répercutées dans les deux systèmes.

>[!NOTE]
>
>S&#39;il y a des membres du programme Marketo qui n&#39;existent pas dans Salesforce, Marketo crée ces personnes comme pistes dans Salesforce.

## Quels sont les déclencheurs/filtres liés aux campagnes ? {#what-are-the-triggers-filters-related-to-campaigns}

Déclencheurs :

* Ajouté à SFDC Campaign
* Retrait de SFDC Campaign
* Etat modifié dans SFDC Campaign

Filtres :

* Membre de la DDC Campaign

## Puis-je ajouter des personnes du marketing à ma campagne SFDC ? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Oui, utilisez l&#39;action de flux de campagne [Ajouter à la FDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Si cette personne n’existe pas dans Salesforce, Marketo la crée dans Salesforce, puis l’ajoute à la campagne.

## Puis-je supprimer des membres de ma campagne SFDC à l’aide de Marketo ? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Oui, utilisez l’action de flux de Campaign [Supprimer de SFDC ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## Puis-je modifier l’état des membres de la campagne à l’aide de Marketing Cloud ? {#can-i-change-campaign-member-status-using-marketo}

Oui, utilisez l’action de flux Campaign [Modifier l’état dans SFDC ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## Pourquoi est-ce que je ne vois aucune de mes campagnes Salesforce ? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Vous pouvez vérifier les éléments suivants :

1. Assurez-vous que la synchronisation de campagne [est activée](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Vérifiez que votre [utilisateur de synchronisation du marketing](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) est un [utilisateur marketing](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) dans Salesforce.

>[!NOTE]
>
>Si votre campagne Salesforce et le programme Marketo mappé présentent des états de programme incompatibles, vous pouvez recevoir un message d’erreur. Nous vous recommandons de [faire correspondre les états du programme avant la synchronisation](sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Synchronisation d’une Campaign SFDC avec un Programme](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Comprendre l&#39;appartenance à un Programme](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Activer/désactiver la synchronisation Campaign](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Faire de Marketo Sync User un utilisateur Marketing](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

>



