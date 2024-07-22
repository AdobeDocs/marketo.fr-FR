---
unique-page-id: 7515131
description: Synchronisation SFDC - Suppression d’un prospect/contact - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Suppression d’un prospect/contact
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Synchronisation SFDC : suppression d’un prospect/contact {#sfdc-sync-deleting-a-lead-contact}

Voici quelques détails :

* Marketo Engage ne supprime pas automatiquement les personnes simplement parce que les pistes ont été supprimées dans Salesforce. L’indicateur &quot;SFDC Is Deleted&quot; du champ est défini sur true. Si vous le souhaitez, vous pouvez déclencher la suppression de ce champ dans Marketo.
* Action de flux [Supprimer la personne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md){target="_blank"}. Cela supprime une personne dans MKTO, mais vous avez également le choix de la supprimer dans `Salesforce`.

* Action de flux [Supprimer de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md){target="_blank"} : supprime un prospect dans SFDC, mais vous avez également le choix de supprimer une personne dans Marketo.
* Si une piste est supprimée dans Salesforce (mais qu’une personne n’est pas supprimée dans Marketo) et qu’elle passe ensuite par l’action de flux [Synchroniser avec Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}, elle crée une piste dans Salesforce.
