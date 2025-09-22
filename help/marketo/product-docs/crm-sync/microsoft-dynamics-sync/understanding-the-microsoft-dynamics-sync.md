---
unique-page-id: 10098625
description: Présentation de la synchronisation  [!DNL Microsoft Dynamics]  documents Marketo - Documentation du produit
title: Présentation de la synchronisation Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 4%

---

# Comprendre la synchronisation des [!DNL Microsoft Dynamics] {#understanding-the-microsoft-dynamics-sync}

Marketo et [!DNL Microsoft Dynamics] vont de pair. Nous gardons vos données de vente et de marketing synchronisées.

>[!CAUTION]
>
>Nous ne prenons actuellement pas en charge l’actualisation du sandbox pour la synchronisation [!DNL Marketo Dynamics]. Si vous devez actualiser votre sandbox CRM [!DNL Dynamics], un nouveau sandbox Marketo sera requis. Contactez votre responsable du succès client pour plus d’informations.

## Fonctionnement de la synchronisation {#how-sync-works}

Marketo synchronise les données avec [!DNL Microsoft Dynamics] en permanence, tous les jours et toute la journée. Cela s’effectue à l’aide de la synchronisation en arrière-plan, par lots, et non en temps réel.

>[!NOTE]
>
>La toute première synchronisation de votre abonnement prend de quelques minutes à quelques heures, selon la taille de votre base de données. Marketo copie l’intégralité de la base de données depuis [!DNL Dynamics]. Ensuite, chaque synchronisation prend généralement des secondes ou des minutes et synchronise uniquement les données qui ont été modifiées.

La synchronisation entre Marketo et [!DNL Dynamics] est bidirectionnelle pour les prospects et les contacts. Si vous apportez des modifications dans Marketo ou [!DNL Dynamics], vos mises à jour seront répercutées sur les deux systèmes. Tous les autres champs, tels que les comptes et les opportunités, sont synchronisés dans un seul sens, de [!DNL Dynamics] à Marketo.

## Qu’est-ce que Synchronisé entre Marketo et [!DNL Microsoft Dynamics] ? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Prospects](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contacts](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Comptes](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Utilisateurs et utilisatrices](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Équipes (groupes d’utilisateurs système)
* [Opportunités](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entités personnalisées](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

Les [ informations d’identification que vous saisissez dans Marketo pour  [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) sont utilisées pour synchroniser les données.

>[!NOTE]
>
>La copie d’instance n’est pas prise en charge si l’instance source est intégrée à [!DNL Microsoft Dynamics].
