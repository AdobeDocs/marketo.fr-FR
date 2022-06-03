---
unique-page-id: 1146942
description: Définition d’une liste dynamique pour Smart Campaign | Déclencheur - Documents Marketo - Documentation du produit
title: Définition d’une liste dynamique pour Smart Campaign | Déclencheur
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
source-git-commit: a15a4b9bccb069b51186aac7b913008d15aa645e
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Définition d’une liste dynamique pour Smart Campaign | Déclencheur {#define-smart-list-for-smart-campaign-trigger}

Effectuez une exécution de campagne intelligente d’une personne à la fois en fonction des événements en direct en ajoutant des déclencheurs.

1. Dans votre campagne dynamique, cliquez sur le bouton **Liste dynamique** .

   ![](assets/image2014-9-19-16-3a22-3a55.png)

1. Recherchez le déclencheur, puis faites-le glisser sur la zone de travail.

   ![](assets/image2014-9-19-16-3a23-3a24.png)

   >[!NOTE]
   >
   >Une campagne dynamique avec des déclencheurs s’exécute dans **Déclencheur** mode . Il s’exécute sur une personne à la fois en fonction des événements déclenchés et des filtres supplémentaires.

   >[!IMPORTANT]
   >
   >Lors de l’utilisation d’un champ booléen dans une liste dynamique de campagne de déclenchement, vous devez le définir explicitement sur &quot;false&quot; afin que le champ soit évalué correctement lors de l’exécution de la campagne.

1. Cliquez sur la liste déroulante et choisissez un opérateur.

   ![](assets/image2014-9-19-16-3a23-3a29.png)

   >[!CAUTION]
   >
   >Des lignes rouges ondulent les erreurs ou les informations manquantes. Si elle n’est pas corrigée, la campagne est invalide et ne s’exécute pas.

   >[!TIP]
   >
   >Dans une campagne dynamique comportant à la fois des déclencheurs et des filtres, les déclencheurs s’affichent en haut et, lorsqu’ils sont déclenchés, seules les personnes qui répondent aux critères de filtrage passent par le flux.

1. Définissez le déclencheur.

   ![](assets/image2014-9-19-16-3a24-3a36.png)

   >[!NOTE]
   >
   >Avec plusieurs déclencheurs, une personne passe par le flux si **ANY** l’un des déclencheurs est activé.

Pour exécuter la campagne sur un ensemble de personnes en même temps, apprenez à [Définition d’une liste dynamique pour Smart Campaign | Lot](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

>[!MORELIKETHIS]
>
>[Ajout d’une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
