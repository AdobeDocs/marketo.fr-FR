---
unique-page-id: 7515131
description: Découvrez comment fonctionne la suppression des prospects et des contacts entre Salesforce et Marketo. Découvrez les actions de flux Supprimer une personne et Supprimer à partir de SFDC .
title: Synchronisation de SFDC - Suppression d’un lead/contact
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/v0nRloqmlp-iedcmE4DdATxpYXnvB13cxkEn7809Hy4'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 4%
---
# Synchronisation SFDC : suppression d’un lead/contact {#sfdc-sync-deleting-a-lead-contact}

Voici quelques détails :

* Marketo ne supprime pas automatiquement les personnes simplement parce que des prospects ont été supprimés en [!DNL Salesforce]. Au lieu de cela, un indicateur de champ « SFDC supprimé » est défini sur « true ». Vous pouvez déclencher l’action hors de ce champ pour le supprimer dans Marketo, si vous le souhaitez.
* [Supprimer une personne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) action de flux. Cela supprime une personne dans MKTO, mais vous avez également la possibilité de la supprimer dans `Salesforce`.

* [Supprimer de SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) action de flux : permet de supprimer un prospect dans SFDC, mais vous pouvez également supprimer une personne dans Marketo.
* Si un prospect est supprimé dans [!DNL Salesforce] (mais qu’une personne n’est pas supprimée dans Marketo), puis qu’il est exécuté par la suite dans l’action de flux [Synchroniser avec [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), un nouveau prospect est créé dans [!DNL Salesforce].
