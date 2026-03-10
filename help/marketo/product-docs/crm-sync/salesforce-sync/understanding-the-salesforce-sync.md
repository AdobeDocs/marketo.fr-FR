---
unique-page-id: 4719283
description: Découvrez comment la synchronisation Salesforce maintient les données Marketo et Salesforce synchronisées. Découvrez ce qui est synchronisé et comment fonctionne la synchronisation bidirectionnelle pour les prospects et les contacts.
title: Présentation de la synchronisation Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 89%

---

# Présentation de la synchronisation [!DNL Salesforce] {#understanding-the-salesforce-sync}

Marketo Engage et Salesforce fonctionnent très bien ensemble. Nous maintenons vos données de vente et de marketing synchronisées.

## Fonctionnement de la synchronisation {#how-sync-works}

Marketo se synchronise avec [!DNL Salesforce] toute la journée, tous les jours. Chaque synchronisation prend du temps, s’interrompt pendant 5 minutes, puis redémarre.

>[!NOTE]
>
>La toute première synchronisation de votre abonnement peut prendre des heures, voire des jours, car Marketo copie l’intégralité de la base de données depuis [!DNL Salesforce]. Ensuite, chaque synchronisation prend généralement quelques secondes ou quelques minutes et synchronise uniquement les données qui ont été modifiées.

![](assets/sync-illustration.png)

La synchronisation entre [!DNL Salesforce] et Marketo est bidirectionnelle uniquement pour les prospects, les contacts et les campagnes [!DNL Salesforce]. Dans ces cas, chaque fois que vous apportez des modifications à [!DNL Salesforce] ou à Marketo, vos mises à jour sont répercutées sur les deux systèmes. Toutes les autres synchronisations vont de [!DNL Salesforce] vers Marketo uniquement. Cliquez sur les liens ci-dessous pour avoir plus de détails sur chaque élément.

## Quel contenu est synchronisé entre Marketo et [!DNL Salesforce] ? {#what-is-synced-between-marketo-and-salesforce}

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
>Les [informations d’identification que vous saisissez dans Marketo pour Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

La synchronisation de Marketo avec [!DNL Salesforce] est la plus puissante de ce type. On dirait de la magie : une modification est apportée et l’autre système est rapidement mis à jour.
