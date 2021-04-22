---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - Synchronisation des utilisateurs - Documentation Marketo - Documentation du produit
title: Microsoft Dynamics Sync -Sync utilisateur
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Microsoft Dynamics Sync : Synchronisation utilisateur {#microsoft-dynamics-sync-user-sync}

Saviez-vous que Marketo synchronise votre base de données complète avec Dynamics ? Il se synchronise, puis attend 5 minutes puis se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la façon dont Marketo traite spécifiquement les comptes Dynamics.

Vous aurez besoin d&#39;un utilisateur dédié à Microsoft Dynamics CRM pour l&#39;intégration. Nous appelons cet utilisateur l&#39;utilisateur de synchronisation.

## Comment les détails des utilisateurs sont-ils synchronisés entre les deux systèmes ? {#how-are-user-details-kept-in-sync-between-the-two-systems}

La synchronisation de l&#39;utilisateur est un moyen : Dynamics to Marketo. Si vous apportez des modifications à un utilisateur dans Dynamics, les modifications seront répercutées dans Marketo.

## Puis-je créer un utilisateur à l’aide de Marketo ? {#can-i-create-an-user-using-marketo}

Nombre Marketo ne peut pas créer d&#39;utilisateurs dans Dynamics.

## Quels champs seront synchronisés avec Marketo ? {#which-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) pendant la configuration. Mais Marketo synchronise uniquement les champs auxquels votre utilisateur Dynamics sync a accès.
