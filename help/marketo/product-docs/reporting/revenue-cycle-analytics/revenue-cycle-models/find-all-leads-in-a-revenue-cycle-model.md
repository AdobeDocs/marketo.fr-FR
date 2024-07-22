---
unique-page-id: 2360423
description: Recherche de toutes les pistes dans un modèle de cycle de revenu - Documents Marketo - Documentation du produit
title: Recherche de toutes les pistes dans un modèle de cycle du revenu
exl-id: 428dbfa1-2f19-41ce-bfc6-e63edfdaba17
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Recherche de toutes les pistes dans un modèle de cycle du revenu {#find-all-leads-in-a-revenue-cycle-model}

En utilisant des listes dynamiques, vous pouvez facilement trouver tous les membres du modèle de cycle des recettes.

>[!PREREQUISITES]
>
>[Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Une fois la liste dynamique sélectionnée, cliquez sur l’onglet **Liste dynamique**.

   ![](assets/image2015-4-29-14-3a6-3a36.png)

1. Recherchez le filtre **Member of Revenue Model** et faites-le glisser dans la zone de travail.

   ![](assets/image2015-4-29-14-3a12-3a33.png)

1. Sélectionnez un **modèle**.

   ![](assets/image2015-5-13-18-3a2-3a23.png)

   Cela vous donnerait toutes les pistes de ce modèle, indépendamment de l&#39;étape. En règle générale, vous souhaitez une étape spécifique. Utilisez plutôt le filtre suivant.

1. Recherchez le filtre **Évaluation des recettes** et faites-le glisser dans la zone de travail.

   ![](assets/image2015-5-13-17-3a27-3a0.png)

1. Sélectionnez un **Stage**.

   ![](assets/image2015-5-13-17-3a31-3a9.png)

1. Accédez à l&#39;onglet **Leads** pour afficher les résultats.

   ![](assets/2.png)

   >[!TIP]
   >
   >Vous n’avez pas besoin des deux filtres, choisissez simplement celui dont vous avez besoin. Nous vous montrons tous les deux d&#39;être minutieux.

   >[!CAUTION]
   >
   >Si l’étape d’une piste est modifiée par une campagne externe lors de la création initiale de la piste, alors une activité n’est pas enregistrée dans la base de données. Cela signifie que le prospect ne sera pas inclus par le filtre de liste dynamique.
