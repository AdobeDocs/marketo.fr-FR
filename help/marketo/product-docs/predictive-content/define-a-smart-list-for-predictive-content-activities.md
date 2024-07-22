---
unique-page-id: 10097873
description: Définition d’une liste dynamique pour les activités de contenu prédictif - Documents Marketo - Documentation du produit
title: Définition d’une liste dynamique pour les activités de contenu prédictif
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Définition d’une liste dynamique pour les activités de contenu prédictif {#define-a-smart-list-for-predictive-content-activities}

Vous pouvez utiliser des activités de contenu prédictif dans les déclencheurs et les filtres lorsque vous définissez une liste dynamique dans une campagne dynamique. Vous pouvez déclencher une action pour toute personne qui clique sur du contenu prédictif via le [modèle de média enrichi](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), la [barre de recommandation de contenu](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md) ou dans un [email](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. Dans votre campagne dynamique, accédez à l’onglet **Liste dynamique**.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Les listes intelligentes peuvent faire des choses étonnantes. Pour en savoir plus, consultez la [présentation détaillée de la liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Recherchez le déclencheur, puis faites-le glisser sur la zone de travail.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Une campagne dynamique avec des déclencheurs s’exécute en mode Déclencheur. Il s’exécute sur une personne à la fois en fonction des événements déclenchés et des filtres ajoutés.

1. Cliquez sur la liste déroulante **Nom** et sélectionnez un opérateur.

   ![](assets/smart-list-dropdown-hands.png)

1. Définissez le déclencheur.

   ![](assets/smart-lislt-select-content-hands.png)

1. Ajoutez la contrainte **Type** .

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Sélectionnez la source dont vous avez besoin pour votre liste dynamique.

   ![](assets/pc-add-constraint.png)

1. Si vous utilisez la source de courrier électronique pour votre contenu prédictif, ajoutez le déclencheur **Lien des clics dans Email**. Sélectionnez votre email et ajoutez la contrainte **Is Predictive**, définie comme **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Ajoutez d’autres filtres si nécessaire.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >Dans une campagne dynamique avec des déclencheurs et des filtres, les déclencheurs se situent dans la partie supérieure. Lorsqu’elles sont déclenchées, seules les personnes qui répondent aux critères de filtrage traversent le flux.

   >[!NOTE]
   >
   >Avec plusieurs déclencheurs, une personne passe au flux si l’un d’eux est activé.

   Pour exécuter la campagne sur un ensemble de personnes en même temps, apprenez à [définir une liste dynamique pour une campagne dynamique par lot](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [ Définition d’une liste dynamique pour une campagne dynamique | Lot](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Ajout d’une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Définition d’une liste dynamique pour les activités Web Personalization](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Activer le contenu prédictif pour le contenu multimédia Web enrichi](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Activer la barre de recommandation de contenu](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)
