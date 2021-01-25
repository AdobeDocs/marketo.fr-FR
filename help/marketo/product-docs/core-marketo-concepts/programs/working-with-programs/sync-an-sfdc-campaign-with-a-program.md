---
unique-page-id: 1147154
description: Synchronisation d’un Campaign SFDC avec un Programme - Docs marketing - Documentation du produit
title: Synchronisation d’une Campaign SFDC avec un Programme
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Synchroniser un Campaign SFDC avec un Programme {#sync-an-sfdc-campaign-with-a-program}

Marketo vous permet de synchroniser vos programmes avec les campagnes Salesforce afin de conserver la même liste de personnes dans les deux systèmes, y compris leur état. Commençons !

>[!PREREQUISITES]
>
>Vous devez d&#39;abord [activer la synchronisation des campagnes Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).

>[!CAUTION]
>
>Lors de la synchronisation d’une campagne SFDC avec un programme Marketo, les actions SFDC implicites (par exemple, ajouter à SFDC Campaign, synchroniser à SFDC) seront désactivées pour les campagnes enfants du programme.

1. Accédez à **Activités marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Sélectionnez votre programme.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Cliquez sur **Actions de Programme**, puis sélectionnez **Salesforce Campaign Sync**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Sélectionnez **Créer** ou choisissez une campagne Salesforce existante.

   >[!TIP]
   >
   >Si vous sélectionnez une campagne Salesforce existante, veillez à [correspondre aux états de programme de la campagne Salesforce et du programme Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Saisissez le nom de la nouvelle campagne et cliquez sur **Enregistrer**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Vous pouvez maintenant vérifier les détails de synchronisation de la campagne dans la page de résumé du programme.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Excellent ! Désormais, toute modification de l’état du programme dans Marketo est synchronisée avec la campagne de la DDC et vice versa.
