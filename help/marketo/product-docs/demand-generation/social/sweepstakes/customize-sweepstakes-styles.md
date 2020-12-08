---
unique-page-id: 2359807
description: Personnaliser les styles de tirage - Documents marketing - Documentation du produit
title: Personnaliser les styles de tirage
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Personnaliser les styles de tirage {#customize-sweepstakes-styles}

Lorsque vous [créez un tirage](create-sweepstakes.md), vous pouvez personnaliser son aspect sur votre landing page.

>[!NOTE]
>
>**Disponibilité**
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus de détails.

1. Accédez à Activités marketing.

![](assets/login-marketing-activities-1.png)

1. Sélectionnez le tirage, puis cliquez sur **Modifier** le **brouillon**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Dans l’éditeur Tirage, accédez à **App** **Settings** **>** **Appearance.**

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Modifiez le texte de votre bouton d’inscription et du lien de progression.
1. ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Pour chaque élément que vous souhaitez personnaliser, saisissez vos propriétés CSS personnalisées.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Exemple de CSS pour le bouton ****Entrée :
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>` Exemple d’image pour le bouton ****Entrée :
   `<pre>background:url(http://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Si vous utilisez une image avec du texte dessus, n&#39;oubliez pas de supprimer le texte du champ **Saisir** **Bouton **sous Texte ci-dessus.

1. A chaque modification, le résultat s’affiche dans la prévisualisation Vue et modification.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >Testez votre bouton dans plusieurs navigateurs différents, y compris dans les versions plus anciennes.

   >[!NOTE]
   >
   >**Articles connexes**
   >
   >
   >L’étape suivante consiste à ajouter des courriers électroniques d’ [inscription et d’exécution à vos tirages](../../../../product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).

