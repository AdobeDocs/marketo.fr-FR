---
unique-page-id: 2360337
description: Création et utilisation d’un champ de chaîne concaténée (formule) - Documents Marketo - Documentation du produit
title: Créer et utiliser un champ de chaîne concaténée (formule)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 9%

---

# Créer et utiliser un champ de chaîne concaténée (formule) {#create-and-use-a-concatenated-string-formula-field}

Vous pouvez combiner des valeurs provenant de plusieurs champs ou créer une valeur conditionnelle à l’aide d’un champ de formule Marketo Engage.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Cliquez sur **[!UICONTROL Gestion des champs]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Cliquez sur **[!UICONTROL Nouveau champ personnalisé]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Sélectionnez **[!UICONTROL Formule]** pour le **[!UICONTROL Type]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Saisissez un **[!UICONTROL Nom]** pour votre champ, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Recherchez et sélectionnez votre champ de formule, puis cliquez sur **[!UICONTROL Modifier les règles]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Ajoutez deux choix et définissez-les comme la capture d’écran ci-dessous.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >En savoir plus sur les [jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Vous pouvez maintenant ajouter le champ de formule sous la forme d’un jeton dans un e-mail.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Les champs de formule peuvent être utilisés dans les colonnes Pages de destination, E-mails et Liste dynamique. Les e-mails avec des champs de formule ne peuvent _pas_ être envoyés à l’aide d’une campagne par lots. Utilisez un [jeton de script d’e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) dans ce scénario.

Bon travail ! Vous disposez maintenant d’un champ intelligent qui sait quelle qualification inclure en fonction du genre. Amusez-vous avec ceci et soyez créatif.
