---
unique-page-id: 4719283
description: Présentation de la synchronisation Salesforce - Marketo Docs - Documentation du produit
title: Présentation de la synchronisation Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 2%

---

# Présentation de la synchronisation Salesforce {#understanding-the-salesforce-sync}

Marketo et Salesforce vont ensemble comme des pois et des carottes. Vos données de vente et de marketing sont synchronisées.

## Fonctionnement de la synchronisation {#how-sync-works}

Marketo se synchronise avec Salesforce toute la journée, tous les jours. Chaque synchronisation prend un certain temps, puis s’interrompt pendant 5 minutes, puis revient en début.

>[!NOTE]
>
>La toute première synchronisation dans votre abonnement peut prendre des heures, voire des jours, parce que Marketo copie la base de données entière depuis Salesforce. Ensuite, chaque synchronisation prend généralement des secondes ou des minutes et synchronise uniquement les données qui ont changé.

![](assets/sync-illustration.png)

La synchronisation entre Salesforce et Marketo est bidirectionnelle uniquement pour les pistes, les contacts et les campagnes Salesforce. Dans ce cas, chaque fois que vous apportez des modifications dans Salesforce ou Marketo, vos mises à jour seront répercutées dans les deux systèmes. Toutes les autres synchronisations vont de Salesforce à Marketo uniquement. Cliquez sur les liens ci-dessous pour plus de détails sur chacun d&#39;eux.

## Qu’est-ce que la synchronisation entre Marketo et Salesforce ? {#what-is-synced-between-marketo-and-salesforce}

* [Prospects](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Contacts](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Comptes](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [Utilisateurs](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Opportunités](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Campagnes Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Objets personnalisés](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Activité](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Les [informations d’identification que vous saisissez dans Marketo pour Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

Le Marketo sync avec Salesforce est le plus puissant du genre au monde. On se sent magique. un changement est apporté et l&#39;autre système est bientôt à jour.
