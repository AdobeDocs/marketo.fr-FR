---
unique-page-id: 3571836
description: Microsoft Dynamics Sync - Synchronisation des comptes - Documents marketing - Documentation du produit
title: Microsoft Dynamics Sync -Synchronisation des comptes
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---


# Microsoft Dynamics Sync : Synchronisation du compte {#microsoft-dynamics-sync-account-sync}

Saviez-vous que Marketo synchronise votre base de données complète avec Dynamics ? Il se synchronise, puis attend 5 minutes puis se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la façon dont Marketo traite spécifiquement les comptes Dynamics.

## De quelle façon les informations sont-elles synchronisées ? {#which-way-does-the-information-sync}

Un seul moyen : de Dynamics à Marketo.

## Comment fonctionnent les mises à jour ? {#how-do-the-updates-work}

Si vous mettez à jour un champ Compte pour un contact dans Marketo, il modifie les valeurs de tous les contacts appartenant à ce compte dans Marketo. Il n&#39;est pas synchronisé avec Dynamics. Cependant, la prochaine fois que ce compte sera mis à jour dans Dynamics, les modifications remplaceront toutes les informations de compte dans Marketing.

## Puis-je créer un compte à l’aide de Marketo ? {#can-i-create-an-account-using-marketo}

Non. Marketo ne peut pas créer de comptes dans Dynamics.

## Quels champs seront synchronisés avec Marketo ? {#which-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) pendant la configuration. Mais Marketo synchronise uniquement les champs auxquels votre utilisateur Dynamics sync a accès.

## Est-ce qu&#39;une modification d&#39;un champ de compte dans Dynamics génère un journal d&#39;Activité des valeurs de données de modification pour chaque contact ?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Surtout, oui. Cependant, si un compte a plus de 5 000 contacts et qu&#39;un champ sur ce compte change dans Dynamics, nous synchronisons la modification mais ne consignons pas l&#39;activité pour les 5 000 contacts et plus.
