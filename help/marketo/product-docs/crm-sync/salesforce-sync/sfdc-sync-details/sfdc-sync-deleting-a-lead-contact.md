---
unique-page-id: 7515131
description: Synchronisation SFDC - Suppression d’une piste/d’un contact - Documents marketing - Documentation du produit
title: Synchronisation SFDC - Suppression d’une piste/d’un contact
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# Synchronisation SFDC : Suppression d&#39;une piste/d&#39;un contact {#sfdc-sync-deleting-a-lead-contact}

Voici quelques détails :

* Marketo ne supprime pas automatiquement les personnes simplement parce que les pistes ont été supprimées dans Salesforce. L’indicateur &quot;SFDC Is Deleted&quot; du champ est défini sur true. Si vous le souhaitez, vous pouvez déclencher la suppression de ce champ dans Marketing.
* [Supprimer l’action ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) Personflow. Ceci supprime une personne dans MKTO mais vous avez le choix de supprimer dans `Salesforce` également.

* [Supprimer de l’action ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow : Ceci supprime une piste dans la DDC mais vous avez le choix de supprimer une personne sur le marché également.
* Si une piste est supprimée dans Salesforce (mais qu&#39;une personne n&#39;est pas supprimée dans Marketo) et qu&#39;elle passe ensuite par l&#39;action de flux [Synchroniser avec Salesforce](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), elle crée une piste dans Salesforce.

En d&#39;autres termes, ça marche comme de la magie !

![—](assets/image2015-5-20-15-3a3-3a27.png)

