---
unique-page-id: 2953469
description: Synchronisation SFDC - Synchronisation Campaign - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation des campagnes
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 5%

---

# Synchronisation SFDC : synchronisation des campagnes {#sfdc-sync-campaign-sync}

Les programmes Marketo Engage peuvent être synchronisés avec les campagnes Salesforce. Voici un aperçu de son fonctionnement.

## Pourquoi synchroniser les programmes Marketo avec les campagnes Salesforce ? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilisez les puissantes fonctionnalités d’un programme Marketo.
* Maintenez les membres et leur état synchronisés entre un programme Marketo et une campagne Salesforce.
* Appuyez sur les fonctionnalités de création de rapports dans Marketo et Salesforce.

## Comment synchronise un programme Marketo et une campagne Salesforce ? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

Dans Marketo, vous avez la possibilité de créer un mapping un-à-un entre un programme et une campagne Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

Le **[canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}** et le **[coût par période](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md){target="_blank"}** dans Marketo se synchronisent avec Salesforce en tant que **type de campagne** et **coût réel**. Cette synchronisation est **d’une manière**, de Marketo à Salesforce.

Les **membres du programme Marketo** et leurs **[états de progression](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}** sont synchronisés avec les **membres de campagne Salesforce** et les **états des membres de campagne**. Il s’agit d’une **synchronisation bidirectionnelle**. Toute modification apportée dans Marketo ou Salesforce est donc répercutée dans les deux systèmes.

>[!NOTE]
>
>Si des membres du programme Marketo n’existent pas dans Salesforce, Marketo crée ces personnes en tant que prospects dans Salesforce.

## Quels sont les déclencheurs/filtres liés aux campagnes ? {#what-are-the-triggers-filters-related-to-campaigns}

Déclencheurs :

* Ajouté à la campagne SFDC
* Supprimé de la campagne SFDC
* Modification du statut dans la campagne SFDC

Filtres:

* Membre de la campagne SFDC

## Puis-je ajouter des personnes Marketo à ma campagne SFDC ? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Oui, utilisez l’action [Ajouter à l’action de flux de campagne SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md){target="_blank"}. Si cette personne n’existe pas dans Salesforce, Marketo la crée dans Salesforce, puis l’ajoute à la campagne.

## Puis-je supprimer des membres de ma campagne SFDC à l’aide de Marketo ? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Oui, utilisez l’action [Supprimer de l’action de flux de campagne SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## Puis-je modifier le statut des membres de la campagne à l’aide de Marketo ? {#can-i-change-campaign-member-status-using-marketo}

Oui, utilisez l’action [Modifier l’état dans le flux de campagne SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## Pourquoi ne puis-je voir aucune de mes campagnes Salesforce ? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Vous pouvez vérifier les éléments suivants :

1. Assurez-vous que la [synchronisation de campagne est activée](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
1. Confirmez que votre [utilisateur de synchronisation de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} est un [utilisateur marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} dans Salesforce.

>[!NOTE]
>
>Si votre campagne Salesforce et le programme Marketo mappé ont des statuts de programme incompatibles, vous pouvez recevoir un message d’erreur. Nous vous recommandons de [correspondre aux états du programme avant la synchronisation](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Synchroniser une campagne SFDC avec un programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Comprendre l’appartenance au programme](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Activer/Désactiver la synchronisation de campagne](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Faire de l’utilisateur de synchronisation Marketo un utilisateur marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
