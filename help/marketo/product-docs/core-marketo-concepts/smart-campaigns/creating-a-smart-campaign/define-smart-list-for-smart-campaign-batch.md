---
unique-page-id: 1146940
description: Définir une Liste intelligente pour une Campaign intelligente | Lot - Docs marketing - Documentation du produit
title: Définir une Liste intelligente pour une Campaign intelligente | Lot
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---


# Définir une Liste intelligente pour une Campaign intelligente | Lot {#define-smart-list-for-smart-campaign-batch}

Les listes intelligentes sont le mécanisme utilisé dans tout Marketo pour définir &quot;qui&quot; (quelles personnes) inclure, qu’il s’agisse d’un rapport, d’une liste ou d’une campagne intelligente. Voici comment définir une liste intelligente pour une campagne par lot.

1. Choisissez une campagne intelligente, puis cliquez sur **Liste intelligente**.

   ![](assets/campaignchoose-hand.png)

1. Tapez pour rechercher un filtre, puis faites-le glisser sur la trame. Répétez cette opération pour plusieurs filtres.

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >Une campagne intelligente avec uniquement des filtres s’exécute en mode **Batch**. Il trouve dans la base de données les personnes qui remplissent les critères en fonction des filtres et les exécute toutes à la fois dans le flux.

   >[!NOTE]
   >
   >Vous pouvez exécuter une campagne intelligente sur une personne à la fois en fonction des événements en direct en ajoutant des déclencheurs, ce qui place la campagne intelligente en mode **Déclencheur**.

1. Cliquez sur la liste déroulante et choisissez un opérateur de filtre pour le filtre choisi.

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >Des lignes rouges ondulantes indiquent des erreurs ou des informations manquantes. Si elle n’est pas corrigée, la campagne n’est pas valide et ne s’exécute pas.

1. Entrez la valeur du filtre.

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >Par défaut, les personnes qui respectent TOUTES les règles de liste intelligente sont qualifiées. Il est possible de le modifier en fonction de vos besoins de campagne. Consultez [Règles de Liste intelligente pour la logique complexe](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) pour en savoir plus.

   Pour déclencher sur les événements en direct une personne à la fois, apprenez comment [définir une Liste intelligente pour le Campaign intelligent | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Définir une Liste intelligente pour une Campaign intelligente | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Ajouter une étape de flux à un Campaign dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

