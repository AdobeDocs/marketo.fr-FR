---
title: définir-une-liste-intelligente-pour-une-campagne-par-lot
description: Définir une Liste dynamique pour un Campaign par lot
exl-id: 35130f40-cce5-4677-8eaf-f9d73c995ba3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Définir une Liste dynamique pour un Campaign par lot

<br> 

Les listes intelligentes sont le mécanisme utilisé dans toute Marketo pour définir &quot;qui&quot; (quelles personnes) inclure, que ce soit un rapport, une liste ou une campagne intelligente. Voici comment définir une liste intelligente pour une campagne par lot.

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
