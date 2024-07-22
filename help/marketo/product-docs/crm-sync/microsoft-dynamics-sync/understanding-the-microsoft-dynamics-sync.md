---
unique-page-id: 10098625
description: Présentation de la synchronisation Microsoft Dynamics - Documents Marketo - Documentation du produit
title: Présentation de la synchronisation Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 2%

---

# Présentation de la synchronisation Microsoft Dynamics {#understanding-the-microsoft-dynamics-sync}

Marketo Engage et Microsoft Dynamics vont ensemble. Vos données de vente et marketing sont synchronisées.

>[!NOTE]
>
>Marketo ne prend en charge que les certificats SSL compatibles avec Java 7 pour le moment.

>[!CAUTION]
>
>Actuellement, nous ne prenons pas en charge l’actualisation des environnements de test pour la synchronisation Marketo Dynamics. Si vous devez actualiser votre environnement de test Dynamics CRM, un nouvel environnement de test Marketo est requis. Pour plus d’informations, contactez l’équipe du compte d’Adobe (votre gestionnaire de compte).

## Fonctionnement de la synchronisation {#how-sync-works}

Marketo synchronise en permanence les données avec Microsoft Dynamics toute la journée, tous les jours. Elle est effectuée en utilisant la synchronisation en arrière-plan, par lots, et non en temps réel.

>[!NOTE]
>
>La toute première synchronisation de votre abonnement prend des minutes à des heures, selon la taille de votre base de données. Marketo copie la base de données entière de Dynamics. Ensuite, chaque synchronisation prend généralement quelques secondes ou minutes et synchronise uniquement les données qui ont changé.

La synchronisation entre Marketo et Dynamics est bidirectionnelle pour les pistes et les contacts. Si vous apportez des modifications dans Marketo ou Dynamics, vos mises à jour seront répercutées dans les deux systèmes. Tous les autres champs, tels que les comptes et les opportunités, sont synchronisés d’une seule manière, de Dynamics à Marketo.

## Qu’est-ce qui est synchronisé entre Marketo et Microsoft Dynamics ? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Prospects](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contacts](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Comptes](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Utilisateurs et utilisatrices](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Équipes (groupes d’utilisateurs système)
* [Opportunités](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entités personnalisées](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

Les [informations d’identification que vous saisissez dans Marketo pour Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) sont utilisées pour synchroniser les données.

>[!NOTE]
>
>La copie d’instance n’est pas prise en charge si l’instance source est intégrée à Microsoft Dynamics.
