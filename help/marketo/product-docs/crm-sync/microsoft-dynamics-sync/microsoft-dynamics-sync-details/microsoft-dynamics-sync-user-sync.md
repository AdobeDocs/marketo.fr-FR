---
unique-page-id: 3571840
description: Microsoft [!DNL Dynamics] Sync - Synchronisation Des Utilisateurs - Documents Marketo - Documentation Du Produit
title: Microsoft [!DNL Dynamics] Sync - Synchronisation des utilisateurs
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Microsoft [!DNL Dynamics] Sync : synchronisation des utilisateurs {#microsoft-dynamics-sync-user-sync}

Saviez-vous que Marketo synchronise l’ensemble de votre base de données avec [!DNL Dynamics] ? Il se synchronise, puis attend 5 minutes, puis se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les comptes [!DNL Dynamics].

Vous aurez besoin d’un utilisateur Microsoft [!DNL Dynamics] CRM dédié aux fins de l’intégration. Nous appelons cet utilisateur l’utilisateur de synchronisation.

## Comment les informations de l’utilisateur sont-elles synchronisées entre les deux systèmes ? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La synchronisation des utilisateurs ne fonctionne que dans un sens : [!DNL Dynamics] à Marketo. Si vous apportez des modifications à un utilisateur dans [!DNL Dynamics], elles seront répercutées dans Marketo.

## Puis-je créer un utilisateur à l’aide de Marketo ? {#can-i-create-an-user-using-marketo}

Non. Marketo ne peut pas créer d’utilisateurs dans [!DNL Dynamics].

## Quels champs seront synchronisés avec Marketo ? {#which-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) lors de la configuration. Cependant, Marketo ne synchronise que les champs auxquels l’utilisateur de la synchronisation [!DNL Dynamics] a accès.
