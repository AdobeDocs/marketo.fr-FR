---
unique-page-id: 4720257
description: Ajout d’audiences personnalisées Facebook as a LaunchPoint Service - Documents Marketo - Documentation du produit
title: Ajout d’audiences personnalisées Facebook en tant que service LaunchPoint
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Ajout d’audiences personnalisées Facebook en tant que service LaunchPoint {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Avec cette intégration, vous pouvez envoyer des données d’audience à partir de listes statiques et dynamiques Marketo vers Facebook afin de les utiliser comme audiences personnalisées dans les campagnes publicitaires Facebook. Voici comment le mettre en place.

1. Accéder à Marketo **Administration**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Accédez à **LaunchPoint**, cliquez sur **Nouveau** et sélectionnez **Nouveau service**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Saisissez un **Nom d’affichage** pour votre service et sélectionnez l’option **Audiences personnalisées facebook** du service **Service** menu déroulant.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Ouvrez un nouvel onglet dans le même navigateur et accédez à [facebook.com](https://www.facebook.com/). Connectez-vous à Facebook à l’aide du compte que vous souhaitez utiliser pour l’intégration.

   >[!CAUTION]
   >
   >Pour que Marketo puisse envoyer des audiences sur plusieurs comptes Ad Manager, l’utilisateur Facebook que vous autorisez aux étapes suivantes doit avoir accès à *all* de ces comptes.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Une fois connecté à Facebook, revenez à Marketo. Cliquez sur **Autoriser**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >You _must_ utilisez un compte Facebook Business Manager pour que l’intégration des audiences personnalisées fonctionne. Pour découvrir comment configurer un compte Business Manager, reportez-vous à la section [Aide de facebook](https://www.facebook.com/business/help/1710077379203657).

1. Si vous y êtes invité, cliquez sur **OK** pour accepter l’installation de l’application Marketo dans Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Vous êtes maintenant autorisé ! Sélectionnez un mode correspondant et cliquez sur **Créer**.

   >[!NOTE]
   >
   >**Correspondance de base** utilise uniquement des adresses électroniques. **Correspondance avancée** utilise sept champs supplémentaires, ce qui augmente le taux de correspondance, pour plus de conversion. Toutefois, si la politique de confidentialité de votre entreprise n’autorise pas le partage de champs supplémentaires, ou si vos données ne les incluent pas, sélectionnez Correspondance de base.

   ![](assets/fb-custom-adv-matching-hands.png)

   Très bon travail ! Vous pouvez désormais accéder à n’importe quelle liste statique ou dynamique de Marketo et envoyer des données d’audience à Facebook.

   >[!CAUTION]
   >
   >Oh, avant de partir, assurez-vous de [Acceptation de termes d’audiences personnalisés Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) dans votre compte Facebook. Sans cela, les mises à jour de l’audience échoueront.

>[!MORELIKETHIS]
>
>* [Création d’une audience personnalisée dans Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configuration de publicités Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
