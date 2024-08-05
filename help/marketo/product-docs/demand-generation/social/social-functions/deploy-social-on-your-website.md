---
unique-page-id: 2950524
description: Déploiement de Social sur votre site web - Documents Marketo - Documentation du produit
title: Déploiement de Social sur votre site web
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Déploiement de Social sur votre site web {#deploy-social-on-your-website}

Incorporez les applications sociales à vos pages autres que Marketo.

>[!IMPORTANT]
>
>Le 31 juillet 2024, nous avons commencé à abandonner cette fonctionnalité. Il n’est plus possible de créer de nouvelles ressources. Les ressources existantes continueront à fonctionner jusqu’au 31 janvier 2025. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Tous les utilisateurs de Marketo Engage n’ont pas acheté cette fonctionnalité. Pour plus d’informations, contactez l’équipe du compte d’Adobe (votre gestionnaire de compte).

Vous pouvez déployer des applications sociales sur votre propre site web afin d’impliquer votre audience et de faire participer tout le monde à la conversation générale sur les réseaux sociaux. À mesure que les visiteurs partagent vos promotions et vos contenus avec leurs amis sur les réseaux sociaux, vous générez plus de trafic sur votre site.

1. Sélectionnez une application sociale approuvée, telle qu’une vidéo YouTube ou un bouton Social .

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Sélectionnez **Code incorporé** dans les actions de l’application sociale.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Copiez le code de l’en-tête de page de votre site (`<head>`) et du corps (`<body>`).

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Collez le premier fragment de code dans l’en-tête de page de votre site web.

   ![](assets/socialonsite-embedhead.png)

1. Collez le deuxième fragment de code dans chaque page, où vous souhaitez que votre application sociale apparaisse sur la page.

   ![](assets/socialonsite-embedwidget.png)

1. Si vous devez définir la taille de l’application sociale sur des dimensions spécifiques de votre page, ajoutez les options **outerHeight** et **outerWidth** au deuxième fragment de code. Par exemple, vous pouvez ajouter `options='{"outerHeight":400, "outerWidth":600}'`, comme dans :

   ![](assets/socialonsite-resizewidget2.png)

   Votre application sociale Marketo ajoute désormais du contenu et de l’interactivité à votre site web, invitant les fans, les visiteurs et les clients existants à vous informer. En même temps, il ajoute les données de profil à votre base de données et effectue le suivi des mesures d’influence sociale.

   >[!MORELIKETHIS]
   >
   >* [ Bouton Personnaliser l’application sociale ](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Définition de l’exigence de partage sur les réseaux sociaux](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Pages d’entrée Publish vers Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
