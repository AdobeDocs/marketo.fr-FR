---
unique-page-id: 4719283
description: Présentation de la synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Présentation de la synchronisation Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 2%

---

# Présentation de la synchronisation Salesforce {#understanding-the-salesforce-sync}

Marketo Engage et Salesforce vont ensemble comme des pois et des carottes. Vos données de vente et marketing sont synchronisées.

## Fonctionnement de la synchronisation {#how-sync-works}

Marketo se synchronise avec Salesforce toute la journée, tous les jours. Chaque synchronisation prend un certain temps, puis s’interrompt pendant 5 minutes, puis recommence.

>[!NOTE]
>
>La toute première synchronisation de votre abonnement peut prendre des heures, voire des jours, car Marketo copie l’intégralité de la base de données depuis Salesforce. Ensuite, chaque synchronisation prend généralement quelques secondes ou minutes et synchronise uniquement les données qui ont changé.

![](assets/sync-illustration.png)

La synchronisation entre Salesforce et Marketo est bidirectionnelle uniquement pour les prospects, les contacts et les campagnes Salesforce. Dans ce cas, chaque fois que vous apportez des modifications dans Salesforce ou Marketo, vos mises à jour seront répercutées dans les deux systèmes. Toutes les autres synchronisations vont de Salesforce à Marketo uniquement. Cliquez sur les liens ci-dessous pour plus de détails sur chacun d’eux.

## Qu’est-ce qui est synchronisé entre Marketo et Salesforce ? {#what-is-synced-between-marketo-and-salesforce}

* [Prospects](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [Contacts](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [Comptes](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [Utilisateurs et utilisatrices](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [Opportunités](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Campagnes Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [Objets personnalisés](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [Activité](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>La variable [informations d’identification saisies dans Marketo pour Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

La synchronisation Marketo avec Salesforce est la plus puissante du monde. C&#39;est magique, un changement est fait et l&#39;autre système est bientôt à jour.
