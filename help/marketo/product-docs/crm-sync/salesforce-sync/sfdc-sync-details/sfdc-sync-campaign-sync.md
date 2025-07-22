---
unique-page-id: 2953469
description: Synchronisation de SFDC - Synchronisation de Campaign - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - Synchronisation de la campagne
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 5%

---

# Synchronisation de SFDC : synchronisation de la campagne {#sfdc-sync-campaign-sync}

Les programmes Marketo peuvent être synchronisés avec les campagnes [!DNL Salesforce]. Voici un aperçu de son fonctionnement.

## Pourquoi synchroniser les programmes Marketo avec les campagnes [!DNL Salesforce] ? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Utilisez les puissantes fonctionnalités d’un programme Marketo.
* Gardez les membres et leur statut synchronisés entre un programme Marketo et une campagne [!DNL Salesforce].
* Accédez aux fonctions de création de rapports de Marketo et [!DNL Salesforce].

## Comment un programme Marketo et une campagne [!DNL Salesforce] sont-ils synchronisés ? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

Dans Marketo, vous avez la possibilité de créer un mapping un-à-un entre un programme et une campagne [!DNL Salesforce].

![](assets/image2015-7-8-9-3a43-3a8.png)

Le **[canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** et le **[coût de la période](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** dans la synchronisation Marketo à [!DNL Salesforce] que le **type de campagne** et le **coût réel**. Cette synchronisation s’effectue **dans un sens**, de Marketo à [!DNL Salesforce].

Marketo **membres du programme** et leurs **[états de progression](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** sont synchronisés avec les **[!DNL Salesforce]membres de campagne** et **états des membres de campagne**. Il s’agit d’une **synchronisation bidirectionnelle**, de sorte que toute modification apportée à Marketo ou à [!DNL Salesforce] est répercutée sur les deux systèmes.

>[!NOTE]
>
>S’il existe des membres dans le programme Marketo qui n’existent pas dans [!DNL Salesforce], Marketo les transforme en prospects dans [!DNL Salesforce].

## Quels sont les déclencheurs/filtres liés aux campagnes ? {#what-are-the-triggers-filters-related-to-campaigns}

Déclencheurs :

* Ajouté à la campagne SFDC
* Supprimé de la campagne SFDC
* Modification du statut dans la campagne SFDC

Filtres:

* Membre de la campagne SFDC

## Puis-je ajouter des personnes Marketo à ma campagne SFDC ? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Oui, utiliser l’action de flux de campagne [ Ajouter à SFDC ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Si cette personne n’existe pas dans [!DNL Salesforce], Marketo la créera dans [!DNL Salesforce] puis l’ajoutera à la campagne.

## Puis-je supprimer des membres de ma campagne SFDC à l’aide de Marketo ? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Oui, utiliser l’action de flux [ Supprimer de SFDC Campaign ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## Puis-je modifier le statut de membre de la campagne à l’aide de Marketo ? {#can-i-change-campaign-member-status-using-marketo}

Oui, utiliser l’action de flux [ Modifier le statut dans SFDC Campaign ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## Pourquoi est-ce que je ne vois aucune de mes campagnes [!DNL Salesforce] ? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Voici ce que vous pouvez vérifier :

1. Assurez-vous que la [synchronisation de la campagne est activée](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Vérifiez que votre [utilisateur de synchronisation Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) est un [utilisateur marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) dans [!DNL Salesforce].

>[!NOTE]
>
>Si votre campagne [!DNL Salesforce] et le programme Marketo mappé ont des statuts de programme incompatibles, vous pouvez recevoir un message d’erreur. Nous vous recommandons de [faire correspondre les statuts du programme avant la synchronisation](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Synchroniser une campagne SFDC avec un programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Comprendre l’appartenance à un programme](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Activer/Désactiver La Synchronisation De La Campagne](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Faire de l’utilisateur de synchronisation Marketo un utilisateur marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
