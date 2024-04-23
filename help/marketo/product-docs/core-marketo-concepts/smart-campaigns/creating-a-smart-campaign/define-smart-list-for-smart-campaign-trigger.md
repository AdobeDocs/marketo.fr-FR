---
unique-page-id: 1146942
description: Définition d’une liste dynamique pour Smart Campaign | Déclencheur - Documents Marketo - Documentation du produit
title: Définition d’une liste dynamique pour Smart Campaign | Déclencheur
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
source-git-commit: c3aa1a29b084cb1c1add9d22cdbfc23bdcf7512b
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Définition d’une liste dynamique pour Smart Campaign | Déclencheur {#define-smart-list-for-smart-campaign-trigger}

Effectuez une exécution de campagne dynamique sur une personne à la fois en fonction des événements en direct en ajoutant des déclencheurs.

>[!CAUTION]
>
>La modification d’une campagne active à l’étape Liste dynamique ou Flux peut potentiellement interrompre ses fonctionnalités. Si vous choisissez de le faire, faites preuve de prudence.

1. Dans votre campagne dynamique, cliquez sur le bouton **[!UICONTROL Liste dynamique]** .

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. Recherchez le déclencheur souhaité, puis faites-le glisser sur la zone de travail.

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >Une campagne dynamique avec des déclencheurs s’exécute dans _Déclencheur_ mode . Il s’exécute sur une personne à la fois en fonction des événements déclenchés et des filtres supplémentaires.

   >[!IMPORTANT]
   >
   >Lors de l’utilisation d’un champ booléen dans une liste dynamique de campagne de déclenchement, vous devez le définir explicitement sur &quot;false&quot; afin que le champ soit évalué correctement lors de l’exécution de la campagne.

1. Cliquez sur la liste déroulante et choisissez un opérateur.

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >Des lignes rouges ondulent les erreurs ou les informations manquantes. Si elle n’est pas corrigée, la campagne est invalide et ne s’exécute pas.

   >[!TIP]
   >
   >Dans une campagne dynamique avec à la fois des déclencheurs et des filtres, les déclencheurs s’affichent en haut et, lorsqu’ils sont déclenchés, seules les personnes qui répondent aux critères de filtrage passent par le flux.

1. Définissez le déclencheur.

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >Avec plusieurs déclencheurs, une personne passe par le flux si _ANY_ l’un des déclencheurs est activé.

Pour exécuter la campagne sur un ensemble de personnes simultanément, apprenez à [Définition d’une liste dynamique pour Smart Campaign | Lot](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Ajout d’une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
