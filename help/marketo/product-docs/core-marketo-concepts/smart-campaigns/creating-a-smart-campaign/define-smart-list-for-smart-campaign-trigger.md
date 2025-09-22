---
unique-page-id: 1146942
description: Définir une liste dynamique pour une campagne dynamique | Déclencheur - Documents Marketo - Documentation du produit
title: Définir une liste intelligente pour une campagne intelligente | À déclencheur
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 5%

---

# Définir une liste intelligente pour une campagne intelligente | À déclencheur {#define-smart-list-for-smart-campaign-trigger}

Créez une campagne intelligente exécutée sur une personne à la fois en fonction des événements en direct en ajoutant des déclencheurs.

>[!CAUTION]
>
>Apporter des modifications à une liste dynamique ou à une étape de flux à une campagne active peut potentiellement interrompre sa fonctionnalité. Si vous choisissez de le faire, faites preuve de prudence.

1. Dans votre campagne dynamique, cliquez sur l’onglet **[!UICONTROL Liste dynamique]**.

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. Recherchez le déclencheur souhaité, puis faites-le glisser et déposez-le sur la zone de travail.

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >Une campagne dynamique avec des déclencheurs s’exécute en mode _déclencheur_. Il s’exécute sur une personne à la fois en fonction des événements déclenchés et des filtres supplémentaires.

   >[!IMPORTANT]
   >
   >Lors de l’utilisation d’un champ booléen dans une liste dynamique de campagne de déclenchement, vous devez le définir explicitement sur « false » pour que le champ s’évalue correctement lors de l’exécution de la campagne.

1. Cliquez dans la liste déroulante et sélectionnez un opérateur.

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >Des lignes pointilleuses rouges indiquent des erreurs ou des informations manquantes. Si elle n’est pas corrigée, la campagne ne sera pas valide et ne s’exécutera pas.

   >[!TIP]
   >
   >Dans une campagne dynamique avec des déclencheurs et des filtres, les déclencheurs se trouvent en haut et, lorsqu’ils sont déclenchés, seules les personnes répondant aux critères de filtre passent par le flux.

1. Définissez le déclencheur.

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >Avec plusieurs déclencheurs, une personne passe par le flux si _ANY_ l’un des déclencheurs est activé.

Pour exécuter la campagne sur un ensemble de personnes en même temps, découvrez comment [ Définir une liste dynamique pour une campagne dynamique | Lot](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Ajouter une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
