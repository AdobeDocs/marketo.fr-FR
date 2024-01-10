---
unique-page-id: 2360337
description: Créer et utiliser un champ de chaîne concaténée (formule) - Documents Marketo - Documentation du produit
title: Créer et utiliser un champ de chaîne concaténée (formule)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 9181a599ae715e9ffcfd84d8316dfa1c094329a6
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Créer et utiliser un champ de chaîne concaténée (formule) {#create-and-use-a-concatenated-string-formula-field}

Vous pouvez combiner des valeurs provenant de plusieurs champs ou créer une valeur conditionnelle à l’aide d’un champ de formule de Marketo Engage.

1. Accédez au **[!UICONTROL Administration]** zone.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Cliquez sur **[!UICONTROL Gestion des champs]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Cliquez sur **[!UICONTROL Nouveau champ personnalisé]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Sélectionner **[!UICONTROL Formule]** pour le **[!UICONTROL Type]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Saisissez un **[!UICONTROL Nom]** pour votre champ, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Recherchez et sélectionnez votre champ de formule, puis cliquez sur **[!UICONTROL Modifier des règles]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Ajoutez deux options et définissez-les comme la capture d’écran ci-dessous.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >En savoir plus sur [jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Vous pouvez maintenant ajouter le champ de formule en tant que jeton dans un email.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Les champs de formule peuvent être utilisés dans les colonnes Pages d’entrée, Emails et Liste dynamique . Les emails contenant des champs de formule peuvent _not_ être envoyé à l’aide d’une campagne par lots. Veuillez utiliser un [jeton de script de courrier électronique](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) dans ce scénario.

Bon travail ! Vous avez maintenant un champ intelligent qui sait quelle formule de salutation inclure en fonction du genre. Amuse-toi bien avec ça et deviens créatif.
