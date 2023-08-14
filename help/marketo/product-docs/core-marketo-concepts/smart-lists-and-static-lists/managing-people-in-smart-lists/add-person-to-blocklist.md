---
unique-page-id: 9438139
description: Ajouter une personne à la Liste bloquée - Documents Marketo - Documentation du produit
title: Ajouter une personne à la Liste bloquée
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: cc87ecb8d3245734ec0ce984eeccf742833a85d2
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 3%

---

# Ajouter une personne à la Liste bloquée {#add-person-to-blocklist}

L’ajout de personnes à votre Liste bloquée les empêche de recevoir votre correspondance.

1. [Créer un programme par défaut](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) et nommez-le **Ajouter à la Liste bloquée**.

1. Cliquez sur **Nouveau** et sélectionnez **Nouvelle ressource locale**.

   ![](assets/add-person-to-blocklist-1.png)

1. Sélectionner **Liste dynamique**.

   ![](assets/add-person-to-blocklist-2.png)

1. Nommez votre liste et cliquez sur **Créer**.

   ![](assets/add-person-to-blocklist-3.png)

1. Ajoutez toutes les personnes à votre **Liste dynamique** vous voulez être ajouté à votre Liste bloquée.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Les personnes de votre Liste bloquée ne recevront pas d’e-mails opérationnels.

1. Revenez à votre programme.

   ![](assets/add-person-to-blocklist-5.png)

1. Cliquez sur **Nouveau** et sélectionnez **Nouvelle campagne dynamique**.

   ![](assets/add-person-to-blocklist-6.png)

1. Attribuez un nom au **Nouvelle campagne dynamique**. Cliquez sur **Créer**.

   ![](assets/add-person-to-blocklist-7.png)

1. Glisser-déposer **Membre de la liste dynamique**.

   ![](assets/add-person-to-blocklist-8.png)

1. Sélectionnez la liste dynamique que vous venez de créer.

   ![](assets/add-person-to-blocklist-9.png)

1. Cliquez sur l&#39;onglet **Flux.** Faites glisser et déposez le **Modifier la valeur des données** Action de flux.

   ![](assets/add-person-to-blocklist-10.png)

1. Dans le **Attribut** menu déroulant **Liste bloquée** et défini **Nouvelle valeur** to **true**.

   ![](assets/add-person-to-blocklist-11.png)

1. Cliquez sur le bouton **Planification** et sélectionnez **Exécuter une fois**.

   ![](assets/add-person-to-blocklist-12.png)

1. Sélectionner **Exécuter maintenant** et cliquez sur **Exécuter**.

   ![](assets/add-person-to-blocklist-13.png)

1. Cliquez sur **Exécuter** encore une fois.

   ![](assets/add-person-to-blocklist-14.png)

Ces personnes ne recevront plus d’e-mails.

>[!TIP]
>
>Créez un [déclencher une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) using **Modifier la valeur des données** avec **La liste bloquée est vraie** pour toutes les personnes qui, à l’avenir, auront des attributs qui leur permettront de placer sur la liste bloquée.
