---
unique-page-id: 1146980
description: Utilisation de l’option Ajouter un choix dans une étape de flux - Documents Marketo - Documentation du produit
title: Utilisation de l’option Ajouter un choix à une étape de flux
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Utilisation de l’option Ajouter un choix à une étape de flux {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Ajout d’une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

&quot;Ajouter un choix&quot; vous permet d’utiliser une étape de flux et de dire &quot;cela dépend&quot; lorsque vous choisissez les détails.

1. Sous , **[!UICONTROL Flux]** de la campagne dynamique, ajoutez toute étape de flux, puis cliquez sur **[!UICONTROL Ajouter un choix]**.

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. Sélectionnez la condition de choix.

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. Sélectionnez l&#39;opérateur de choix et saisissez une valeur de choix. Cela définit vos critères ou votre choix.

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. Saisissez une valeur d’étape de flux pour le choix.

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >Les jetons seront _not_ travailler dans la partie condition d’une étape de flux de choix.

1. Répétez les étapes ci-dessus pour ajouter plusieurs choix, puis ajoutez/ajustez la valeur par défaut.

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >Vous pouvez définir l’une de vos étapes de flux sur —Do Nothing—, auquel cas aucune action ne sera effectuée sur ce choix.

   >[!CAUTION]
   >
   >Seul le premier choix correspondant est appliqué à l’étape de flux. Découvrez comment [Réorganiser &quot;Ajouter un choix&quot; dans une action de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   Fantastique ! Vous pouvez désormais créer une seule campagne dynamique avec des choix d’étape de flux au lieu de créer plusieurs campagnes dynamiques pour chaque choix.

   >[!MORELIKETHIS]
   >
   >[Réorganiser l’ajout de choix à une étape de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
