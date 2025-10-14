---
unique-page-id: 7516241
description: Synchronisation de SFDC - File d’attente des leads - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - File d’attente des leads
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 15%

---

# Synchronisation SFDC : file d’attente des leads {#sfdc-sync-lead-queue}

Marketo vous permet d’ajouter des personnes aux [[!DNL Salesforce] files d’attente de prospects](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) pour faciliter la distribution des prospects. Voici les détails.

## Comment affecter une personne à une file d’attente dans Marketo ? {#how-to-assign-a-person-to-a-queue-in-marketo}

Vous pouvez affecter une personne à une file d’attente de leads [!DNL Salesforce] à l’aide de l’une des actions de flux suivantes :

* [&#x200B; Synchroniser la personne avec SFDC &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Modifier le propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>Vous ne pouvez pas créer ni modifier des files d’attente dans Marketo.

## Comment les informations sur le propriétaire du prospect sont-elles stockées si la personne appartient à une file d’attente ? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Si un prospect appartient à une file d’attente dans [!DNL Salesforce], ces champs de commercial restent vides jusqu’à ce que le prospect soit affecté à un propriétaire.

* Prénom du détenteur des ventes
* Nom du détenteur des ventes
* Titre du propriétaire des ventes
* Numéro de téléphone du détenteur des ventes
* Adresse e-mail du détenteur des ventes
