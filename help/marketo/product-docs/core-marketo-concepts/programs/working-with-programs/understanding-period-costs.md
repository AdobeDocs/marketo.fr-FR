---
unique-page-id: 7504676
description: Comprendre les coûts de la période - Documents Marketo - Documentation du produit
title: Comprendre les coûts de la période
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
feature: Programs
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# Comprendre les coûts de la période {#understanding-period-costs}

## Vue d’ensemble {#overview}

Les coûts de la période font référence aux sommes que vous avez dépensées au cours d’un mois spécifique pour un programme.

>[!NOTE]
>
>**Exemple**
>
>Si vous dépensez 1 000 $ pour embaucher un illustrateur pour une [!DNL eBook] qui débute en juillet, le programme [!DNL eBook] aurait un coût de période de 1 000 $ en juillet.
>
>Si vous dépensez 200 $ par mois en [!DNL Google Adwords] - le programme [!DNL Google Adwords] aurait un coût de période de 200 $ _chaque mois_.

>[!NOTE]
>
>[Présentation des programmes](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Comprendre l’appartenance à un programme](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Méthode de calcul des coûts de la période {#how-period-costs-are-calculated}

Imaginez un événement, comme un webinaire, qui a lieu en mars. De nouvelles personnes sont acquises au préalable à partir de la publicité en janvier et février. De nouveaux contacts sont également acquis après l’événement, lorsque les gens téléchargent le webinaire en avril et en mai.

1. Avec un coût de période unique attribué à mars...

   ![](assets/graph1.png)

   ...les contacts ajoutés au cours des mois précédents et suivants _uniquement_ compteront vers le mois de mars.

   ![](assets/graph2.png)

1. Avec les coûts de la période attribués à janvier, février et mars...

   ![](assets/graph3.png)

   ...les contacts ajoutés seulement dans les mois suivant mars compteront vers mars.

   ![](assets/graph4.png)

1. Avec les coûts de la période attribués à janvier et avril...

   ![](assets/graph5.png)

   ...les contacts ajoutés dans les mois de janvier à mars seront comptabilisés vers janvier. Les contacts ajoutés au cours des mois d’avril et de mai seront comptabilisés dans le courant du mois d’avril.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >En résumé, les mois sans période définie pour les coûts seront rétrogradés au dernier mois défini. S&#39;il n&#39;existe aucun coût de la période précédente, les mois sont reportés au suivant qui a été défini. Si un coût de période n&#39;a pas été défini pour _n&#39;importe quel_ mois, la déclaration en RCE ne sera pas disponible pour le programme.

   >[!MORELIKETHIS]
   >
   >* [Utilisation des coûts de période dans un programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtrer un rapport de programme par coût de période](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)
