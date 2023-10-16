---
unique-page-id: 1147154
description: Synchronisation d’une campagne SFDC avec un programme - Documents Marketo - Documentation du produit
title: Synchronisation d’une campagne SFDC avec un programme
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# Synchronisation d’une campagne SFDC avec un programme {#sync-an-sfdc-campaign-with-a-program}

Marketo Engage vous permet de synchroniser vos programmes avec [!DNL Salesforce] des campagnes pour maintenir la même liste de personnes dans les deux systèmes, y compris leur état. Commençons!

>[!PREREQUISITES]
>
>Vous devrez [enable [!DNL Salesforce] synchronisation des campagnes](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) en premier.

>[!CAUTION]
>
>Lors de la synchronisation d’une campagne SFDC avec un programme de Marketo Engage, les actions SFDC implicites (par exemple, ajouter à une campagne SFDC, Synchroniser avec SFDC) seront désactivées pour les campagnes enfants du programme.

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Sélectionnez votre programme.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Cliquez sur **[!UICONTROL Actions de programme]**, puis sélectionnez **[!UICONTROL Synchronisation des campagnes Salesforce]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Sélectionner **[!UICONTROL Créer]** ou sélectionnez une campagne Salesforce existante.

   >[!TIP]
   >
   >Si vous sélectionnez une campagne Salesforce existante, veillez à [correspondent aux états de programme de la campagne Salesforce et du programme Marketo.](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Saisissez le nom de la nouvelle campagne, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Vous pouvez maintenant vérifier les détails de synchronisation de la campagne dans la page de résumé du programme.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Excellent ! Désormais, toutes les modifications d’état de programme dans Marketo sont synchronisées avec la campagne SFDC et vice versa.
