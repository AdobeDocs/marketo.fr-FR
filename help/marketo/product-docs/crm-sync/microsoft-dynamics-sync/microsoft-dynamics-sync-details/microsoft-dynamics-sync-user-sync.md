---
unique-page-id: 3571840
description: Synchronisation Microsoft Dynamics - Synchronisation des utilisateurs - Documents Marketo - Documentation du produit
title: Synchronisation Microsoft Dynamics - Synchronisation des utilisateurs
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Synchronisation Microsoft Dynamics : synchronisation des utilisateurs {#microsoft-dynamics-sync-user-sync}

Saviez-vous que Marketo Engage synchronise entièrement votre base de données avec Dynamics ? Il se synchronise, puis attend 5 minutes et se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les comptes Dynamics.

Vous aurez besoin d’un utilisateur CRM Microsoft Dynamics dédié aux fins de l’intégration. Nous appelons cet utilisateur l’utilisateur de synchronisation.

## Comment les informations utilisateur sont-elles synchronisées entre les deux systèmes ? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La synchronisation des utilisateurs est un moyen : Dynamics vers Marketo. Si vous apportez des modifications à un utilisateur dans Dynamics, les modifications seront répercutées dans Marketo.

## Puis-je créer un utilisateur à l’aide de Marketo ? {#can-i-create-an-user-using-marketo}

Nombre Marketo ne peut pas créer d’utilisateurs dans Dynamics.

## Quels champs seront synchronisés avec Marketo ? {#which-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} lors de la configuration. Mais Marketo synchronise uniquement les champs auxquels votre utilisateur de synchronisation Dynamics a accès.
