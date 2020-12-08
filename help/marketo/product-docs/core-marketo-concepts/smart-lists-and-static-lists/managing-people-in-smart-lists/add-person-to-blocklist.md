---
unique-page-id: 9438139
description: Ajouter la personne à Placer sur la liste bloquée - Documentation sur le marketing - Documentation sur le produit
title: Ajouter une personne à Placer sur la liste bloquée
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# Ajouter une personne à Placer sur la liste bloquée {#add-person-to-blocklist}

Ajouter des personnes à votre Liste bloquée les empêche de recevoir votre correspondance.

>[!NOTE]
>
>Marketo est en train de modifier des termes tels que la Liste bloquée et la Liste autorisée à la Liste bloquée et à la Liste autorisée dans notre produit. Au cours de cette mise à jour, vous verrez peut-être les anciens termes de l’interface utilisateur et les captures d’écran de la documentation, ainsi que les nouveaux termes dans le texte de la documentation. Nous nous excusons pour toute confusion.

1. [Créez un programme](../../../../product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) par défaut et nommez-le **Ajouter à la Liste bloquée**.
1. Cliquez sur **Nouveau** et sélectionnez **Nouveau fichier** local.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Nommez votre liste, puis cliquez sur **Créer**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Ajoutez toutes les personnes à votre Liste **** intelligente que vous souhaitez ajouter à votre Liste bloquée.

   >[!NOTE]
   >
   >Les personnes de votre Liste bloquée ne recevront pas de courriels opérationnels.

   ![](assets/three-6.png)

1. Cliquez sur **Nouveau** et sélectionnez **Nouvelle Campaign** intelligente.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Nommez la **Nouvelle Campaign** intelligente. Cliquez sur **Créer**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Faites glisser et déposez **Membre de la Liste** dynamique.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Sélectionnez la liste intelligente que vous venez de créer.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Faites glisser et déposez **Modifier la valeur** des données.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Pour le **flux**, saisissez le **bloc répertorié** pour l’ **attribut** et définissez **Nouvelle valeur sur true.******

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Dans l’onglet **Planification** , sélectionnez **Exécuter une fois**.

   ![](assets/ten.png)

1. Sélectionnez **Exécuter maintenant** et cliquez sur **Exécuter**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   OUI ! Ces personnes ne recevront plus de courriels.

   >[!TIP]
   >
   >Créez une campagne [intelligente](../../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) déclencheuse à l’aide de la fonction **Modifier la valeur** des données avec liste **de blocs est vraie** pour toutes les personnes qui, dans le futur, auront des attributs pouvant bénéficier de la liste bloquée.

