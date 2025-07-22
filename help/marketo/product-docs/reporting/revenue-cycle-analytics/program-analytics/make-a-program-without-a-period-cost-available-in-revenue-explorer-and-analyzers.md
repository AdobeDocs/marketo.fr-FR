---
unique-page-id: 2360389
description: Mise à disposition d’un programme sans coût de période dans l’Explorateur et les analyseurs de revenus - Documents Marketo - Documentation du produit
title: Rendre un programme sans coût de période disponible dans l’explorateur et les analyseurs de revenus
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Rendre un programme sans coût de période disponible dans l’explorateur et les analyseurs de revenus {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Les coûts de la période du programme vous permettent de définir « combien d’argent » et « quand » pour un programme. Cela s’affiche dans l’Explorateur du cycle du chiffre d’affaires et [analyseurs](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Il se peut que certains programmes doivent être inclus même s&#39;ils n&#39;ont pas de coût de période. Bien que vous puissiez entrer 0 pour le coût de la période, nous avons facilité l&#39;inclusion de ces programmes.

>[!NOTE]
>
>L’analyseur de programmes regroupe les Succès du programme par coût de période. Si aucun coût de période n’est disponible, le succès du programme ne s’affiche pas, quel que soit le comportement d’analyse du programme. Si le comportement d’analyse est configuré, les données s’affichent pour les mesures d’opportunité (opportunités de pipeline, chiffre d’affaires gagné, etc.).

1. Dans la section [!UICONTROL Admin], cliquez sur **[!UICONTROL Balises]**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Développez vos Chaînes et double-cliquez sur la chaîne de votre choix.

   >[!NOTE]
   >
   >Tous les programmes utilisant ce canal, quel que soit le coût de la période, seront disponibles pour l’explorateur et les analyseurs de chiffre d’affaires. Cette modification prendra effet le jour suivant.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Modifiez le [!UICONTROL Comportement d’Analytics] en **Inclusif**, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Avez-vous remarqué l&#39;option Opérationnelle ? Cela fait le contraire. Il exclut ces programmes quel que soit le coût de la période.

Joli travail ! Désormais, tout programme utilisant le canal modifié sera inclus dans l’explorateur et les analyseurs de chiffre d’affaires sans avoir besoin d’un coût de période.

>[!MORELIKETHIS]
>
>[Remplacer le comportement d’Analytics au niveau du programme](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
