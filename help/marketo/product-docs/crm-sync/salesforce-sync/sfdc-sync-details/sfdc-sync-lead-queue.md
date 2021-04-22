---
unique-page-id: 7516241
description: Synchronisation SFDC - File d’attente des pistes - Documentation Marketo - Documentation du produit
title: Synchronisation SFDC - File d’attente des pistes
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 15%

---

# Synchronisation SFDC : File d&#39;attente de piste {#sfdc-sync-lead-queue}

Marketo vous permet d&#39;ajouter des personnes à [files d&#39;attente de pistes Salesforce](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) pour faciliter la distribution de pistes. Voici les détails.

## Comment affecter une personne à une file d&#39;attente à Marketo ? {#how-to-assign-a-person-to-a-queue-in-marketo}

Vous pouvez affecter une personne à une file d&#39;attente de piste Salesforce à l&#39;aide de l&#39;une des actions de flux suivantes :

* [Synchroniser individu dans SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Modifier détenteur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Vous ne pouvez pas créer ni modifier de files d&#39;attente dans Marketo.

## Comment les informations de propriétaire de prospect sont-elles stockées si la personne appartient à une file d&#39;attente ? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Si une piste appartient à une file d&#39;attente dans Salesforce, ces champs de propriétaire commercial sont conservés vides jusqu&#39;à ce que la piste soit affectée à un propriétaire.

* Prénom du détenteur des ventes
* Nom du détenteur des ventes
* Titre du propriétaire commercial
* Numéro de téléphone du détenteur des ventes
* Adresse e-mail du détenteur des ventes
