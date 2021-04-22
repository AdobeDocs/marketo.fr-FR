---
unique-page-id: 2953463
description: Synchronisation SFDC - Synchronisation des prospects/propriétaires de comptes - Marketo Docs - Documentation du produit
title: Synchronisation SFDC - Synchronisation des prospects/propriétaires de comptes
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 13%

---

# Synchronisation SFDC : Synchronisation des propriétaires de piste/compte {#sfdc-sync-lead-account-owner-sync}

Techniquement, il s&#39;agit de la synchronisation de la table &quot;utilisateur&quot; dans Salesforce. Cependant, nous l&#39;appellerons champs de responsable/propriétaire de compte.

## Quels champs seront synchronisés avec Marketo ? {#which-fields-will-sync-to-marketo}

Pour chaque personne synchronisée sur Marketo, nous synchronisons également les champs de propriétaire suivants :

* Prénom du détenteur des ventes
* Nom du détenteur des ventes
* Titre du propriétaire commercial
* Numéro de téléphone du détenteur des ventes
* Adresse e-mail du détenteur des ventes

Pour chaque contact, nous synchronisons les cinq champs de propriétaire de prospect ci-dessus ainsi que les champs de propriétaire de compte suivants :

* Prénom du détenteur du compte
* Nom du détenteur du compte
* Adresse e-mail du détenteur du compte

## Puis-je changer le propriétaire principal à Marketo ? {#can-i-change-the-lead-owner-in-marketo}

Absolument, il vous suffit d’utiliser l’action de flux [Changer de propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md).

>[!NOTE]
>
>Vous ne pouvez pas modifier les informations de propriétaire à l&#39;aide de la [page Détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Que puis-je faire avec ces données ? {#what-can-i-do-with-this-data}

Il existe de nombreuses raisons d’utiliser ces données, telles que

* Envoyer un e-mail personnalisé avec une signature du propriétaire des ventes
* Filtrage sur des commerciaux spécifiques pour le marketing ou même l&#39;analyse de l&#39;efficacité
* Règles d’affectation (et de réaffectation) dans Marketo
* Utilisez-les dans les actions de flux [Modifier le propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) et [Créer une Tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

Marketo a une synchronisation Salesforce impressionnante. Personne d&#39;autre ne le fait si bien !
