---
unique-page-id: 4719283
description: Présentation de la synchronisation Salesforce - Documents marketing - Documentation du produit
title: Présentation de la synchronisation Salesforce
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '263'
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

* [Pistes](sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Contacts](sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Comptes](sfdc-sync-details/sfdc-sync-account-sync.md)
* [Utilisateurs](sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Opportunités](sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Campagnes Salesforce](sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Objets personnalisés](sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Activité](sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Les [informations d&#39;identification que vous saisissez dans Marketo pour Salesforce](setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

La synchronisation Salesforce comporte de nombreuses nuances et fonctionnalités. Consultez les détails dans la section [Détails de la synchronisation SFDC](http://docs.marketo.com/display/docs/sfdc+sync+details).

>[!MORELIKETHIS]
>
>* [Configuration de la synchronisation Salesforce](http://docs.marketo.com/display/docs/setup)
>* [Détails de la synchronisation SFDC](http://docs.marketo.com/display/docs/sfdc+sync+details)

>



La synchronisation de Marketo avec Salesforce est la plus puissante du monde. C&#39;est comme de la magie - un changement est fait et l&#39;autre système est bientôt à jour.