---
unique-page-id: 4719283
description: Présentation de la synchronisation Salesforce - Documentation de Marketo - Documentation du produit
title: Présentation de la synchronisation avec Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# Comprendre la synchronisation des [!DNL Salesforce] {#understanding-the-salesforce-sync}

Marketo Engage et Salesforce vont de pair comme des petits pois et des carottes. Nous gardons vos données de vente et de marketing synchronisées.

## Fonctionnement de la synchronisation {#how-sync-works}

Marketo se synchronise avec [!DNL Salesforce] toute la journée, tous les jours. Chaque synchronisation prend du temps, s’interrompt pendant 5 minutes, puis redémarre.

>[!NOTE]
>
>La toute première synchronisation de votre abonnement peut prendre des heures, voire des jours, car Marketo copie l’intégralité de la base de données depuis [!DNL Salesforce]. Ensuite, chaque synchronisation prend généralement des secondes ou des minutes et synchronise uniquement les données qui ont été modifiées.

![](assets/sync-illustration.png)

La synchronisation entre [!DNL Salesforce] et Marketo est bidirectionnelle uniquement pour les prospects, les contacts et les campagnes [!DNL Salesforce]. Dans ces cas, chaque fois que vous apportez des modifications à [!DNL Salesforce] ou à Marketo, vos mises à jour sont répercutées sur les deux systèmes. Toutes les autres synchronisations vont de [!DNL Salesforce] à Marketo uniquement. Cliquez sur les liens ci-dessous pour plus de détails sur chacun d’eux.

## Qu’est-ce que Synchronisé entre Marketo et [!DNL Salesforce] ? {#what-is-synced-between-marketo-and-salesforce}

* [Leads](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [Contacts](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [Comptes](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [Utilisateurs](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [&#x200B; Opportunités &#x200B;](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Campagnes Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [Objets personnalisés &#x200B;](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [&#x200B; Activité &#x200B;](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>Les [informations d’identification que vous saisissez dans Marketo pour Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

La synchronisation de Marketo avec [!DNL Salesforce] est la plus puissante de ce type au monde. C&#39;est comme de la magie : un changement est fait et l&#39;autre système est bientôt à jour.
