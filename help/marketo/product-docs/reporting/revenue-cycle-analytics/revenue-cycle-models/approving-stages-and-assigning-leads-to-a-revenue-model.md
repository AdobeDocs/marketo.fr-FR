---
unique-page-id: 4718683
description: Approbation d’étapes et affectation de leads à un modèle de chiffre d’affaires - Documents Marketo - Documentation du produit
title: Approuver des étapes et affecter des leads à un modèle de revenu
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Approuver des étapes et affecter des leads à un modèle de revenu {#approving-stages-and-assigning-leads-to-a-revenue-model}

Mettez en service votre **modèle de chiffre d’affaires** en ajoutant des prospects existants et en créant des règles d’affectation pour tous les nouveaux prospects.

## Approbation des étapes {#approving-stages}

Approuvons les étapes de votre modèle avant d’ajouter des prospects.

1. Accédez à la zone **[!UICONTROL Analytics]**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Sélectionnez le modèle dont vous souhaitez approuver les étapes.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Sous **[!UICONTROL Actions du modèle]**, sélectionnez **[!UICONTROL Approuver les étapes]**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Une alerte s’affichera à l’accueil ; cliquez sur **[!UICONTROL Attribuer les prospects]**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Excellent ! Passons à autre chose et attribuons ces prospects.

## Affecter des leads existants {#assigning-existing-leads}

[Créez une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) pour identifier les prospects d’une étape de votre modèle dans votre base de données de prospects.

1. Une fois que vous avez [créé votre liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), cliquez sur l’onglet **[!UICONTROL Prospects]**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Cliquez sur **[!UICONTROL Tout sélectionner]** pour sélectionner les prospects.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Ouvrez la liste déroulante **[!UICONTROL Actions de lead]** et sélectionnez **[!UICONTROL Spécial]**. Cliquez sur **[!UICONTROL Modifier l’étape Revenu...]**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Sélectionnez le **[!UICONTROL modèle]** et le **[!UICONTROL stade]** appropriés. Cliquez sur **[!UICONTROL Exécuter maintenant]**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Répétez cette opération jusqu’à ce que toutes vos pistes soient affectées aux différentes étapes de votre modèle.

Fantastique ! Pour spécifier comment les nouveaux prospects sont affectés aux étapes, créez des règles d’affectation.

>[!NOTE]
>
>Si votre modèle est à l’état Étapes approuvées , vous ne verrez aucun événement d’étape Modifier le chiffre d’affaires dans les journaux d’activité des prospects. Si votre modèle est entièrement approuvé, cette étape de flux est ignorée si vous déplacez un prospect vers l’étape dans laquelle il se trouve actuellement.

## Nouveaux Leads : Créer Des Règles D&#39;Affectation  {#new-leads-create-assignment-rules}

1. Cliquez de nouveau sur **Accueil Marketo** puis sélectionnez **[!UICONTROL Analytics]**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Cliquez sur votre modèle dans l&#39;arborescence, puis sur le menu **[!UICONTROL Actions du modèle]** en sélectionnant **[!UICONTROL Règles d&#39;affectation]**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Si vos règles d’affectation contiennent plusieurs choix par défaut, cliquez sur **[!UICONTROL Phase]**, effectuez votre sélection, puis cliquez sur **[!UICONTROL Ajouter un choix]**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Exemple de règle d’affectation {#example-assignment-rule}

Créez une règle [!UICONTROL Score du lead] pour affecter les nouveaux leads ayant un score minimum à une étape appropriée.

1. Sous **[!UICONTROL Si]**, sélectionnez **[!UICONTROL Score du lead]**. Choisissez ensuite **[!UICONTROL au moins]**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Saisissez **40** dans le champ et sélectionnez **[!UICONTROL Lead commercial]** comme [!UICONTROL Étape]. Cliquez sur **[!UICONTROL Enregistrer]** pour terminer.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Pour approuver votre modèle, consultez notre page d&#39;aide sur **[Approuver et annuler l&#39;approbation d&#39;un modèle de produit](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
