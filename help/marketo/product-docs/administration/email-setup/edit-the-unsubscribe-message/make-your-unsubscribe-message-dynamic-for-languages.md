---
unique-page-id: 6848782
description: Rendre votre message de désabonnement dynamique pour les langues - Documents marketing - Documentation du produit
title: Rendre votre message de désabonnement dynamique pour les langues
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---


# Rendre votre message de désabonnement dynamique pour les langues {#make-your-unsubscribe-message-dynamic-for-languages}

Le message de désabonnement et le lien par défaut sont en anglais. Vous pouvez utiliser du contenu dynamique pour l’afficher dans différentes langues.

>[!NOTE]
>
>Nous avons mis en place ce joli petit tutoriel ci-dessous pour vous. Il s&#39;agit d&#39;une bonne pratique, mais cela peut se faire autrement.

1. Préparation de vos données
1. [Créez un](../../../../product-docs/administration/field-management/create-a-custom-field-in-marketo.md)champ personnalisé nommé &quot;Langue préférée&quot;. (Configurez-le dans votre gestion de la relation client si vous souhaitez que ce champ soit synchronisé).

   >[!TIP]
   >
   >Dans le futur, utilisez ce champ lorsque vous [créez un formulaire](../../../../product-docs/demand-generation/forms/creating-a-form/create-a-form.md) pour capturer les préférences de langue.

1. Créer une segmentation
1. Accédez à la **base de données**.
** ![](assets/db.png)

   **

1. Dans la liste **déroulante Nouveau** , cliquez sur **Nouvelle segmentation**.

   ![](assets/two.png)

1. Nommez la langue **** préférée de la segmentation. Cliquez sur **Ajouter un segment**. Entrez une langue.

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >Le segment par défaut est Anglais.

1. Continuez à ajouter des segments jusqu’à ce que toutes vos langues soient représentées. Cliquez sur **Créer**.

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. Sélectionnez un segment.

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. Accédez à l’onglet **Smart Liste** . Entrez la langue **** préférée dans le champ de recherche. Faites glisser et déposez le filtre sur la trame.

   ![](assets/six.png)

1. Définissez la langue correspondante appropriée.

   ![](assets/seven.png)

1. Répétez cette opération pour toutes vos langues. Sélectionnez ensuite la liste déroulante Actions **de** segmentation, puis cliquez sur **Approuver**.

   ![](assets/image2015-3-9-8-3a39-3a36.png)

1. Création d’un extrait de code
1. Accédez au **Design Studio**.

   ![](assets/ds.png)

1. Dans la liste déroulante **Nouveau** , cliquez sur **Nouveau fragment de code**.

   ** ![](assets/ten.png)

   **

1. Nommez le fragment de code Message **de** désabonnement. Cliquez sur **Créer**.

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. Saisissez votre message de désabonnement par défaut, mettez-le en surbrillance, puis cliquez sur l’icône d’hyperlien.

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. Copiez et collez ce jeton : **`{{system.unsubscribeLink}}`** dans le champ URL **de** lien. Cliquez sur **Insérer**.

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. Sélectionnez **Segmenter par** dans la section Segmentation.

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. Dans la liste déroulante Segmentation, saisissez **Préférée** et sélectionnez Langue **** Préférée. Cliquez sur **Enregistrer**.

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. Sélectionnez un segment dans l’arborescence. Tapez votre message de désabonnement dans cette langue.

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. Copiez et collez le même jeton : **`{{system.unsubscribeLink}}`** dans le champ URL **de** lien. Cliquez sur **Insérer**.

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. Répétez cette opération pour tous vos segments. Revenez ensuite à Design Studio, cliquez sur la liste déroulante Actions **** d’extrait de code, puis cliquez sur **Approuver**.

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   Super. Presque là.

1. Utiliser un extrait de code dans un courrier électronique
1. Dans l’éditeur de courrier électronique, cliquez sur l’élément modifiable. Cliquez ensuite sur l’icône d’engrenage et sélectionnez **Remplacer par un extrait de code**. Si vous sélectionnez un élément de fragment modifiable, cliquez sur l’icône d’engrenage et sélectionnez **Modifier**.

   ![](assets/4.1.png)

1. Recherchez et sélectionnez votre extrait de code dans la liste déroulante, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. Pour le tester, cliquez sur **Précédent**...

   ![](assets/4.3.png)

1. ...puis l’onglet **Dynamique** .

   ![](assets/4.4.png)

1. Cliquez sur les différentes langues pour afficher le changement du fragment de code.

   ![](assets/4.5.png)

   >[!TIP]
   >
   >Bien sûr, vous pouvez également modifier le reste de votre courrier électronique pour une langue dynamique. Pendant que vous y êtes, effectuez la même technique sur la page de désabonnement.

1. Personnalisation de votre page de désabonnement avec du contenu dynamique

   Si vous souhaitez que vos utilisateurs consultent une page de désabonnement dans la langue de leur choix, vous pouvez utiliser du contenu dynamique sur le landing page et la page de confirmation.

   Accédez à Design Studio.

   ![](assets/ds.png)

   Tapez Désabonner dans le champ de recherche. Vous devriez trouver vos pages de désabonnement.

   ![](assets/image2015-3-9-8-3a51-3a53.png)

   Cliquez sur Modifier le brouillon.

   ![](assets/image2015-3-9-8-3a52-3a23.png)

   Sélectionnez Segmenter par.

   ![](assets/image2015-3-9-8-3a52-3a57.png)

   Recherchez le segment Langue préférée. Cliquez sur Enregistrer.

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   Modifiez votre contenu pour chaque landing page, approuvez-le, et c&#39;est une bonne chose d&#39;y aller !

   >[!NOTE]
   >
   >**Plongée profonde**
   >
   >
   >En savoir plus sur le contenu [](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) dynamique et toutes les choses cool que vous pouvez faire.

