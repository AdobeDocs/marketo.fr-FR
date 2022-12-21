---
unique-page-id: 10097867
description: Définition d’une liste dynamique pour les activités de personnalisation web - Documents Marketo - Documentation du produit
title: Définition d’une liste dynamique pour les activités de personnalisation web
exl-id: 9987f922-f50c-47b3-aef6-230326b094fc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Définition d’une liste dynamique pour les activités de personnalisation web {#define-a-smart-list-for-web-personalization-activities}

Vous pouvez utiliser des activités de personnalisation web dans des filtres et des triggers lorsque vous définissez une liste dynamique dans une campagne dynamique. Ici, vous souhaitez capturer toute personne ayant cliqué sur un appel à l’action de personnalisation web (campagne).

Utilisez un trigger pour envoyer un email ou une alerte, ou pour modifier une valeur ou un score en fonction des visiteurs qui ont cliqué et ont interagi avec un appel à l’action de personnalisation web. Vous pouvez également filtrer et afficher les pistes ayant cliqué sur un appel à l’action de personnalisation web.

1. Dans votre campagne dynamique, cliquez sur le bouton **Liste dynamique** .

   ![](assets/image2016-2-9-10-3a49-3a18.png)

   >[!NOTE]
   >
   >Les listes intelligentes peuvent faire des choses étonnantes. En savoir plus dans la section [Exploration approfondie par liste intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Recherchez le déclencheur, puis faites-le glisser sur la zone de travail.

   ![](assets/image2016-6-8-9-3a24-3a24.png)

   >[!NOTE]
   >
   >Une campagne dynamique avec des déclencheurs s’exécute en mode Déclencheur. Il s’exécute sur une personne à la fois en fonction des événements déclenchés et des filtres ajoutés.

1. Cliquez sur la liste déroulante et choisissez un opérateur.

   ![](assets/image2016-6-7-11-3a10-3a8.png)

   >[!CAUTION]
   >
   >Les lignes rouge ondulent indiquent une erreur. Si elle n’est pas corrigée, la campagne devient non valide et elle ne s’exécute pas.

1. Définissez le déclencheur.

   ![](assets/image2016-6-7-11-3a12-3a23.png)

1. Ajoutez des filtres selon vos besoins.

   ![](assets/image2016-6-7-11-3a14-3a20.png)

   >[!TIP]
   >
   >Dans une campagne dynamique avec des déclencheurs et des filtres, les déclencheurs se situent dans la partie supérieure. Lorsqu’elle est déclenchée, seules les personnes qui répondent aux critères de filtrage parcourent le flux.

   >[!NOTE]
   >
   >Avec plusieurs déclencheurs, une personne passe au flux si L’UN D’eux est activé.

   Pour exécuter la campagne sur un ensemble de personnes en même temps, apprenez à [Définition d’une liste dynamique pour Smart Campaign | Lot](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Définition d’une liste dynamique pour Smart Campaign | Lot](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Ajout d’une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Définition d’une liste dynamique pour les activités de contenu prédictif](/help/marketo/product-docs/predictive-content/define-a-smart-list-for-predictive-content-activities.md)

