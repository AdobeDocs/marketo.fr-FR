---
unique-page-id: 9438139
description: Ajouter une personne à la Liste bloquée - Documents Marketo - Documentation du produit
title: Ajouter une personne à la Liste bloquée
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Ajouter une personne à la Liste bloquée {#add-person-to-blocklist}

L’ajout de personnes à votre Liste bloquée les empêche de recevoir votre correspondance.

1. Créez un [programme par défaut](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} et nommez-le &quot;Ajouter à la Liste bloquée&quot;.

1. Cliquez sur **[!UICONTROL New]** et sélectionnez **[!UICONTROL New Local Asset]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Sélectionnez **[!UICONTROL Liste dynamique]**.

   ![](assets/add-person-to-blocklist-2.png)

1. Nommez votre liste et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/add-person-to-blocklist-3.png)

1. Ajoutez toutes les personnes à votre liste dynamique que vous souhaitez ajouter à votre Liste bloquée.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Les personnes de votre Liste bloquée ne recevront pas d’e-mails opérationnels.

1. Revenez à votre programme.

   ![](assets/add-person-to-blocklist-5.png)

1. Cliquez sur **[!UICONTROL New]** et sélectionnez **[!UICONTROL New Smart Campaign]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Nommez la nouvelle campagne dynamique. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Effectuez un glisser-déposer de **[!UICONTROL Member of Smart List]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Sélectionnez la liste dynamique que vous venez de créer.

   ![](assets/add-person-to-blocklist-9.png)

1. Cliquez sur l’onglet **[!UICONTROL Flux]** . Faites glisser et déposez l’action Flux **[!UICONTROL Modifier la valeur de données]**.

   ![](assets/add-person-to-blocklist-10.png)

1. Dans la liste déroulante **[!UICONTROL Attribute]** , sélectionnez **[!UICONTROL Block Listed]** et définissez **[!UICONTROL New Value]** sur **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Cliquez sur l’onglet **[!UICONTROL Planning]** et sélectionnez **[!UICONTROL Exécuter une fois]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Sélectionnez **[!UICONTROL Run Now]** et cliquez sur **[!UICONTROL Run]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Cliquez de nouveau sur **[!UICONTROL Exécuter]**.

   ![](assets/add-person-to-blocklist-14.png)

Ces personnes ne recevront plus d’e-mails.

>[!TIP]
>
>Créez une [campagne de déclenchement](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} à l’aide de **Modifier la valeur des données** avec **La liste bloquée est vraie** pour toutes les personnes qui, à l’avenir, auront des attributs pouvant bénéficier d’une liste bloquée.
