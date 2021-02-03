---
unique-page-id: 7516241
description: Synchronisation SFDC - File d’attente des pistes - Documents marketing - Documentation du produit
title: Synchronisation SFDC - File d’attente des pistes
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# Synchronisation SFDC : File d&#39;attente de piste {#sfdc-sync-lead-queue}

Marketo vous permet d&#39;ajouter des personnes à [files d&#39;attente de pistes Salesforce](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) pour faciliter la distribution de pistes. Voici les détails.

## Comment affecter une personne à une file d&#39;attente dans Marketo ? {#how-to-assign-a-person-to-a-queue-in-marketo}

Vous pouvez affecter une personne à une file d&#39;attente de piste Salesforce à l&#39;aide de l&#39;une des actions de flux suivantes :

* [Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Changer de propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Vous ne pouvez pas créer ni modifier les files d&#39;attente dans Marketo.

## Comment les informations de propriétaire de prospect sont-elles stockées si la personne appartient à une file d&#39;attente ? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Si une piste appartient à une file d&#39;attente dans Salesforce, ces champs de propriétaire commercial sont conservés vides jusqu&#39;à ce que la piste soit affectée à un propriétaire.

* Prénom du vendeur
* Nom du propriétaire commercial
* Titre du propriétaire commercial
* Numéro de téléphone du vendeur
* Adresse électronique du propriétaire des ventes
