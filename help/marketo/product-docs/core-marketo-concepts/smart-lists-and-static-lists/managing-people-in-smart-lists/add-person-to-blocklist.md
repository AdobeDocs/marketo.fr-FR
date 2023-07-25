---
unique-page-id: 9438139
description: Ajout d’une personne à la Liste bloquée - Documents Marketo - Documentation du produit
title: Ajouter une personne à la Liste bloquée
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Ajouter une personne à la Liste bloquée {#add-person-to-blocklist}

L’ajout de personnes à votre Liste bloquée les empêche de recevoir votre correspondance.

>[!NOTE]
>
>Marketo est en train de modifier des termes tels que Liste bloquée et Liste autorisée pour Placer sur la liste bloquée et Placer sur la liste autorisée dans notre produit. Au cours de cette mise à jour, il se peut que les anciens termes apparaissent dans les captures d’écran de l’interface utilisateur et de la documentation, ainsi que les nouveaux termes dans le texte de la documentation. Nous nous excusons pour toute confusion.

1. [Création d’un programme par défaut](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) et nommez-le **Ajouter à la Liste bloquée**.

1. Cliquez sur **Nouveau** et sélectionnez **Nouvelle ressource locale**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Nommez votre liste et cliquez sur **Créer**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Ajoutez toutes les personnes à votre **Liste dynamique** vous voulez être ajouté à votre Liste bloquée.

   >[!NOTE]
   >
   >Les personnes de votre Liste bloquée ne recevront pas d’e-mails opérationnels.

   ![](assets/three-6.png)

1. Cliquez sur **Nouveau** et sélectionnez **Nouvelle campagne dynamique**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Attribuez un nom au **Nouvelle campagne dynamique**. Cliquez sur **Créer**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Glisser-déposer **Membre de la liste dynamique**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Sélectionnez la liste dynamique que vous venez de créer.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Glisser-déposer **Modifier la valeur des données**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Pour le **Flux**, saisissez **Liste bloquée** pour le **Attribut** et défini **Nouvelle valeur** to **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Sur le **Planification** onglet, sélectionnez **Exécuter une fois**.

   ![](assets/ten.png)

1. Sélectionner **Exécuter maintenant** et cliquez sur **Exécuter**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   OUI ! Ces personnes ne recevront plus d’e-mails.

   >[!TIP]
   >
   >Créez un [déclencher une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) using **Modifier la valeur des données** avec **La liste bloquée est vraie** pour toutes les personnes qui, à l’avenir, auront des attributs qui leur permettront de placer sur la liste bloquée.
