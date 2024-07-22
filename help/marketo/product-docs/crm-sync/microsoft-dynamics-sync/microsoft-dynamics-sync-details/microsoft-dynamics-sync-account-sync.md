---
unique-page-id: 3571836
description: Synchronisation Microsoft Dynamics - Synchronisation des comptes - Documents Marketo - Documentation du produit
title: Synchronisation Microsoft Dynamics - Synchronisation des comptes
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Synchronisation Microsoft Dynamics : synchronisation des comptes {#microsoft-dynamics-sync-account-sync}

Saviez-vous que Marketo Engage synchronise entièrement votre base de données avec Dynamics ? Il se synchronise, puis attend 5 minutes et se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les comptes Dynamics.

## De quelle manière les informations se synchronisent-elles ? {#which-way-does-the-information-sync}

Une seule méthode : de Dynamics à Marketo.

## Comment fonctionnent les mises à jour ? {#how-do-the-updates-work}

Si vous mettez à jour un champ Compte pour un contact dans Marketo, cela modifie les valeurs de tous les contacts appartenant à ce compte dans Marketo. Il ne se synchronise pas avec Dynamics. Cependant, la prochaine fois que ce compte sera mis à jour dans Dynamics, les modifications remplaceront toutes les informations de compte dans Marketo.

## Puis-je créer un compte à l’aide de Marketo ? {#can-i-create-an-account-using-marketo}

Nombre Marketo ne peut pas créer de comptes dans Dynamics.

## Quels champs seront synchronisés avec Marketo ? {#which-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} lors de la configuration. Mais Marketo synchronise uniquement les champs auxquels votre utilisateur de synchronisation Dynamics a accès.

## Une modification d’un champ de compte dans Dynamics entraîne-t-elle un journal d’activité de modification de la valeur de données pour chaque contact ?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Surtout, oui. Cependant, si un compte comporte plus de 5 000 contacts et un champ sur ce compte change dans Dynamics, nous synchronisons la modification mais ne consignons pas l’activité pour plus de 5 000 contacts.
