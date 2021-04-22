---
unique-page-id: 1146980
description: Utiliser le choix d'Ajoute dans une étape de flux - Marketo Docs - Documentation du produit
title: Utiliser le choix des Ajoutes dans une étape de flux
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Utiliser le choix d&#39;Ajoute dans une étape de flux {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Ajouter une étape de flux à un Campaign dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

**Ajoutez** Choicelets vous utilisez une étape de flux et dites &quot;Ça dépend&quot; lorsque vous choisissez les détails.

1. Sous l&#39;onglet **Flux** de la campagne dynamique, ajoutez toute étape de flux, puis cliquez sur **Ajouter le choix**.

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. Sélectionnez la condition de choix.

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. Sélectionnez l’opérateur de choix et entrez une valeur de choix. Cela définit vos critères ou choix.

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. Entrez une valeur d&#39;étape de flux pour le choix.

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >Les jetons **ne fonctionnent pas** dans la partie condition d’une étape de flux de choix.

1. Répétez les étapes ci-dessus pour ajouter plusieurs choix, puis ajoutez/ajustez la valeur par défaut.

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >Vous pouvez définir l&#39;une de vos étapes de flux sur —Do Nothing—, auquel cas aucune action ne sera entreprise sur ce choix.

   >[!CAUTION]
   >
   >Seul le premier choix de correspondance est appliqué à l’étape de flux. Découvrez comment [réorganiser &quot;Choix d&#39;Ajoute&quot; dans une action de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md).

   Fantastique ! Vous pouvez désormais créer une seule campagne dynamique avec des choix d’étape de flux au lieu de créer plusieurs campagnes dynamiques pour chaque choix.

   >[!MORELIKETHIS]
   >
   >[Réorganiser le choix des Ajoutes à une étape de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md)
