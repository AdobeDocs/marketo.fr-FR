---
unique-page-id: 2359807
description: Personnalisation des styles de tirage - Documents Marketo - Documentation du produit
title: Personnalisation des styles de tirage
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Personnalisation des styles de tirage {#customize-sweepstakes-styles}

Lorsque vous [création d’un tirage](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), vous pouvez personnaliser son aspect sur votre page d’entrée.

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

   Exemple de CSS pour **Bouton Entrée**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Exemple d’image pour **Bouton Entrée**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Si vous utilisez une image avec du texte dessus, pensez à supprimer le texte de la variable **Bouton Entrée** sous Texte ci-dessus.

1. A chaque modification, le résultat s’affiche dans l’aperçu Afficher et modifier .

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Testez votre bouton dans plusieurs navigateurs différents, dont des versions plus anciennes.

   >[!MORELIKETHIS]
   >
   >L’étape suivante consiste à ajouter [e-mails d’inscription et d’exécution à votre tirage](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
