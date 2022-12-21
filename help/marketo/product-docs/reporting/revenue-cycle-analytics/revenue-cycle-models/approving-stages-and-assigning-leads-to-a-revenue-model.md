---
unique-page-id: 4718683
description: Approbation des étapes et attribution de pistes à un modèle de revenu - Documents Marketo - Documentation du produit
title: Approbation des étapes et attribution de pistes à un modèle de revenu
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Approbation des étapes et attribution de pistes à un modèle de revenu {#approving-stages-and-assigning-leads-to-a-revenue-model}

Obtenez votre **Modèle Recettes** être opérationnel en ajoutant des pistes existantes, en créant des règles d’attribution pour toutes les nouvelles pistes.

## Approbation des étapes {#approving-stages}

Approuvons les étapes de votre modèle avant d’ajouter des pistes.

1. Accédez au **Analytics** zone.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Sélectionnez le modèle dont vous souhaitez approuver les étapes.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Sous **Actions de modèle**, sélectionnez **Approuver les étapes**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Vous serez accueilli par une alerte ; click **Attribuer des pistes**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Excellent ! Passons à ces pistes.

## Attribution de pistes existantes {#assigning-existing-leads}

[Création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) pour identifier les pistes pour une étape de votre modèle dans votre base de données de pistes.

1. Une fois que vous avez [création de votre liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), cliquez sur le bouton **Pistes** .

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Cliquez sur **Tout sélectionner** pour sélectionner les pistes.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Ouvrez le **Actions de piste** et sélectionnez **Spécial**. Cliquez sur **Modifier l’étape des recettes**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Sélectionnez la **Modèle** et le **Évaluation**. Cliquez sur **Exécuter maintenant**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Répétez cette opération jusqu’à ce que toutes vos pistes soient affectées aux différentes étapes de votre modèle.

Fantastique ! Pour spécifier comment de nouvelles pistes sont affectées aux scènes, créez des règles d’attribution.

>[!NOTE]
>
>Si votre modèle se trouve à l’état Étapes approuvées, aucun événement Étape du chiffre d’affaires des modifications n’apparaît dans les journaux d’activité des pistes. Si votre modèle est entièrement approuvé, cette étape de flux sera ignorée si vous déplacez une piste dans la même étape qu’actuellement.

## Nouvelles pistes : Création de règles d’affectation  {#new-leads-create-assignment-rules}

1. Cliquez sur **Accueil de Marketo** de nouveau, puis sélectionnez **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Cliquez sur votre modèle dans l’arborescence, puis sur **Actions de modèle** , en sélectionnant **Règles d’affectation**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Si vos règles d’affectation contiennent plusieurs clics de choix par défaut **Évaluation**, effectuez votre sélection, puis cliquez sur **Ajouter un choix**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Exemple de règle d’affectation {#example-assignment-rule}

Créez une règle Score de piste pour attribuer aux nouvelles pistes avec un score minimal une étape appropriée.

1. Sous **If**, sélectionnez **Score de piste**. Sélectionnez **au moins**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Entrée **40** dans le champ et sélectionnez **prospect** comme une scène. Cliquez sur **Enregistrer** pour terminer.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Pour approuver votre modèle, consultez notre page d’aide sur **[Approbation et annulation de l’approbation d’un modèle de recette](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
