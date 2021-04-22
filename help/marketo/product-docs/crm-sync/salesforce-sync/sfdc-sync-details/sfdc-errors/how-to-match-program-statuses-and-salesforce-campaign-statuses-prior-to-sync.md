---
unique-page-id: 2360370
description: Comment faire correspondre les états de Programme et les états de Campaign de Salesforce avant synchronisation - Marketo Docs - Documentation du produit
title: Comment faire correspondre les états de Programme et les états de Campaign de Salesforce avant synchronisation
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Comment faire correspondre les états de Programme et les états de Campaign de Salesforce avant synchronisation {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Cet article décrit comment corriger une erreur d’état incompatible et mapper les états avant la synchronisation Marketo Programme et Salesforce Campaign.

## Que faire si vous avez reçu un message d&#39;erreur {#what-do-you-do-if-you-received-an-error-message}

Si vous essayez de synchroniser avec un Campaign Salesforce existant qui contient des pistes et que la campagne contient un ou plusieurs états incompatibles, un message d’erreur s’affiche. Un Programme Marketo et un Campaign Salesforce *ne sont pas synchronisés* si les états ne correspondent pas exactement.

![](assets/image2015-7-22-9-3a23-3a29.png)

Dans ce message d’erreur, vous pouvez opter pour :

1. Sélectionnez une autre campagne à synchroniser dans le menu déroulant OU
1. Vous pouvez annuler, corriger les erreurs d’état et essayer de synchroniser une fois les erreurs réparées. Pour corriger les erreurs d’état, effectuez l’une des opérations suivantes :

   * Connectez-vous à Salesforce et supprimez ou renommez les États membres Campaign incompatibles pour les mapper aux états Programmes Marketo utilisés pour le type de canal associé à votre Programme Marketo.
   * Modifiez les statuts du Programme dans Marketo pour établir une correspondance avec les statuts de Campaign de Salesforce que vous avez en place. Il s’agit d’une fonction d’administration Marketo. Pour plus d’informations, voir [Création d’un Canal de Programme](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
