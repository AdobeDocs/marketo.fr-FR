---
unique-page-id: 2950561
description: Script de conversion pour les événements personnalisés - Documents Marketo - Documentation du produit
title: Script de conversion pour les événements personnalisés
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Script de conversion pour les événements personnalisés {#conversion-script-for-custom-events}

Vous définissez l’objectif d’exécution lors de la création d’une offre de parrainage. Si l’action qui compte pour l’objectif est un événement spécifique sur votre propre page web, vous pouvez utiliser un script de conversion pour appeler notre API JavaScript.

## Récupération du script de conversion {#retrieve-the-conversion-script}

1. Dans l’éditeur d’offres de référence, cliquez sur **Détails de l’offre**, puis sélectionnez **Événement JavaScript client** dans la liste déroulante d’objectif d’exécution.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copiez le script supérieur dans la zone grise et placez-le sur votre page web à l’intérieur des balises `<body>`. Le script inférieur est placé dans les balises `<header>`.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >N’oubliez pas de copier et de coller les deux scripts s’ils se trouvent sur un site web autre que Marketo.

## Récupération du script de chargeur {#retrieve-the-loader-script}

1. Sélectionnez l’offre de référence dans l’arborescence, puis cliquez sur **Actions d’offre de référence** et **Code incorporé**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Cliquez avec le bouton droit de la souris sur le **Code d’en-tête** et insérez-le dans l’en-tête de votre page web. Faites ensuite de même pour le **Body Code**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Collage des scripts sur votre page web {#pasting-the-scripts-onto-your-webpage}

Collez les scripts de conversion dans l’HTML pour le corps et l’en-tête. Placez ensuite les scripts de chargeur dans l’HTML pour le corps et l’en-tête.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Connexion au script de conversion {#connecting-the-conversion-script}

C’est là que vous allez écrire une fonction JavaScript qui utilise l’identifiant d’HTML spécifique de l’élément de page sur lequel vous souhaitez déclencher la fin de l’objectif. Par exemple :

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

Dans cet exemple, il y a un bouton sur la page web avec l’identifiant &quot;#myButtonId&quot;. Lorsque l’utilisateur clique sur ce bouton, la personne est enregistrée comme ayant atteint l’objectif.

Super ! Votre site web capture désormais les objectifs personnalisés de promotion sociale avec Marketo.

>[!MORELIKETHIS]
>
>* [Définition de l’objectif pour l’offre de parrainage](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Créer une offre de parrainage](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Déployer Social sur votre site Web](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
