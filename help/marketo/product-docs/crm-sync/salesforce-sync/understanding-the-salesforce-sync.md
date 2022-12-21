---
unique-page-id: 4719283
description: Présentation de la synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Présentation de la synchronisation Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 2%

---

# Présentation de la synchronisation Salesforce {#understanding-the-salesforce-sync}

Marketo et Salesforce vont ensemble comme des pois et des carottes. Vos données de vente et marketing sont synchronisées.

## Fonctionnement de la synchronisation {#how-sync-works}

Marketo se synchronise avec Salesforce toute la journée, tous les jours. Chaque synchronisation prend un certain temps, puis s’interrompt pendant 5 minutes, puis recommence.

>[!NOTE]
>
>La toute première synchronisation de votre abonnement peut prendre des heures, voire des jours, car Marketo copie l’intégralité de la base de données à partir de Salesforce. Ensuite, chaque synchronisation prend généralement quelques secondes ou minutes et synchronise uniquement les données qui ont changé.

![](assets/sync-illustration.png)

La synchronisation entre Salesforce et Marketo est bidirectionnelle uniquement pour les prospects, les contacts et les campagnes Salesforce. Dans ce cas, chaque fois que vous apportez des modifications dans Salesforce ou Marketo, vos mises à jour seront répercutées dans les deux systèmes. Toutes les autres synchronisations vont de Salesforce à Marketo uniquement. Cliquez sur les liens ci-dessous pour plus de détails sur chacun d’eux.

## Qu’est-ce qui est synchronisé entre Marketo et Salesforce ? {#what-is-synced-between-marketo-and-salesforce}

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
>Le [informations d’identification que vous saisissez dans Marketo pour Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

La synchronisation Marketo avec Salesforce est la plus puissante du monde. C&#39;est comme de la magie. une modification est apportée et l’autre système sera bientôt à jour.
