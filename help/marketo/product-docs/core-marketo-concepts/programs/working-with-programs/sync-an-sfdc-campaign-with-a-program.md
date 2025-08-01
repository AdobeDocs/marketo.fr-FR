---
unique-page-id: 1147154
description: Synchronisation d’une campagne SFDC avec un programme - Documentation de Marketo - Documentation du produit
title: Synchronisation d’une campagne SFDC avec un programme
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 1%

---

# Synchronisation d’une campagne SFDC avec un programme {#sync-an-sfdc-campaign-with-a-program}

Marketo Engage vous permet de synchroniser vos programmes avec les campagnes [!DNL Salesforce] afin de conserver la même liste de personnes dans les deux systèmes, y compris leurs statuts. C’est parti !

>[!PREREQUISITES]
>
>Vous devez d’abord [activer [!DNL Salesforce] la synchronisation de la campagne](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.

>[!CAUTION]
>
>Lors de la synchronisation d’une campagne SFDC avec un programme Marketo Engage, les actions SFDC implicites (par exemple, ajouter à SFDC Campaign, Synchroniser avec SFDC) sont désactivées pour les campagnes enfants du programme.

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Sélectionnez votre programme.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Cliquez sur **[!UICONTROL Actions du programme]**, puis sélectionnez **[!UICONTROL Synchronisation de la campagne Salesforce]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Sélectionnez **[!UICONTROL Créer]** ou choisissez une campagne [!DNL Salesforce] existante.

   >[!TIP]
   >
   >Si vous sélectionnez une campagne [!DNL Salesforce] existante, veillez à [correspondre aux statuts du programme de la campagne et  [!DNL Salesforce]  programme Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

1. Saisissez le nom de la nouvelle campagne et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Vous pouvez maintenant vérifier les détails de synchronisation de la campagne dans la page de résumé du programme.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Excellent ! Désormais, toutes les modifications de statut du programme dans Marketo sont synchronisées avec la campagne SFDC et vice versa.
