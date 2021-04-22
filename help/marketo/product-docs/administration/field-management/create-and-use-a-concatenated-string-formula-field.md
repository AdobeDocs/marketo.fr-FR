---
unique-page-id: 2360337
description: Créer et utiliser un champ de chaîne concaténée (formule) - Marketo Docs - Documentation du produit
title: Créer et utiliser un champ de chaîne concaténée (formule)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Créer et utiliser un champ de chaîne concaténée (formule) {#create-and-use-a-concatenated-string-formula-field}

Vous pouvez combiner des valeurs provenant de plusieurs champs ou créer une valeur conditionnelle à l’aide d’un champ de formule Marketo.

1. Accédez à **Admin** et cliquez sur **Gestion des champs**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. Cliquez sur **Nouveau champ personnalisé**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. Sélectionnez **Formule** pour le **Type**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. Saisissez un **nom** pour votre champ, puis cliquez sur **Créer**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. Recherchez et sélectionnez votre champ de formule, puis cliquez sur **Modifier les règles**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. Ajoutez deux options et définissez-les comme la capture d&#39;écran ci-dessous.

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >En savoir plus sur les [jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Vous pouvez désormais ajouter le champ de formule en tant que jeton dans un courrier électronique.

   ![](assets/seven.png)

>[!NOTE]
>
>Les champs de formule peuvent être utilisés dans des colonnes de landings page, de courriers électroniques et de listes dynamiques (ils ne sont pas exportés). Les courriers électroniques contenant des champs de formule peuvent **ne pas** être envoyés à l’aide d’une campagne par lot. Utilisez un [jeton de script de courrier électronique](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) dans ce scénario.

Bon travail ! Maintenant vous avez un champ intelligent qui sait quelle formule de salutation inclure en fonction du sexe. Amusez-vous avec ça et devenez créatif.
