---
unique-page-id: 2953463
description: Synchronisation de SFDC - Synchronisation prospect/propriétaire de compte - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation entre prospect et propriétaire de compte
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 13%

---

# Synchronisation SFDC : synchronisation entre prospect/propriétaire de compte {#sfdc-sync-lead-account-owner-sync}

Techniquement, il s’agit de la synchronisation de la table &quot;utilisateur&quot; dans Salesforce. Nous l’appelons toutefois champs de prospect/propriétaire de compte.

## Quels champs seront synchronisés avec Marketo Engage ? {#which-fields-will-sync-to-marketo-engage}

Pour chaque personne synchronisée dans Marketo, nous synchronisons également les champs de propriétaire suivants :

* Prénom du détenteur des ventes
* Nom du détenteur des ventes
* Titre du propriétaire des ventes
* Numéro de téléphone du détenteur des ventes
* Adresse e-mail du détenteur des ventes

Pour chaque contact, nous synchronisons les cinq champs de propriétaire de prospect ci-dessus ainsi que les champs de propriétaire de compte suivants :

* Prénom du détenteur du compte
* Nom du détenteur du compte
* Adresse e-mail du détenteur du compte

## Puis-je modifier le propriétaire de prospect dans Marketo ? {#can-i-change-the-lead-owner-in-marketo}

Absolument, utilisez simplement l’action de flux [Changer de propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}.

>[!NOTE]
>
>Vous ne pouvez pas modifier les informations du propriétaire à l’aide de la [page Détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## Que puis-je faire avec ces données ? {#what-can-i-do-with-this-data}

Il existe de nombreuses raisons d’utiliser ces données, telles que

* Envoyer un email personnalisé avec signature du propriétaire du commerce
* Filtrage sur des commerciaux spécifiques pour le marketing ou même l&#39;analyse de l&#39;efficacité
* Règles d’affectation (et de réaffectation) dans Marketo
* Utilisez-les dans les actions de flux [Changer de propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} et [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}.

Marketo dispose certainement d’une super synchronisation Salesforce. Personne d&#39;autre ne le fait si bien !
