---
unique-page-id: 6848782
description: Utilisez le contenu dynamique et la segmentation pour afficher le message de désabonnement et le lien dans différentes langues.
title: Rendre votre message de désabonnement dynamique pour les langues
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
feature: Email Setup
TQID: https://experienceleague.adobe.com/K4c0CGEKTpE-BbYd1i6f24B8L9oltiBYo3AhI6cHHPE
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 472
ht-degree: 8%

---

# Rendre votre message de désabonnement dynamique pour les langues {#make-your-unsubscribe-message-dynamic-for-languages}

Le message et le lien de désabonnement par défaut sont en anglais. Vous pouvez utiliser du contenu dynamique pour les afficher dans différentes langues.

>[!NOTE]
>
>Cet article représente une bonne pratique, mais il peut être réalisé d’autres façons.

## Préparation des données {#prepare-your-data}

1. [Créez un champ personnalisé](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) appelé « Langue préférée ». (Configurez-le dans votre CRM si vous souhaitez que ce champ soit synchronisé).

   >[!TIP]
   >
   >À l’avenir, utilisez ce champ lorsque vous [créez un formulaire](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) pour capturer les préférences linguistiques.

## Créer une segmentation {#create-segmentation}

1. Accédez à la **[!UICONTROL Base de données]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. Dans la liste déroulante **[!UICONTROL Nouveau]**, cliquez sur **[!UICONTROL Nouvelle segmentation]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Nommez la segmentation **[!UICONTROL Langue préférée]**. Cliquez sur **[!UICONTROL Ajouter un segment]**. Saisissez une langue.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >Le segment par défaut sera l’anglais.

1. Continuez à ajouter des segments jusqu’à ce que toutes les langues soient représentées. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Sélectionnez un segment.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Accédez à l’onglet **[!UICONTROL Liste intelligente]**. Saisissez **[!UICONTROL Langue préférée]** dans le champ de recherche. Faites glisser et déposez le filtre sur la zone de travail.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Définissez la langue correspondante appropriée.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Répétez l’opération pour toutes vos langues. Sélectionnez ensuite le menu déroulant **[!UICONTROL Actions de segmentation]** et cliquez sur **[!UICONTROL Approuver]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Créer un extrait {#create-a-snippet}

1. Accédez au **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. Dans la liste déroulante **[!UICONTROL Nouveau]**, cliquez sur **[!UICONTROL Nouveau fragment de code]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Nommez le fragment de code **Message de désabonnement**. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Saisissez votre message de désabonnement par défaut, mettez-le en surbrillance, puis cliquez sur l’icône de lien hypertexte.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Copiez et collez ce jeton : `{{system.unsubscribeLink}}` dans le champ **[!UICONTROL URL]**. Cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Sélectionnez **[!UICONTROL Segmenter par]** dans la section **[!UICONTROL Segmentation]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. Dans le menu déroulant **[!UICONTROL Segmentation]**, saisissez **[!UICONTROL Préféré]** et sélectionnez **[!UICONTROL Langue préférée]**. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Sélectionnez un segment dans l’arborescence. Cliquez sur le texte de désabonnement, puis sur l’icône de lien.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Vérifiez que `{{system.unsubscribeLink}}` se trouve toujours dans le champ **[!UICONTROL URL]**. Modifiez le **[!UICONTROL Texte d’affichage]** pour qu’il corresponde à la langue sélectionnée. Cliquez sur **[!UICONTROL Appliquer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Répétez l’opération pour tous vos segments. Revenez ensuite au **[!UICONTROL Design Studio]**, cliquez sur la liste déroulante **[!UICONTROL Actions liées aux fragments de code]**, puis sur **[!UICONTROL Approuver]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

## Utilisation d’un fragment de code dans un e-mail {#use-a-snippet-in-an-email}

1. Dans l’éditeur d’e-mail, cliquez sur l’élément modifiable. Cliquez ensuite sur l’icône d’engrenage et sélectionnez **[!UICONTROL Remplacer par le fragment de code]**. Si vous sélectionnez un élément de fragment modifiable, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Modifier]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Recherchez et sélectionnez le fragment de code dans la liste déroulante, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Pour tester, cliquez sur **[!UICONTROL Précédent]**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...puis l’onglet **[!UICONTROL Dynamique]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Cliquez sur les différentes langues pour afficher la modification du fragment de code.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >Vous pouvez également modifier le reste de votre e-mail pour la langue dynamique. Utilisez la même technique sur la page de désabonnement.

## Personnalisation de votre page de désabonnement avec du contenu dynamique {#customize-your-unsubscribe-page-with-dynamic-content}

Si vous souhaitez que vos salariés visitent une page de désabonnement dans leur langue préférée, vous pouvez utiliser du contenu dynamique sur la page de destination et la page de confirmation.

1. Accédez au **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Saisissez _Se désabonner_ dans le champ de recherche, puis sélectionnez la page de désabonnement de votre choix.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Sélectionnez **[!UICONTROL Segmenter par]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Recherchez le segment **[!UICONTROL Langue préférée]**. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   >[!NOTE]
   >
   >En savoir plus sur le [contenu dynamique](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md).
