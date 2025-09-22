---
unique-page-id: 7515131
description: Synchronisation de SFDC - Suppression d’un prospect/contact - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - Suppression d’un lead/contact
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 4%

---

# Synchronisation SFDC : suppression d’un lead/contact {#sfdc-sync-deleting-a-lead-contact}

Voici quelques détails :

* Marketo ne supprime pas automatiquement les personnes simplement parce que des prospects ont été supprimés en [!DNL Salesforce]. Au lieu de cela, un indicateur de champ « SFDC supprimé » est défini sur « true ». Vous pouvez déclencher l’action hors de ce champ pour le supprimer dans Marketo, si vous le souhaitez.
* [Supprimer une personne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) action de flux. Cela supprime une personne dans MKTO, mais vous avez également la possibilité de la supprimer dans `Salesforce`.

* [Supprimer de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) action de flux : permet de supprimer un prospect dans SFDC, mais vous pouvez également supprimer une personne dans Marketo.
* Si un prospect est supprimé dans [!DNL Salesforce] (mais qu’une personne n’est pas supprimée dans Marketo), puis qu’il est exécuté par la suite dans l’action de flux [Synchroniser avec [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), un nouveau prospect est créé dans [!DNL Salesforce].
