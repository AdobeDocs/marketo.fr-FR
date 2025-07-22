---
unique-page-id: 2360401
description: Comparer l’efficacité des canaux avec l’analyseur de programme - Documents Marketo - Documentation du produit
title: Comparer l’efficacité des canaux avec l’analyseur de programmes
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# Comparaison de l’efficacité des canaux avec l’[!UICONTROL analyseur de programmes] {#compare-channel-effectiveness-with-the-program-analyzer}

Utilisez l’[!UICONTROL analyseur de programmes] pour comparer les coûts des canaux, l’acquisition de membres, le pipeline, le chiffre d’affaires, etc., afin d’identifier vos canaux les plus et les moins efficaces.

>[!PREREQUISITES]
>
>[Créer un [!UICONTROL analyseur de programmes]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Cliquez sur **[!UICONTROL Analytics]** dans **Mon Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Sélectionnez l’analyseur de programmes.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Modifiez la Vue en **[!UICONTROL Par canal]**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Utilisez le menu déroulant **[!UICONTROL Axe X]** pour choisir une mesure pour l’axe horizontal. Commençons par **[!UICONTROL Coût du programme]**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Utilisez le menu déroulant **[!UICONTROL Axe Y]** pour choisir une mesure pour l’axe vertical. Nous allons maintenant passer au pipeline **[!UICONTROL (FT) créé]**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >De nombreuses mesures que vous pouvez choisir dans l’analyseur de programme sont disponibles avec les calculs Première touche (FT) et Multitouche (MT). Il est important de comprendre la [ différence entre l’attribution FT et MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Utilisez le menu déroulant **[!UICONTROL Axe Y]** pour choisir **[!UICONTROL Pipeline MT créé]**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   Dans cette vue d’attribution multipoint, nous constatons que le canal Webinaire a plus d’influence sur le pipeline créé et coûte moins cher que les canaux Salon professionnel et Advertising en ligne.

   Ajoutons maintenant deux dimensions supplémentaires.

1. Utilisez le menu déroulant **[!UICONTROL Taille de bulle]** pour sélectionner une mesure supplémentaire, telle que **[!UICONTROL Nouveaux noms]**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Observez comment le graphique change.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Nous constatons que le canal Webinaire se rétrécit, comme le montrent les mesures **[!UICONTROL Nouveaux noms]**. Nous pouvons conclure que, bien qu&#39;elle compte de nombreux membres, elle est moins efficace pour générer de nouvelles pistes que le canal du salon professionnel.

1. Enfin, utilisez la liste déroulante Couleur pour ajouter la quatrième dimension. Sélectionnons **[!UICONTROL (FT) Chiffre d’affaires gagné]**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Observez les couleurs changer dans votre graphique.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   À partir des couleurs, nous apprenons que le canal du salon professionnel, la bulle la plus verte, a influencé le plus grand chiffre d&#39;affaires gagné, mesuré par l&#39;attribution première touche.

1. Désormais, si nous modifions la mesure Couleur en **[!UICONTROL (MT) Chiffre d’affaires gagné]**, nous constatons que le canal Advertising en ligne, désormais le plus vert, a influencé plus de chiffres d’affaires _au fil du temps_ que les canaux Webinaire et Salon professionnel.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

Dans notre exemple, nous constatons que le canal du salon professionnel est à la fois le plus cher (le plus à droite) et le plus réussi (le plus haut sur l’axe Y) lors de la mesure du pipeline créé par la première touche. Examinons à présent le pipeline de chaque canal créé tel qu’il est mesuré par l’attribution multipoint.

>[!TIP]
>
>Les exemples de ces étapes mesurent l’efficacité en fonction du pipeline créé. Utilisez le menu déroulant [!UICONTROL Axe Y] pour sélectionner d’autres méthodes de mesure de l’efficacité des canaux, telles que [!UICONTROL Nouveaux noms], [!UICONTROL Membres], [!UICONTROL Coût par succès], etc.

>[!MORELIKETHIS]
>
>* [Explorer les détails du programme et du canal avec l’[!UICONTROL analyseur de programmes]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Comparer l’efficacité du programme avec l’[!UICONTROL Analyseur de programmes]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)
