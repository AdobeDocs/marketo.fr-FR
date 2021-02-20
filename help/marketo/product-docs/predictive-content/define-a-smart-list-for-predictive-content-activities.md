---
unique-page-id: 10097873
description: Définir une Liste dynamique pour les Activités de contenu prédictif - Documents marketing - Documentation du produit
title: Définition d’une Liste dynamique pour les Activités de contenu prédictif
translation-type: tm+mt
source-git-commit: f1d7b270454ba41db5197a069e0dcc2caebdec63
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Définir une Liste intelligente pour les Activités de contenu prédictif {#define-a-smart-list-for-predictive-content-activities}

Vous pouvez utiliser des activités de contenu prédictif dans les déclencheurs et les filtres lorsque vous définissez une liste intelligente dans une campagne dynamique. Vous pouvez déclencher une action pour toute personne qui clique sur du contenu prédictif via le [modèle de média enrichi](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), la [barre de recommandation du contenu](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md) ou dans un [courriel](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. Dans votre campagne intelligente, accédez à l&#39;onglet **Liste intelligente**.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Les listes intelligentes peuvent faire des choses incroyables. Pour en savoir plus sur la plongée en [liste intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Recherchez le déclencheur, puis faites-le glisser sur la trame.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Une campagne intelligente avec des déclencheurs s’exécute en mode Déclencheur. Il s’exécute sur une personne à la fois en fonction des événements déclenchés et des filtres ajoutés.

1. Cliquez sur la liste déroulante **Nom** et sélectionnez un opérateur.

   ![](assets/smart-list-dropdown-hands.png)

1. Définissez le déclencheur.

   ![](assets/smart-lislt-select-content-hands.png)

1. Ajoutez la contrainte **Type**.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Sélectionnez la source dont vous avez besoin pour votre liste intelligente.

   ![](assets/pc-add-constraint.png)

1. Si vous utilisez la source de courriel pour votre contenu prédictif, ajoutez le déclencheur **Lien de clics dans Courriel**. Sélectionnez votre adresse électronique et ajoutez la contrainte **Is Predictive**, définie comme **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Ajoutez les autres filtres si nécessaire.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >Dans une campagne intelligente avec des déclencheurs et des filtres, les déclencheurs sont placés en haut. Lorsqu’elle est déclenchée, seules les personnes qui satisfont aux critères de filtre parcourent le flux.

   >[!NOTE]
   >
   >Avec plusieurs déclencheurs, une personne passe au flux si l’un des déclencheurs est activé.

   Pour exécuter la campagne sur un ensemble de personnes en même temps, apprenez comment [définir une liste intelligente pour une campagne par lots ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Définir une Liste intelligente pour une Campaign intelligente | Lot](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Ajouter une étape de flux à un Campaign dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Définir une Liste intelligente pour les Activités de personnalisation Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Activer le contenu prédictif pour les médias enrichis en ligne](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Activation de la barre de recommandation de contenu](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)

