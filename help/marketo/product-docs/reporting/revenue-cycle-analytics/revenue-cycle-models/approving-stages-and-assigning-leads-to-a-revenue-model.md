---
unique-page-id: 4718683
description: Approbation des étapes et affectation de pistes à un modèle de recettes - Documents marketing - Documentation sur les produits
title: Approbation d'étapes et affectation de pistes à un modèle de recettes
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Approbation d&#39;étapes et affectation de pistes à un modèle de recettes {#approving-stages-and-assigning-leads-to-a-revenue-model}

Exécutez votre **modèle** de recettes **** en ajoutant des pistes existantes, en créant des règles d&#39;affectation pour toutes les nouvelles pistes.

## Approbation des étapes {#approving-stages}

Approuvons les étapes de votre modèle avant d&#39;ajouter des pistes.

1. Accédez à la **zone **Analytics.** **

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Sélectionnez le modèle dont vous souhaitez approuver les étapes.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Sous Actions **** du modèle, sélectionnez **Approuver** **les étapes**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Vous serez accueilli avec une alerte ; cliquez sur **Attribuer des pistes**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Excellent ! Passons à autre chose et affectons ces pistes.

## Affectation de pistes existantes {#assigning-existing-leads}

[Créez une Liste](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) dynamique pour identifier les pistes pour une étape de votre modèle dans votre base de données de pistes.

1. Une fois que vous avez [créé votre Liste](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)dynamique, cliquez sur l’onglet **Pistes** .

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Cliquez sur **Sélectionner tout** pour sélectionner les pistes.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Ouvrez la liste déroulante Actions **de** piste et sélectionnez **Spécial**. Cliquez sur **Modifier l’étape** des recettes.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Sélectionnez le **modèle** correct et la **phase** appropriée. Cliquez sur **Exécuter maintenant**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Répétez cette opération jusqu&#39;à ce que toutes vos pistes soient affectées aux différentes étapes de votre modèle.

Super ! Pour spécifier comment de nouvelles pistes sont affectées aux étapes, créez des règles d&#39;affectation.

>[!NOTE]
>
>Si votre modèle est à l&#39;état Etapes approuvées, aucun événement d&#39;étape Modifier les recettes ne s&#39;affichera dans les journaux d&#39;activité des pistes. Si votre modèle est entièrement approuvé, cette étape de flux sera ignorée si vous déplacez une piste dans la même étape qu&#39;elle est actuellement.

## Nouvelles pistes : Créer des règles d&#39;affectation  {#new-leads-create-assignment-rules}

1. Cliquez à nouveau sur** Accueil du marketing**, puis sélectionnez **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. `Click your model in the tree, then the`**`Model Actions`**`menu, selecting`**`Assignment Rules`** `.`

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. `If your assignment rules contain more than just one default choice click **Stage, **make your selection, then click`**`Add Choice`**`.`

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Exemple de règle d&#39;affectation {#example-assignment-rule}

Créez une règle Score de piste pour affecter les nouvelles pistes avec un score minimum à une étape appropriée.

1. Sous **Si**, sélectionnez Score de **piste**. Choisissez ensuite **au moins**.
` ![](assets/image2015-4-29-13-3a27-3a8.png)

   `

1. Saisissez **40** dans le champ et sélectionnez **Sales Lead** as a Stage (Pistecommerciale). Cliquez sur **Enregistrer** pour terminer.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!NOTE]
>
>**Articles connexes**
>
>Pour approuver votre modèle, lisez notre page d&#39;aide sur ** [Approbation et désapprobation d&#39;un modèle](approve-unapprove-a-revenue-model.md)de recettes**.

