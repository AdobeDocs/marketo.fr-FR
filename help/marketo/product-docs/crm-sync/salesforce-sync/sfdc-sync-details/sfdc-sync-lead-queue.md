---
unique-page-id: 7516241
description: Synchronisation SFDC - File d’attente des pistes - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - File d’attente des pistes
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 15%

---

# Synchronisation SFDC : File d’attente des pistes {#sfdc-sync-lead-queue}

Marketo vous permet d’ajouter des personnes à [Files d’attente de prospect Salesforce](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) pour faciliter la distribution des pistes. Voici les détails.

## Comment affecter une personne à une file d’attente dans Marketo ? {#how-to-assign-a-person-to-a-queue-in-marketo}

Vous pouvez affecter une personne à une file d’attente de prospect Salesforce à l’aide de l’une des actions de flux suivantes :

* [Synchroniser individu dans SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Modifier détenteur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Vous ne pouvez pas créer ni modifier de files d’attente dans Marketo.

## Comment les informations du propriétaire de prospect sont-elles stockées si la personne appartient à une file d’attente ? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Si une piste est détenue par une file d’attente dans Salesforce, ces champs du propriétaire des ventes sont vides jusqu’à ce que la piste soit assignée à un propriétaire.

* Prénom du détenteur des ventes
* Nom du détenteur des ventes
* Titre du propriétaire des ventes
* Numéro de téléphone du détenteur des ventes
* Adresse e-mail du détenteur des ventes
