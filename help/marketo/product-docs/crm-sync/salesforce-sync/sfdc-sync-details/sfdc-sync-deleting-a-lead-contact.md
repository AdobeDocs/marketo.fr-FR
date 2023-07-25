---
unique-page-id: 7515131
description: Synchronisation SFDC - Suppression d’un prospect/contact - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Suppression d’un prospect/contact
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Synchronisation SFDC : Suppression d’un prospect/contact {#sfdc-sync-deleting-a-lead-contact}

Voici quelques détails :

* Marketo ne supprime pas automatiquement les personnes simplement parce que les pistes ont été supprimées dans Salesforce. L’indicateur &quot;SFDC Is Deleted&quot; du champ est défini sur true. Si vous le souhaitez, vous pouvez déclencher la suppression de ce champ dans Marketo.
* [Supprimer une personne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) action de flux. Cela supprime une personne dans MKTO, mais vous avez le choix de la supprimer dans `Salesforce` trop.

* [Supprimer de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) action de flux : Cela supprime une piste dans SFDC, mais vous avez également le choix de supprimer une personne dans Marketo.
* Si une piste est supprimée dans Salesforce (mais qu’une personne n’est pas supprimée dans Marketo), elle passe ensuite par [Synchroniser avec Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) d’une action de flux, qui créerait un nouveau prospect dans Salesforce.
