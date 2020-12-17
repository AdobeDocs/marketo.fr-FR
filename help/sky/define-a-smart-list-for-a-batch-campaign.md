---
title: définir-une-liste-intelligente-pour-une-campagne-par-lot
description: Définir une Liste dynamique pour un Campaign par lot
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---


# Définir une Liste dynamique pour un Campaign par lot

<br> 

Les listes intelligentes sont le mécanisme utilisé dans tout Marketo pour définir &quot;qui&quot; (quelles personnes) inclure, qu’il s’agisse d’un rapport, d’une liste ou d’une campagne intelligente. Voici comment définir une liste intelligente pour une campagne par lot.

1. Choisissez une campagne intelligente, puis cliquez sur **[!UICONTROL Liste intelligente]**.

   ![Image un](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. Tapez pour rechercher un filtre, puis faites-le glisser sur la trame. Répétez cette opération pour plusieurs filtres.

   ![Image 2](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >Une campagne intelligente avec uniquement des filtres s’exécute en mode Batch. Il trouve dans la base de données les personnes qui remplissent les critères en fonction des filtres et les exécute toutes à la fois dans le flux.

   >[!IMPORTANT]
   >
   >Vous pouvez exécuter une campagne dynamique sur une personne à la fois en fonction des événements en direct en ajoutant des déclencheurs, ce qui place la campagne dynamique en mode Déclencheur.

1. Cliquez sur la liste déroulante et choisissez un opérateur de filtre (ex. **[!UICONTROL est]**, **[!UICONTROL n&#39;est pas]**, etc.) pour le filtre que vous avez choisi.

   ![Image trois](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >Les lignes rouges indiquent des erreurs ou des informations manquantes. Si elle n’est pas corrigée, la campagne n’est pas valide et ne s’exécute pas.

1. Entrez la valeur du filtre.

   ![Image 4](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>Par défaut, les personnes qui respectent TOUTES les règles de liste intelligente sont
>qualifié. Il est possible de le modifier en fonction de vos besoins de campagne. Consultez [Règles de Liste intelligente pour la logique complexe](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic) pour en savoir plus.
>
>Pour déclencher sur les événements en direct une personne à la fois, apprenez comment [définir une Liste intelligente pour le Campaign intelligent | Déclencheur](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger).
