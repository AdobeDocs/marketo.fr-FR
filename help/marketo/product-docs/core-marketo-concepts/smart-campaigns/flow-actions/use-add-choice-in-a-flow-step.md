---
unique-page-id: 1146980
description: Utilisation de l’option Ajouter un choix dans une étape de flux - Documents Marketo - Documentation du produit
title: Utilisation de l’option Ajouter un choix à une étape de flux
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Utilisation de l’option Ajouter un choix à une étape de flux {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Ajout d’une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

&quot;Ajouter un choix&quot; vous permet d’utiliser une étape de flux et de dire &quot;cela dépend&quot; lorsque vous choisissez les détails.

1. Sous l’onglet **[!UICONTROL Flux]** de la campagne dynamique, ajoutez n’importe quelle étape de flux, puis cliquez sur **[!UICONTROL Ajouter un choix]**.

   ![](assets/use-add-choice-in-a-flow-step-1.png)

1. Sélectionnez la condition de choix.

   ![](assets/use-add-choice-in-a-flow-step-2.png)

1. Sélectionnez l&#39;opérateur de choix et saisissez une valeur de choix. Cela définit vos critères ou votre choix.

   ![](assets/use-add-choice-in-a-flow-step-3.png)

1. Saisissez une valeur d’étape de flux pour le choix.

   ![](assets/use-add-choice-in-a-flow-step-4.png)

   >[!CAUTION]
   >
   >Les jetons _ne fonctionnent pas_ dans la partie condition d’une étape de flux de choix.

1. Répétez les étapes ci-dessus pour ajouter plusieurs choix, puis ajoutez/ajustez la valeur par défaut.

   ![](assets/use-add-choice-in-a-flow-step-5.png)

   >[!TIP]
   >
   >Vous pouvez définir l’une de vos étapes de flux sur —Do Nothing—, auquel cas aucune action ne sera effectuée sur ce choix.

   >[!CAUTION]
   >
   >Seul le premier choix correspondant est appliqué à l’étape de flux. Découvrez comment [réorganiser &quot;Ajouter un choix&quot; dans une action de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   Fantastique ! Vous pouvez désormais créer une seule campagne dynamique avec des choix d’étape de flux au lieu de créer plusieurs campagnes dynamiques pour chaque choix.

   >[!MORELIKETHIS]
   >
   >[Réorganiser l’ajout de choix dans une étape de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
