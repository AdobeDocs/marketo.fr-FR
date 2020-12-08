---
unique-page-id: 7516241
description: Synchronisation SFDC - File d’attente des pistes - Documents marketing - Documentation du produit
title: Synchronisation SFDC - File d’attente des pistes
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Synchronisation SFDC : File d&#39;attente de piste {#sfdc-sync-lead-queue}

Marketo vous permet d&#39;ajouter des personnes aux files d&#39;attente [de pistes](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) Salesforce pour faciliter la distribution de pistes. Voici les détails.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Comment affecter une personne à une file d&#39;attente dans Marketo ? {#how-to-assign-a-person-to-a-queue-in-marketo}

Vous pouvez affecter une personne à une file d&#39;attente de piste Salesforce à l&#39;aide de l&#39;une des actions de flux suivantes :

* [Synchroniser la personne avec SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Changer de propriétaire](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

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

