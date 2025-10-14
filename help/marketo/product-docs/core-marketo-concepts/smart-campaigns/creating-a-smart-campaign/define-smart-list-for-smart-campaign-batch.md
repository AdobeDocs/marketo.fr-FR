---
unique-page-id: 1146940
description: Définir une liste dynamique pour une campagne dynamique | Lot - Documents Marketo - Documentation Du Produit
title: Définir une liste intelligente pour une campagne intelligente | Par lots
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 5%

---

# Définir une liste intelligente pour une campagne intelligente | Par lots {#define-smart-list-for-smart-campaign-batch}

Les listes dynamiques sont le mécanisme utilisé dans Marketo Engage pour définir les « personnes » à inclure, qu’il s’agisse d’un rapport, d’une liste ou d’une campagne dynamique. Voici comment définir une liste dynamique pour une campagne par lots.

>[!CAUTION]
>
>Apporter des modifications à une liste dynamique ou à une étape de flux à une campagne active peut potentiellement interrompre sa fonctionnalité. Si vous choisissez de le faire, faites preuve de prudence.

1. Choisissez une campagne dynamique, puis cliquez sur **[!UICONTROL Liste dynamique]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Saisissez pour rechercher un filtre, puis faites-le glisser et déposez-le sur la zone de travail. Répétez l’opération pour plusieurs filtres.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Une campagne dynamique avec uniquement des filtres s’exécute en mode _lot_. Il trouve dans la base de données les personnes qui remplissent les critères en fonction des filtres et les exécute toutes en même temps dans le flux.

   >[!NOTE]
   >
   >Vous pouvez faire en sorte qu’une campagne intelligente s’exécute sur une personne à la fois en fonction d’événements en direct en ajoutant des déclencheurs, ce qui place la campagne intelligente en mode _déclencheur_.

1. Cliquez dans la liste déroulante et choisissez un opérateur de filtre pour le filtre que vous avez choisi.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Des lignes pointilleuses rouges indiquent des erreurs ou des informations manquantes. Si elle n’est pas corrigée, la campagne ne sera pas valide et ne s’exécutera pas.

1. Saisissez la valeur du filtre.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Par défaut, les personnes qui répondent à TOUTES les règles de liste dynamique sont qualifiées. Elle peut être modifiée en fonction de vos besoins de campagne. Consultez [Règles de liste dynamique pour une logique complexe](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} pour en savoir plus.

   Pour déclencher des événements en direct une personne à la fois, découvrez comment [Définir une liste dynamique pour une campagne dynamique | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [Définir une liste dynamique pour une campagne dynamique | Déclencheur &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [Ajouter une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
