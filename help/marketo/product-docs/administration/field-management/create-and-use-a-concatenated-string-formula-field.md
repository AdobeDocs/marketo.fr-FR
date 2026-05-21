---
unique-page-id: 2360337
description: Combinez des valeurs provenant de plusieurs champs ou créez des valeurs conditionnelles à l’aide de champs de formule dans Marketo Engage.
title: Créer et utiliser un champ de chaîne concaténée (formule)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
TQID: https://experienceleague.adobe.com/Yk-Xh-WHUE8-GR2KTCxXRSqerdz-JHu2JnzYp8tAq9U
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 148
ht-degree: 10%

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
