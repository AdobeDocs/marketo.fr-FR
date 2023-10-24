---
unique-page-id: 9438139
description: Ajouter une personne à la Liste bloquée - Documents Marketo - Documentation du produit
title: Ajouter une personne à la Liste bloquée
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Ajouter une personne à la Liste bloquée {#add-person-to-blocklist}

L’ajout de personnes à votre Liste bloquée les empêche de recevoir votre correspondance.

1. Créer [programme par défaut](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} et donnez-lui le nom &quot;Ajouter à la Liste bloquée&quot;.

1. Cliquez sur **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouvelle ressource locale]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Sélectionner **[!UICONTROL Liste dynamique]**.

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

1. Cliquez sur **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouvelle campagne dynamique]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Nommez la nouvelle campagne dynamique. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Glisser-déposer **[!UICONTROL Membre de la liste dynamique]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Sélectionnez la liste dynamique que vous venez de créer.

   ![](assets/add-person-to-blocklist-9.png)

1. Cliquez sur l&#39;onglet **[!UICONTROL Flux.]** Faites glisser et déposez le **[!UICONTROL Modifier la valeur des données]** Action de flux.

   ![](assets/add-person-to-blocklist-10.png)

1. Dans le **[!UICONTROL Attribut]** menu déroulant **[!UICONTROL Liste bloquée]** et défini **[!UICONTROL Nouvelle valeur]** to **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Cliquez sur le bouton **[!UICONTROL Planification]** et sélectionnez **[!UICONTROL Exécuter une fois]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Sélectionner **[!UICONTROL Exécuter maintenant]** et cliquez sur **[!UICONTROL Exécuter]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Cliquez sur **[!UICONTROL Exécuter]** encore une fois.

   ![](assets/add-person-to-blocklist-14.png)

Ces personnes ne recevront plus d’e-mails.

>[!TIP]
>
>Créez un [Campagne de déclenchement](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} using **Modifier la valeur des données** avec **La liste bloquée est vraie** pour toutes les personnes qui, à l’avenir, auront des attributs qui leur permettront de placer sur la liste bloquée.
