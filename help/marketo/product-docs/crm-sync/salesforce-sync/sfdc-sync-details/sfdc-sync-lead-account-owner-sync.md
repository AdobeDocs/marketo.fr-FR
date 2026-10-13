---
unique-page-id: 2953463
description: Découvrez comment les champs de prospect et de propriétaire de compte se synchronisent de Salesforce vers Marketo. Modifiez le propriétaire du prospect dans Marketo et utilisez les données du propriétaire dans les actions de flux et les listes dynamiques.
title: Synchronisation de SFDC - Synchronisation des prospects et des propriétaires de compte
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/hw4ZXOFSDBvVm45z84aQkxgKU17O-8h1NhukpGCNsos'
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
source-wordcount: '218'
ht-degree: 15%
---
# Synchronisation SFDC : synchronisation propriétaire du compte/lead {#sfdc-sync-lead-account-owner-sync}

Techniquement, ils synchronisent la table « utilisateur » dans [!DNL Salesforce], mais nous l’appellerons champs de prospect/propriétaire de compte.

## Quels champs seront synchronisés avec Marketo Engage ? {#which-fields-will-sync-to-marketo-engage}

Pour chaque personne synchronisée dans Marketo, nous synchronisons également les champs de propriétaire suivants :

* Prénom du propriétaire des ventes
* Nom du propriétaire des ventes
* Titre du propriétaire des ventes
* Numéro de téléphone du propriétaire des ventes
* Adresse e-mail du propriétaire des ventes

Pour chaque contact, nous synchronisons les cinq champs de propriétaire du prospect ci-dessus, ainsi que ces champs de propriétaire de compte :

* Prénom du propriétaire du compte
* Nom du propriétaire du compte
* Adresse e-mail du propriétaire du compte

## Puis-je changer le propriétaire du prospect dans Marketo ? {#can-i-change-the-lead-owner-in-marketo}

Absolument, utilisez simplement l’action de flux [Modifier le propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}.

>[!NOTE]
>
>Vous ne pouvez pas modifier les informations sur le propriétaire à l’aide de la page [Utilisation des détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## Que puis-je faire avec ces données ? {#what-can-i-do-with-this-data}

Il existe de nombreuses raisons d’utiliser ces données, par exemple :

* Envoyer un e-mail personnalisé avec la signature du commercial
* Filtrez des représentants commerciaux spécifiques pour le marketing ou même l’analyse de l’efficacité.
* Règles d’affectation (et de réaffectation) dans Marketo
* Utilisez-les dans les actions de flux [Modifier le propriétaire](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} et [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}

