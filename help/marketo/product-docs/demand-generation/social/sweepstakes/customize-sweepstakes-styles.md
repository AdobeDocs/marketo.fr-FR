---
unique-page-id: 2359807
description: Personnaliser les styles de tirage - Documents marketing - Documentation du produit
title: Personnaliser les styles de tirage
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Personnaliser les styles de tirage {#customize-sweepstakes-styles}

Lorsque vous [créez un tirage](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), vous pouvez personnaliser son aspect sur votre landing page.

>[!AVAILABILITY]
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus de détails.

1. Accédez à **Activités marketing**.

![](assets/login-marketing-activities-1.png)

1. Sélectionnez le tirage, puis cliquez sur **Modifier le brouillon**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Dans l’éditeur Tirage, accédez à **Paramètres de l’application** > **Apparence**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Modifiez le texte de votre bouton d’inscription et du lien de progression.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Pour chaque élément que vous souhaitez personnaliser, saisissez vos propriétés CSS personnalisées.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Exemple de CSS pour **Bouton Entrer** :
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Exemple d’image pour **Bouton d’entrée** :
   `<pre>background:url(http://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Si vous utilisez une image avec du texte dessus, n’oubliez pas de supprimer le texte du champ **Bouton d’entrée** sous Texte ci-dessus.

1. A chaque modification, le résultat s’affiche dans la prévisualisation Vue et modification.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Testez votre bouton dans plusieurs navigateurs différents, y compris dans les versions plus anciennes.

   >[!MORELIKETHIS]
   >
   >L&#39;étape suivante consiste à ajouter des [courriels d&#39;inscription et d&#39;exécution à vos tirages](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
