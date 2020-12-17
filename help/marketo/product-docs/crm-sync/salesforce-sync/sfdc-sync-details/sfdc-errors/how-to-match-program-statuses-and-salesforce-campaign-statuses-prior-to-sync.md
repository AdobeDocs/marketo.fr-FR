---
unique-page-id: 2360370
description: Comment faire correspondre les états de Programme et les états de Campaign de Salesforce avant la synchronisation - Docs marketing - Documentation du produit
title: Comment faire correspondre les états de Programme et les états de Campaign de Salesforce avant synchronisation
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# Comment faire correspondre les états de Programme et les états de Campaign de Salesforce avant synchronisation {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Cet article décrit comment corriger une erreur d’état incompatible et mapper les états avant la synchronisation de Marketo Programme et de Salesforce Campaign.

## Que faire si vous avez reçu un message d&#39;erreur {#what-do-you-do-if-you-received-an-error-message}

Si vous essayez de synchroniser avec un Campaign Salesforce existant qui contient des pistes et que la campagne contient un ou plusieurs états incompatibles, un message d’erreur s’affiche. Un Programme Marketo et un Campaign Salesforce *ne sont pas synchronisés* si les états ne correspondent pas exactement.

![](assets/image2015-7-22-9-3a23-3a29.png)

Dans ce message d’erreur, vous pouvez opter pour :

1. Sélectionnez une autre campagne à synchroniser dans le menu déroulant OU
1. Vous pouvez annuler, corriger les erreurs d’état et essayer de synchroniser une fois les erreurs réparées. Pour corriger les erreurs d’état, effectuez l’une des opérations suivantes :

   * Connectez-vous à Salesforce et supprimez ou renommez les États membres Campaign incompatibles afin de les mapper aux statuts du Programme Marketo utilisés pour le type de canal associé à votre Programme Marketo.
   * Modifiez les états de Programme dans Marketo pour les mapper aux états membres de Salesforce Campaign que vous avez en place. Il s’agit d’une fonction d’administration du marketing. Pour plus d’informations, voir [Création d’un Canal de Programme](../../../../../product-docs/administration/tags/create-a-program-channel.md).

