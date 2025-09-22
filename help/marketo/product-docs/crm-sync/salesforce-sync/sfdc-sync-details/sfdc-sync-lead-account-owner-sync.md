---
unique-page-id: 2953463
description: Synchronisation de SFDC - Synchronisation des prospects/propriétaires de compte - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - Synchronisation des prospects et des propriétaires de compte
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 16%

---

# Synchronisation SFDC : synchronisation du lead/de l’entité propriétaire du compte {#sfdc-sync-lead-account-owner-sync}

Techniquement, ils synchronisent la table « utilisateur » dans [!DNL Salesforce], mais nous l’appellerons champs de prospect/propriétaire de compte.

## Quels champs seront synchronisés avec Marketo Engage ? {#which-fields-will-sync-to-marketo-engage}

Pour chaque personne synchronisée dans Marketo, nous synchronisons également les champs de propriétaire suivants :

* Prénom du détenteur des ventes
* Nom du détenteur des ventes
* Titre du propriétaire des ventes
* Numéro de téléphone du détenteur des ventes
* Adresse e-mail du détenteur des ventes

Pour chaque contact, nous synchronisons les cinq champs de propriétaire du prospect ci-dessus, ainsi que ces champs de propriétaire de compte :

* Prénom du détenteur du compte
* Nom du détenteur du compte
* Adresse e-mail du détenteur du compte

## Puis-je changer le propriétaire du prospect dans Marketo ? {#can-i-change-the-lead-owner-in-marketo}

Absolument, utilisez simplement l’action de flux [Modifier le propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}.

>[!NOTE]
>
>Vous ne pouvez pas modifier les informations sur le propriétaire à l’aide de la page [Utilisation des détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## Que puis-je faire avec ces données ? {#what-can-i-do-with-this-data}

Il existe de nombreuses raisons d’utiliser ces données, par exemple :

* Envoyer un e-mail personnalisé avec la signature du commercial
* Filtrez des représentants commerciaux spécifiques pour le marketing ou même l’analyse de l’efficacité.
* Règles d’affectation (et de réaffectation) dans Marketo
* Utilisez-les dans les actions de flux [Modifier le propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} et [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}

Marketo a vraiment une synchronisation [!DNL Salesforce] impressionnante. Personne d&#39;autre ne le fait aussi bien !
