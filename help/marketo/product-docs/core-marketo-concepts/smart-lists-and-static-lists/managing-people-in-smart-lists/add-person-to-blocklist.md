---
unique-page-id: 9438139
description: Placer sur la liste bloquée Ajouter une personne à la documentation - Documents Marketo - Documentation du produit
title: Ajouter une personne à la liste bloquée
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 5%

---

# Ajouter une personne à la liste bloquée {#add-person-to-blocklist}

L’ajout de personnes à votre Place sur la liste bloquée les empêche de recevoir votre correspondance.

1. Créez un nouveau [programme par défaut](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} et nommez-le « Ajouter à la Liste bloquée ».

1. Cliquez sur **[!UICONTROL Nouveau]** puis sélectionnez **[!UICONTROL Nouvelle ressource locale]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Sélectionnez **[!UICONTROL Liste dynamique]**.

   ![](assets/add-person-to-blocklist-2.png)

1. Nommez votre liste, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/add-person-to-blocklist-3.png)

1. Ajoutez à votre liste dynamique toutes les personnes que vous souhaitez ajouter à votre Place sur la liste bloquée.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Les personnes sur votre Place sur la liste bloquée ne recevront pas d’e-mails opérationnels.

1. Revenez à votre programme.

   ![](assets/add-person-to-blocklist-5.png)

1. Cliquez sur **[!UICONTROL Nouveau]** puis sélectionnez **[!UICONTROL Nouvelle campagne intelligente]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Nommez la nouvelle campagne intelligente. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Glisser-déposer **[!UICONTROL Membre de la liste dynamique]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Sélectionnez la liste dynamique que vous venez de créer.

   ![](assets/add-person-to-blocklist-9.png)

1. Cliquez sur l’onglet **[!UICONTROL Flux]**. Faites glisser et déposez l’action de flux **[!UICONTROL Modifier la valeur des données]**.

   ![](assets/add-person-to-blocklist-10.png)

1. Dans le menu déroulant **[!UICONTROL Attribut]**, sélectionnez **[!UICONTROL Liste bloquée]** et définissez **[!UICONTROL Nouvelle valeur]** sur **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Cliquez sur l’onglet **[!UICONTROL Planifier]** et sélectionnez **[!UICONTROL Exécuter une fois]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Sélectionnez **[!UICONTROL Exécuter maintenant]** et cliquez sur **[!UICONTROL Exécuter]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Cliquez de nouveau sur **[!UICONTROL Exécuter]**.

   ![](assets/add-person-to-blocklist-14.png)

Ces personnes ne recevront plus d’e-mails.

>[!TIP]
>
>Placer sur la liste bloquée Créez une [Campagne Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} à l’aide de **Modifier la valeur des données** avec **La liste bloquée est vraie** pour toutes les personnes qui auront à l’avenir des attributs pouvant être traités par.
