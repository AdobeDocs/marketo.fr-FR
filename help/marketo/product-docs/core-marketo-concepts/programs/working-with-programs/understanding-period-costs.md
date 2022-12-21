---
unique-page-id: 7504676
description: Présentation des coûts de la période - Documents Marketo - Documentation du produit
title: Présentation des coûts de la période
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Présentation des coûts de la période {#understanding-period-costs}

## APERÇU {#overview}

Les coûts par période se rapportent à l’argent que vous dépensez au cours d’un mois spécifique pour un programme.

>[!NOTE]
>
>**Exemple**
>
>Si vous dépensez 1 000 $ pour engager un illustrateur dans un livre électronique lancé en juillet, le programme eBook aura un coût de 1 000 $ en juillet.
>
>Si vous dépensez 200 $ par mois dans Google AdWords, le programme Google AdWords aura un coût de 200 $ **chaque mois**.

>[!NOTE]
>
>[Présentation des programmes](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Compréhension de l’appartenance au programme](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Méthode de calcul des coûts de la période {#how-period-costs-are-calculated}

Imaginez un événement, comme un webinaire, qui se produit en mars. De nouvelles personnes sont acquises à l&#39;avance grâce à la publicité en janvier et février. De nouveaux contacts sont également acquis après l&#39;événement, lorsque les téléspectateurs téléchargent le webinaire dans les mois d&#39;avril et mai.

1. Avec un coût de période unique attribué au mois de mars...

   ![](assets/graph1.png)

   ...Les contacts ajoutés dans les mois précédant et suivant seront *only* comptez jusqu&#39;à mars.

   ![](assets/graph2.png)

1. Avec des coûts de période attribués à janvier, février et mars...

   ![](assets/graph3.png)

   ...Les contacts ajoutés uniquement dans les mois qui suivent le mois de mars seront pris en compte pour le mois de mars.

   ![](assets/graph4.png)

1. Avec des coûts de période attribués à janvier et avril...

   ![](assets/graph5.png)

   ...Les contacts ajoutés dans les mois de janvier à mars seront pris en compte pour janvier. Les contacts ajoutés au mois d&#39;avril et mai seront pris en compte jusqu&#39;au mois d&#39;avril.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >En résumé : les mois sans période définie sont décalés vers l’arrière vers le dernier mois défini. S’il n’y a aucun coût de période précédente, les mois seront reportés à la période suivante qui a été définie. Si un coût de période n’a pas été défini pour _any_ Les mois suivants, les rapports du RCE ne seront pas disponibles pour le programme.

   >[!MORELIKETHIS]
   >
   >* [Utilisation des coûts de période dans un programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtrage d’un rapport de programme par coût par période](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

