---
unique-page-id: 2953463
description: Synchronisation SFDC - Sync responsable/propriétaire de compte - Documentation sur le marketing - Documentation du produit
title: Synchronisation SFDC - Synchronisation des prospects/propriétaires de comptes
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Synchronisation SFDC : Synchronisation des propriétaires de piste/compte {#sfdc-sync-lead-account-owner-sync}

Techniquement, il s&#39;agit de la synchronisation de la table &quot;utilisateur&quot; dans Salesforce. Cependant, nous l&#39;appellerons champs de responsable/propriétaire de compte.

## Quels champs seront synchronisés avec Marketo ? {#which-fields-will-sync-to-marketo}

Pour chaque personne synchronisée sur le marché, nous synchronisons également les champs de propriétaire suivants :

* Prénom du vendeur
* Nom du propriétaire commercial
* Titre du propriétaire commercial
* Numéro de téléphone du vendeur
* Adresse électronique du propriétaire des ventes

Pour chaque contact, nous synchronisons les cinq champs de propriétaire de prospect ci-dessus ainsi que les champs de propriétaire de compte suivants :

* Prénom du propriétaire du compte
* Nom du propriétaire du compte
* Adresse électronique du propriétaire du compte

## Puis-je modifier le propriétaire du prospect dans Marketo ? {#can-i-change-the-lead-owner-in-marketo}

Absolument, il vous suffit d’utiliser l’action de flux [Changer de propriétaire](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md).

>[!NOTE]
>
>Vous ne pouvez pas modifier les informations de propriétaire à l&#39;aide de la [page Détails de la personne](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Que puis-je faire avec ces données ? {#what-can-i-do-with-this-data}

Il existe de nombreuses raisons d’utiliser ces données, telles que

* Envoyer un e-mail personnalisé avec une signature du propriétaire des ventes
* Filtrage sur des commerciaux spécifiques pour le marketing ou même l&#39;analyse de l&#39;efficacité
* Règles d&#39;affectation (et de réaffectation) dans Marketo
* Utilisez-les dans les actions de flux [Modifier le propriétaire](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Synchroniser la personne avec SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) et [Créer une Tâche](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

Le marketing a une synchronisation Salesforce impressionnante. Personne d&#39;autre ne le fait si bien !
