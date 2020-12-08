---
unique-page-id: 7504676
description: Comprendre les coûts de la période - Documents marketing - Documentation du produit
title: Comprendre les coûts de la période
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Comprendre les coûts de la période {#understanding-period-costs}

## Présentation {#overview}

Les coûts périodiques se rapportent à l&#39;argent que vous dépensez au cours d&#39;un mois donné sur un programme.

>[!NOTE]
>
>**Exemple**
>
>Si vous dépensez 1 000 $ pour embaucher un illustrateur pour un eBook qui démarre en juillet, le programme eBook coûterait 1 000 $ en juillet.
>
>Si vous dépensez 200 dollars par mois dans Google Adwords - le programme Google Adwords coûterait 200 dollars **par mois**.

>[!NOTE]
>
>**Plongée profonde**
>
>[Présentation des Programmes](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Comprendre l&#39;appartenance à un Programme](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Méthode de calcul des coûts de la période {#how-period-costs-are-calculated}

Imaginez un événement, comme un webinaire, qui se déroule en mars. De nouvelles personnes sont acquises à l&#39;avance grâce à la publicité en janvier et février. De nouveaux contacts sont également acquis après le événement, lorsque les gens téléchargent le webinaire dans les mois d&#39;avril et mai.

1. Avec un coût de période unique attribué à Mars...

   ![](assets/graph1.png)

   ...les contacts ajoutés dans les mois précédant et suivant ne seront *comptés que* vers mars.

   ![](assets/graph2.png)

1. Avec des coûts de période attribués à janvier, février et mars...

   ![](assets/graph3.png)

   ...les contacts ajoutés seulement dans les mois qui suivent mars seront comptés pour mars.

   ![](assets/graph4.png)

1. Avec les coûts de la période attribués à janvier et avril...

   ![](assets/graph5.png)

   ...les contacts ajoutés dans les mois de janvier à mars compteront pour janvier. Les contacts ajoutés dans les mois d&#39;avril et mai seront comptés vers avril.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >En résumé - les mois sans période définie les coûts remontent &quot;en arrière&quot; à la dernière période définie. S&#39;il n&#39;y a pas de coût pour la période antérieure, les mois seront reportés à la période suivante définie. Si un coût de période n&#39;a pas été défini pour *un mois* , le rapports en RCE ne sera pas disponible pour le programme.

   >[!NOTE]
   >
   >**Articles connexes**
   >
   >    
   >    
   >    * [Utilisation des coûts de période dans un Programme](using-period-costs-in-a-program.md)
   >    * [Filtrage d&#39;un rapport Programme par coût de période](../../../../product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)


