---
unique-page-id: 2360403
description: Comparer l’efficacité du programme avec celle de l’analyseur de programmes - Documents Marketo - Documentation du produit
title: Comparer l’efficacité du programme avec l’analyseur de programme
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 1%

---

# Comparer l’efficacité des programmes avec l’[!UICONTROL analyseur de programmes] {#compare-program-effectiveness-with-the-program-analyzer}

Utilisez l’[!UICONTROL analyseur de programmes] pour identifier vos programmes les plus efficaces et les moins efficaces, en comparant les coûts du programme, l’acquisition des membres, le pipeline et les recettes.

>[!PREREQUISITES]
>
>[Créer un [!UICONTROL analyseur de programmes]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Cliquez sur **[!UICONTROL Analytics]**.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. Sélectionnez l’analyseur de programmes.

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. Modifiez la vue en **[!UICONTROL Par programme]**.

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. Utilisez le **[!UICONTROL filtre de canal]** pour réduire l’affichage à un ou deux canaux uniquement. Pour l&#39;instant, nous allons regarder les programmes dans le canal **[!UICONTROL Salon professionnel]**.

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >Pour filtrer rapidement les programmes sur un seul canal, sélectionnez **[!UICONTROL Affichage]** > **[!UICONTROL Par canal]**, cliquez sur la bulle de ce canal, puis cliquez sur le nom du canal dans la boîte de dialogue pop-up.

1. Utilisez le menu déroulant **[!UICONTROL Axe X]** pour choisir une mesure pour l’axe horizontal. Nous allons commencer par **[!UICONTROL Coût du programme]**.

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. Utilisez le menu déroulant **[!UICONTROL Axe Y]** pour choisir une mesure pour l’axe vertical. Choisissons **[!UICONTROL Nouveaux noms]** pour trouver des programmes qui sont bons pour capturer de nouvelles pistes.

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. Activez les curseurs pour effectuer un zoom avant.

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >Vous pouvez également essayer d&#39;améliorer votre vue en passant d&#39;une échelle linéaire à une échelle logarithmique, ou vice versa. Utilisez le menu **[!UICONTROL Échelle]** en haut.

1. Explorez le graphique qui en résulte.

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   Dans notre exemple, nous apprenons que la [!DNL Origami Expo] est bien meilleure que toutes les autres émissions de ce canal pour capturer de nouveaux noms, et à un coût moyen. Mais ce n&#39;est pas tout. Nous allons ajouter deux mesures supplémentaires pour mieux comprendre.

1. Utilisez le menu déroulant **[!UICONTROL Taille des bulles]** pour choisir une mesure à comparer en fonction de la taille des bulles. Nous choisirons **[!UICONTROL (FT) Revenue Won]** pour notre exemple.

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >De nombreuses mesures que vous pouvez choisir dans l’analyseur de programme sont disponibles avec les calculs Première touche (FT) et Multitouche (MT). Il est important de comprendre la [ différence entre l’attribution FT et MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Observez les bulles changer de taille dans votre graphique.

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   En ajoutant **[!UICONTROL (FT) Revenue Won]**, nous constatons rapidement que, bien que le [!DNL Origami Expo] ait acquis beaucoup de nouveaux noms, il en résulte relativement peu de chiffre d&#39;affaires. De plus, nous constatons que le programme [!DNL Paper Fest 12] reçoit moins de noms, mais de meilleurs noms, car il influence plus de revenus gagnés (plus grande bulle).

1. Utilisez le menu déroulant Couleur pour ajouter une quatrième mesure. Nous allons examiner le rapport **[!UICONTROL (FT) Revenus sur investissements]**.

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. Observez les couleurs changer dans votre graphique.

   ![](assets/image2014-9-17-18-3a55-3a47.png)

On voit que le programme [!DNL Paper Fest 12] influence non seulement plus de revenus (bulle plus importante), mais malgré son coût relativement élevé (tout à droite), il a le meilleur retour sur investissement (bulle la plus verte) de tous les programmes du canal [!UICONTROL salon professionnel].

>[!TIP]
>
>Vous pouvez rapidement comparer les programmes d’un canal avec ceux d’un autre. Utilisez simplement le **filtre de canal** en haut de la fenêtre pour ajouter d’autres canaux.

>[!MORELIKETHIS]
>
>* [Explorer les détails du programme et du canal avec l’[!UICONTROL analyseur de programmes]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Comparer l’efficacité des canaux avec l’[!UICONTROL analyseur de programmes]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)
