---
unique-page-id: 7516241
description: Découvrez comment affecter des personnes aux files d’attente de prospects Salesforce à partir de Marketo. Utilisez Synchroniser la personne avec SFDC ou Modifier le propriétaire pour les actions de flux de distribution de leads.
title: Synchronisation de SFDC - File d’attente des leads
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/aUrT7qSMy65t3K07O176nt-Bzjm9urgnXKAkZgs1-cs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 150
ht-degree: 17%

---

# Synchronisation SFDC : file d’attente des leads {#sfdc-sync-lead-queue}

Marketo vous permet d’ajouter des personnes aux [[!DNL Salesforce] files d’attente de prospects](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) pour faciliter la distribution des prospects. Voici les détails.

## Comment affecter une personne à une file d’attente dans Marketo ? {#how-to-assign-a-person-to-a-queue-in-marketo}

Vous pouvez affecter une personne à une file d’attente de leads [!DNL Salesforce] à l’aide de l’une des actions de flux suivantes :

* [Synchroniser une personne dans SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Modifier l’entité propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

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
