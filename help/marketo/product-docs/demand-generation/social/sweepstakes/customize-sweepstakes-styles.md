---
unique-page-id: 2359807
description: Personnalisation des styles de tirage - Documents Marketo - Documentation du produit
title: Personnalisation des styles de tirage
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# Personnalisation des styles de tirage {#customize-sweepstakes-styles}

Lorsque vous [créez un tirage](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), vous pouvez personnaliser son aspect sur votre page d’entrée.

>[!IMPORTANT]
>
>Le 31 juillet 2024, nous avons commencé à abandonner cette fonctionnalité. Il n’est plus possible de créer de nouvelles ressources. Les ressources existantes continueront à fonctionner jusqu’au 31 janvier 2025. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Tous les utilisateurs de Marketo Engage n’ont pas acheté cette fonctionnalité. Pour plus d’informations, contactez l’équipe du compte d’Adobe (votre gestionnaire de compte).

1. Accédez à **Activités marketing**.

![](assets/login-marketing-activities-1.png)

1. Sélectionnez le tirage, puis cliquez sur **Modifier le brouillon**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Dans l’éditeur Tirage, accédez à **Paramètres de l’application** > **Apparence**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Editez le texte du bouton d&#39;inscription et du lien de progression.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Pour chaque élément que vous souhaitez personnaliser, saisissez vos propriétés CSS personnalisées.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Exemple de CSS pour **Enter Button** :
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Exemple d’image pour **Bouton Entrée** :
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Si vous utilisez une image avec du texte dessus, pensez à supprimer le texte du champ **Bouton d’entrée** sous Texte ci-dessus.

1. A chaque modification, le résultat s’affiche dans l’aperçu Afficher et modifier .

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Testez votre bouton dans plusieurs navigateurs différents, dont des versions plus anciennes.

   >[!MORELIKETHIS]
   >
   >L’étape suivante consiste à ajouter des [emails d’inscription et d’exécution à vos tirages](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
