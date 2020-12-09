---
unique-page-id: 10098625
description: Présentation de Microsoft Dynamics Sync - Documents marketing - Documentation du produit
title: Présentation de Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Présentation de Microsoft Dynamics Sync {#understanding-the-microsoft-dynamics-sync}

Marketo et Microsoft Dynamics vont de pair. Vos données de vente et de marketing sont synchronisées.

>[!NOTE]
>
>Actuellement, Marketo ne prend en charge que les certificats SSL compatibles avec Java 7.

## Fonctionnement de la synchronisation {#how-sync-works}

Marketo synchronise continuellement les données avec Microsoft Dynamics toute la journée, tous les jours. Il est fait en utilisant la synchronisation en arrière-plan, par lots, pas en temps réel.

>[!NOTE]
>
>La toute première synchronisation dans votre abonnement prend des minutes à des heures, selon la taille de votre base de données. Marketo copie la base de données entière de Dynamics. Ensuite, chaque synchronisation prend généralement des secondes ou des minutes et synchronise uniquement les données qui ont changé.

La synchronisation entre Marketo et Dynamics est bidirectionnelle pour les pistes et les contacts. Si vous apportez des modifications dans Marketing ou Dynamics, vos mises à jour seront répercutées dans les deux systèmes. Tous les autres champs, tels que les comptes et les opportunités, sont synchronisés d&#39;une manière unique, de Dynamics à Marketo.

## Qu&#39;est-ce qui est synchronisé entre Marketo et Microsoft Dynamics ? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Pistes](microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contacts](microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Comptes](microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Utilisateurs](microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Équipes (groupes d&#39;utilisateurs système)
* [Opportunités](microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entités personnalisées](microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>Les [informations d&#39;identification que vous saisissez dans Marketo pour Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) sont utilisées pour synchroniser les données.

Dynamics sync comporte de nombreuses nuances et fonctionnalités. Consultez les détails dans la section [Détails de](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)Microsoft Dynamics Sync.

>[!CAUTION]
>
>Actuellement, nous ne prenons pas en charge l&#39;actualisation de sandbox pour Marketing Dynamics Sync. Si vous devez actualiser votre sandbox Dynamics CRM, un nouveau sandbox Marketo sera nécessaire. Pour plus d’informations, contactez votre responsable de succès client.

>[!MORELIKETHIS]
>
>* [Configuration de la synchronisation](http://docs.marketo.com/display/docs/sync+setup)
   >
   >
* [Détails de Microsoft Dynamics Sync](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)

