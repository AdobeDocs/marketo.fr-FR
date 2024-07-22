---
unique-page-id: 6848782
description: Rendre votre message de désabonnement dynamique pour les langues - Documents Marketo - Documentation du produit
title: Rendre votre message de désabonnement dynamique pour les langues
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 3%

---

# Rendre votre message de désabonnement dynamique pour les langues {#make-your-unsubscribe-message-dynamic-for-languages}

Le message de désabonnement et le lien par défaut sont en anglais. Vous pouvez utiliser du contenu dynamique pour l’afficher dans différentes langues.

>[!NOTE]
>
>Cet article représente une bonne pratique, mais il peut être réalisé d’autres façons.

## Préparation des données {#prepare-your-data}

1. [Créez un champ personnalisé](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) nommé &quot;Langue préférée&quot;. (Configurez-le dans votre CRM si vous souhaitez que ce champ soit synchronisé).

   >[!TIP]
   >
   >À l’avenir, utilisez ce champ lorsque vous [ créez un formulaire](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) pour capturer les préférences linguistiques.

## Créer une segmentation {#create-segmentation}

1. Accédez à la **[!UICONTROL base de données]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. Dans la liste déroulante **[!UICONTROL Nouveau]**, cliquez sur **[!UICONTROL Nouvelle segmentation]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Nommez la segmentation **[!UICONTROL Langue préférée]**. Cliquez sur **[!UICONTROL Ajouter un segment]**. Saisissez une langue.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >Le segment par défaut est Anglais.

1. Continuez à ajouter des segments jusqu’à ce que toutes vos langues soient représentées. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Sélectionnez un segment.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Accédez à l’onglet **[!UICONTROL Liste dynamique]** . Saisissez la **[!UICONTROL langue préférée]** dans le champ de recherche. Faites glisser le filtre sur la zone de travail.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Définissez la langue appropriée.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Répétez cette opération pour toutes vos langues. Sélectionnez ensuite la liste déroulante **[!UICONTROL Actions de segmentation]** et cliquez sur **[!UICONTROL Approuver]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Création d’un fragment de code {#create-a-snippet}

1. Accédez à **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. Dans la liste déroulante **[!UICONTROL New]**, cliquez sur **[!UICONTROL New Snippet]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Nommez le fragment de code **Unsubscribe Message**. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Saisissez votre message de désabonnement par défaut, mettez-le en surbrillance, puis cliquez sur l’icône de lien hypertexte.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Copiez et collez ce jeton : `{{system.unsubscribeLink}}` dans le champ **[!UICONTROL URL]** . Cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Sélectionnez **[!UICONTROL Segment par]** dans la section **[!UICONTROL Segmentation]** .

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. Dans la liste déroulante **[!UICONTROL Segmentation]**, saisissez **[!UICONTROL Préféré]** et sélectionnez **[!UICONTROL Langue préférée]**. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Sélectionnez un segment dans l’arborescence. Cliquez sur votre désabonnement puis sur l’icône de lien.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Assurez-vous que `{{system.unsubscribeLink}}` se trouve toujours dans le champ **[!UICONTROL URL]** . Modifiez le **[!UICONTROL texte d’affichage]** pour qu’il corresponde à la langue que vous avez sélectionnée. Cliquez sur **[!UICONTROL Apply]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Répétez l’opération pour tous vos segments. Ensuite, revenez à **[!UICONTROL Design Studio]**, cliquez sur la liste déroulante **[!UICONTROL Actions de fragment de code]**, puis cliquez sur **[!UICONTROL Approuver]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

C&#39;est génial. Presque là !

## Utiliser un fragment de code dans un courrier électronique {#use-snippet-in-an-email}

1. Dans l&#39;éditeur d&#39;email, cliquez sur l&#39;élément éditable. Cliquez ensuite sur l’icône d’engrenage et sélectionnez **[!UICONTROL Remplacer par l’extrait de code]**. Si vous sélectionnez un élément de fragment de code modifiable, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Modifier]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Recherchez et sélectionnez votre fragment de code dans la liste déroulante, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Pour le tester, cliquez sur **[!UICONTROL Précédent]**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...puis l’onglet **[!UICONTROL Dynamique]** .

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Cliquez sur les différentes langues pour afficher le changement du fragment de code.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >Bien sûr, vous pouvez également éditer le reste de votre email pour le langage dynamique. Pendant que vous y êtes, effectuez la même technique sur la page de désabonnement.

## Personnalisation de votre page de désabonnement avec du contenu dynamique {#customizing-your-unsubscribe-page-with-dynamic-content}

Si vous souhaitez que vos visiteurs consultent une page de désabonnement dans la langue de leur choix, vous pouvez utiliser du contenu dynamique sur la landing page et la page de confirmation.

1. Accédez à **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Saisissez _Unsubscribe_ dans le champ de recherche et sélectionnez la page Unsubscribe de votre choix.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Sélectionnez **[!UICONTROL Segment Par]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Recherchez le segment **[!UICONTROL Langue préférée]** . Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   Editez votre contenu pour chaque landing page, validez, et vous n&#39;avez rien à faire !

   >[!NOTE]
   >
   >En savoir plus sur [contenu dynamique](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) et toutes les choses cool que vous pouvez faire.
