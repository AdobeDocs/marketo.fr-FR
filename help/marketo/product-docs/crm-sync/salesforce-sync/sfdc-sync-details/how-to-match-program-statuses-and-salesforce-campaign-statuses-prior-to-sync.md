---
unique-page-id: 2360370
description: Comment faire correspondre les états du programme et les états de Salesforce Campaign avant la synchronisation - Documents Marketo - Documentation du produit
title: Comment faire correspondre les états de programme et les états de campagne Salesforce avant synchronisation
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Comment faire correspondre les états de programme et les états de campagne Salesforce avant synchronisation {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Cet article décrit comment corriger une erreur d’état incompatible et mapper les états avant la synchronisation du programme Marketo et de Salesforce Campaign.

## Que faire si vous avez reçu un message d’erreur {#what-do-you-do-if-you-received-an-error-message}

Si vous essayez de vous synchroniser avec une campagne Salesforce existante qui contient des pistes et que la campagne contient un ou plusieurs statuts incompatibles, un message d’erreur s’affiche. Un programme Marketo et une campagne Salesforce *will not* synchroniser si les états ne correspondent pas exactement.

![](assets/image2015-7-22-9-3a23-3a29.png)

A partir de ce message d&#39;erreur, vous pouvez opter pour :

1. Sélectionnez une autre campagne à synchroniser dans le menu déroulant, OU
1. Vous pouvez annuler, corriger les erreurs d’état et essayer de vous synchroniser une fois les erreurs réparées. Pour corriger les erreurs d’état, effectuez l’une des opérations suivantes :

   * Connectez-vous à Salesforce et supprimez ou renommez les états membres de Campaign incompatibles pour les mapper aux états du programme Marketo utilisés pour le type de canal associé à votre programme Marketo.
   * Modifiez les états du programme dans Marketo pour les mapper aux états membres de Campaign Salesforce que vous avez en place. Il s’agit d’une fonction d’administration Marketo. Pour plus d’informations, voir [Création d’un canal de programme](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.
