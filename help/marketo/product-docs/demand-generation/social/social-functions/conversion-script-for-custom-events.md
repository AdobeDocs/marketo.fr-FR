---
unique-page-id: 2950561
description: Script de conversion pour Événements personnalisés - Documentation sur le marketing - Documentation sur les produits
title: Script de conversion pour Événements personnalisés
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Script de conversion pour Événements personnalisés {#conversion-script-for-custom-events}

Vous définissez l’objectif d’exécution lors de la création d’une offre de référence. Si l’action qui compte pour l’objectif est un événement spécifique sur votre propre page Web, vous pouvez utiliser un script de conversion pour appeler notre API JavaScript.

## Récupération du script de conversion {#retrieve-the-conversion-script}

1. Dans l’éditeur d’offres de référence, cliquez sur Détails **de l’** Offre, puis sélectionnez Événement **JavaScript** client dans la liste déroulante des objectifs d’exécution.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copiez le script supérieur dans la zone grise et placez-le sur votre page Web dans les `<body>` balises. Le script inférieur est placé entre les `<header>` balises.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >N’oubliez pas de copier et coller les deux scripts s’ils se trouvent sur un site Web autre que celui du marketing.

## Récupération du script de chargeur {#retrieve-the-loader-script}

1. Sélectionnez l’offre de référence dans l’arborescence, puis cliquez sur Actions **d’Offre de** référence et Code **** incorporé.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Cliquez avec le bouton droit de la souris sur le code **d’** en-tête et insérez-le dans l’en-tête de votre page Web. Faites ensuite la même chose pour le code **** Corps.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Collage des scripts sur votre page Web {#pasting-the-scripts-onto-your-webpage}

Collez les scripts de conversion dans le code HTML pour le corps et l’en-tête. Ensuite, placez les scripts de chargeur dans le code HTML pour le corps et l’en-tête.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Connexion du script de conversion {#connecting-the-conversion-script}

C’est ici que vous allez écrire une fonction JavaScript qui utilise l’identifiant HTML spécifique de l’élément de page sur lequel vous souhaitez déclencher la fin de l’objectif. Par exemple :

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

Dans cet exemple, il y a un bouton sur la page Web avec l’ID &quot;#myButtonId&quot;. Lorsque l&#39;utilisateur clique sur ce bouton, la personne est enregistrée comme ayant atteint l&#39;objectif.

Super ! Votre site Web capture maintenant des objectifs personnalisés de promotion sociale avec Marketo.

>[!MORELIKETHIS]
>
>* [Définition de l’objectif pour l’Offre de renvoi](../../../../product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Créer une Offre de référence](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Déploiement de Social sur votre site Web](deploy-social-on-your-website.md)

