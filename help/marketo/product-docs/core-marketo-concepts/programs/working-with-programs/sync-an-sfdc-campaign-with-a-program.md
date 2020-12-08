---
unique-page-id: 1147154
description: Synchronisation d’un Campaign SFDC avec un Programme - Docs marketing - Documentation du produit
title: Synchronisation d’une Campaign SFDC avec un Programme
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Synchronisation d’une Campaign SFDC avec un Programme {#sync-an-sfdc-campaign-with-a-program}

Marketo vous permet de synchroniser vos programmes avec les campagnes Salesforce afin de conserver la même liste de personnes dans les deux systèmes, y compris leur état. Commençons !

>[!NOTE]
>
>**Conditions préalables**
>
>Vous devez d&#39;abord [activer la synchronisation](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) des campagnes Salesforce.

>[!CAUTION]
>
>Lors de la synchronisation d’une campagne SFDC avec un programme Marketo, les actions SFDC implicites (par exemple, ajouter à SFDC Campaign, synchroniser à SFDC) seront désactivées pour les campagnes enfants du programme.

1. Accédez à Activités **** marketing.

   ![](assets/login-marketing-activities-1.png)

1. Sélectionnez votre programme.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Cliquez sur Actions **de** Programme, puis sélectionnez **Salesforce Campaign Sync**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Sélectionnez **Créer **ou choisissez une campagne Salesforce existante.

   >[!TIP]
   >
   >Si vous sélectionnez une campagne Salesforce existante, veillez à [correspondre aux états de programme de la campagne Salesforce et du programme](../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)Marketo.

1. Saisissez le nom de la nouvelle campagne, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Vous pouvez maintenant vérifier les détails de synchronisation de la campagne dans la page de résumé du programme.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Excellent ! Désormais, toute modification de l’état du programme dans Marketo est synchronisée avec la campagne de la DDC et vice versa.

