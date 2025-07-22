---
unique-page-id: 3571836
description: Synchronisation de Microsoft Dynamics - Synchronisation de compte - Documents Marketo - Documentation du produit
title: Synchronisation de Microsoft Dynamics - Synchronisation des comptes
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Synchronisation des [!DNL Microsoft Dynamics] : synchronisation des comptes {#microsoft-dynamics-sync-account-sync}

Saviez-vous que Marketo synchronise l’ensemble de votre base de données avec [!DNL Dynamics] ? Il se synchronise, puis attend 5 minutes, puis se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les comptes [!DNL Dynamics].

## De quelle manière les informations sont-elles synchronisées ? {#which-way-does-the-information-sync}

Un seul moyen : de [!DNL Dynamics] à Marketo.

## Comment fonctionnent les mises à jour ? {#how-do-the-updates-work}

Si vous mettez à jour le champ Compte d’un contact dans Marketo, les valeurs de tous les contacts appartenant à ce compte dans Marketo sont modifiées. Il n’est pas synchronisé avec [!DNL Dynamics]. Cependant, la prochaine fois que ce compte sera mis à jour dans [!DNL Dynamics], les modifications remplaceront toutes les informations du compte dans Marketo.

## Puis-je créer un compte à l’aide de Marketo ? {#can-i-create-an-account-using-marketo}

Non. Marketo ne peut pas créer de comptes dans [!DNL Dynamics].

## Quels champs seront synchronisés avec Marketo ? {#which-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) lors de la configuration. Cependant, Marketo ne synchronise que les champs auxquels l’utilisateur de la synchronisation [!DNL Dynamics] a accès.

## Une modification apportée à un champ de compte dans [!DNL Dynamics] génère-t-elle un journal d’activité Modifier la valeur de données pour chaque contact ?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Surtout, oui. Cependant, si un compte comporte plus de 5 000 contacts et qu’un champ de ce compte change dans [!DNL Dynamics], nous synchronisons la modification, mais n’enregistrons pas l’activité pour plus de 5 000 contacts.
