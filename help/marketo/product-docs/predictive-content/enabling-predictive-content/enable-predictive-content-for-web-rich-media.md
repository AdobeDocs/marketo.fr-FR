---
unique-page-id: 7514956
description: Activation du contenu prédictif pour Web Rich Media - Documentation Marketo - Documentation du produit
title: Activation du contenu prédictif pour le contenu multimédia Web enrichi
exl-id: 030f1dd7-8fe7-4c82-be5e-052f0a259e3c
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Activation du contenu prédictif pour le contenu multimédia Web enrichi {#enable-predictive-content-for-web-rich-media}

Le contenu prédictif intéresse vos visiteurs web avec le contenu le plus pertinent, optimisé par l’apprentissage automatique et l’analyse prédictive. Avec Web Rich Media, vous pouvez améliorer votre contenu avec des descriptions textuelles et des images et incorporer plusieurs recommandations de contenu prédictif sur votre site web.

>[!NOTE]
>
>Il est recommandé d’activer plus de cinq éléments de contenu par catégorie et par source (email, média enrichi, barre) avant de tester et d’utiliser du contenu prédictif. Plus de contenu vous donne un meilleur résultat prédictif.

>[!PREREQUISITES]
>
>Avant d’activer le contenu prédictif, vous devez :
>
>* **Préparation de votre contenu prédictif**
   >
   >   * [Modifier le contenu prédictif pour les emails](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target=&quot;_blank&quot;} ou
   >   * [Modification du contenu prédictif pour le contenu multimédia enrichi](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target=&quot;_blank&quot;} ou
   >   * [Modifier le contenu prédictif pour la barre de recommandations](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target=&quot;_blank&quot;}
>
>* [Approbation d’un titre pour le contenu prédictif](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target=&quot;_blank&quot;}


Une fois que vous avez préparé le titre, la description et l’image du contenu pour les médias riches, vous pouvez activer des éléments de contenu individuels ou multiples.

1. Pour activer un titre individuel, cliquez sur un titre pour ouvrir l’éditeur. Cliquez sur Média enrichi, puis cochez la case **Activé pour le contenu prédictif dans les médias riches** puis cliquez sur **Enregistrer**.

   ![](assets/image2017-10-3-9-3a50-3a29.png)

1. Pour plusieurs éléments de contenu, sur la page **Contenu prédictif** , cochez les cases en regard du ou des titres.

   ![](assets/image2017-10-3-10-3a0-3a42.png)

1. Cliquez sur le bouton **Actions de contenu** et sélectionnez **Activation pour Web Rich Media**.

   ![](assets/image2017-10-3-10-3a2-3a6.png)|

## Personnalisation du code JavaScript et incorporation de celui-ci dans votre site web  {#customize-the-javascript-code-and-embed-it-into-your-website}

Reportez-vous à la documentation du modèle de recommandation Média enrichi . [sur le site Marketo Developers](https://developers.marketo.com/documentation/websites/rtp-rich-media-recommendations-api){target=&quot;_blank&quot;}. Cela explique comment personnaliser le modèle de votre site web.

Collez le code JavaScript dans votre site web à l’emplacement où vous souhaitez que le modèle s’affiche.

**Exemples de modèles**

* Template1 : Trois éléments de contenu horizontal avec des images, un en-tête et une description
* Template2 : Trois éléments de contenu vertical avec des images, un en-tête et une description

Voici un exemple du modèle de recommandation pour les médias riches 1 :

![](assets/image2015-6-1-17-3a8-3a33.png)

Voici un exemple du modèle de recommandation Rich Media 2 :

![](assets/image2015-12-20-10-3a35-3a12.png)
