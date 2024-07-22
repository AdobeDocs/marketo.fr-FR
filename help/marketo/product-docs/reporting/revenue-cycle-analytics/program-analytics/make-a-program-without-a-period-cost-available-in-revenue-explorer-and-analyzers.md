---
unique-page-id: 2360389
description: Rendre un programme sans coût de période disponible dans l’Explorateur de recettes et les Analyseurs - Documents Marketo - Documentation du produit
title: Rendre un programme sans coût de période disponible dans l’Explorateur des recettes et les Analyseurs
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Rendre un programme sans coût de période disponible dans l’Explorateur des recettes et les Analyseurs {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Les coûts de la période de programme vous permettent de définir &quot;combien d’argent&quot; et &quot;quand&quot; pour un programme. Cela s’affiche dans l’Explorateur de Recettes Cycle et les [analyseurs](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Certains programmes peuvent avoir besoin d&#39;être inclus même s&#39;ils n&#39;ont pas de coût de période. Bien que vous puissiez saisir 0 pour le coût de la période, nous avons facilité l’inclusion de ces programmes.

>[!NOTE]
>
>L’analyseur de programme associe la réussite du programme par coût de période. Si aucun coût de période n’est disponible, la fonction Succès du programme ne s’affiche pas, quel que soit le comportement d’analyse du programme. Si le comportement d’analyse est configuré, les données s’affichent pour les mesures d’opportunités (opportunités de pipeline, recettes générées, etc.).

1. Dans la section Admin, cliquez sur **Balises**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Développez vos canaux et double-cliquez sur le canal de votre choix.

   >[!NOTE]
   >
   >Tous les programmes utilisant ce canal, quel que soit le coût par période, seront disponibles pour les explorateurs et analyseurs de recettes. Ce changement prendra effet le lendemain.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Définissez le comportement d’Analytics sur Inclusif et cliquez sur **Enregistrer**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Avez-vous remarqué l&#39;option Opérationnelle ? Cela fait le contraire. Il exclut ces programmes, quel que soit le coût de la période.

Beau boulot ! Désormais, tout programme utilisant le canal modifié sera inclus dans l’explorateur de recettes et les analyseurs sans avoir à subir de coût de période.

>[!MORELIKETHIS]
>
>[Remplacer le comportement d’Analytics au niveau du programme](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
