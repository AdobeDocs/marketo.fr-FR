---
unique-page-id: 4719283
description: Présentation de la synchronisation Salesforce - Documents marketing - Documentation du produit
title: Présentation de la synchronisation Salesforce
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

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

## Qu’est-ce qui est synchronisé entre Marketo et Salesforce ? {#what-is-synced-between-marketo-and-salesforce}

* [Pistes](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Contacts](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Comptes](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [Utilisateurs](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Opportunités](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Campagnes Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Objets personnalisés](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Activité](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Les [informations d&#39;identification que vous saisissez dans Marketo pour Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

La synchronisation de Marketo avec Salesforce est la plus puissante du monde. On se sent magique. un changement est apporté et l&#39;autre système est bientôt à jour.
