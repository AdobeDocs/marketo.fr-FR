---
unique-page-id: 1146940
description: Définir une Liste intelligente pour une Campaign intelligente | Lot - Marketo Docs - Documentation du produit
title: Définir une Liste intelligente pour une Campaign intelligente | Lot
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Définir une Liste intelligente pour une Campaign intelligente | Lot {#define-smart-list-for-smart-campaign-batch}

Les listes intelligentes sont le mécanisme utilisé dans toute Marketo pour définir &quot;qui&quot; (quelles personnes) inclure, que ce soit un rapport, une liste ou une campagne intelligente. Voici comment définir une liste intelligente pour une campagne par lot.

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

