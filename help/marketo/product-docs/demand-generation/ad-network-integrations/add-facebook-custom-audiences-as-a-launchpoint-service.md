---
unique-page-id: 4720257
description: Ajouter des Audiences personnalisées Facebook en tant que service LaunchPoint - Marketo Docs - Documentation du produit
title: Ajouter des Audiences personnalisées Facebook en tant que service LaunchPoint
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---


# Ajouter des Audiences personnalisées Facebook en tant que service LaunchPoint {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Cette intégration vous permet d’envoyer des données d’audience des listes statiques et dynamiques de Marketo à Facebook pour les utiliser comme Audiences personnalisées dans les campagnes publicitaires Facebook. Voici comment le configurer.

1. Accédez à Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Accédez à **LaunchPoint**, cliquez sur **New** et sélectionnez **New Service**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Saisissez un **nom d’affichage** pour votre service et sélectionnez le service **Audiences personnalisées Facebook** dans la liste déroulante **Service**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Ouvrez un nouvel onglet dans le même navigateur et accédez à [facebook.com](https://www.facebook.com/). Connectez-vous à Facebook à l’aide du compte que vous souhaitez utiliser pour l’intégration.

   >[!CAUTION]
   >
   >Pour que Marketing puisse envoyer des audiences sur plusieurs comptes Ad Manager, l’utilisateur Facebook que vous autorisez dans les étapes suivantes doit avoir accès à *tous* de ces comptes.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Une fois connecté à Facebook, revenez à Marketo. Cliquez sur **Autoriser**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Vous _devez_ utiliser un compte Facebook Business Manager pour que l’intégration des Audiences personnalisées fonctionne. Pour savoir comment configurer un compte Business Manager, consultez l&#39;[Aide de Facebook](https://www.facebook.com/business/help/1710077379203657).

1. Si vous y êtes invité, cliquez sur **OK** pour accepter l’installation de l’application Marketo dans Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Vous êtes maintenant autorisé ! Sélectionnez un mode correspondant et cliquez sur **Créer**.

   >[!NOTE]
   >
   >**Les** correspondances de base utilisent uniquement les adresses électroniques. **Les** correspondances avancées utilisent sept champs supplémentaires, ce qui augmente le taux de correspondance, pour davantage de conversions. Cependant, si la politique de confidentialité de votre société n’autorise pas le partage de champs supplémentaires ou si vos données ne les incluent pas, sélectionnez Correspondance de base.

   ![](assets/fb-custom-adv-matching-hands.png)

   Super boulot ! Vous pouvez désormais accéder à n’importe quelle liste statique ou intelligente de Marketo et envoyer les données d’audience à Facebook.

   >[!CAUTION]
   >
   >Oh, avant de partir, veillez à [Accepter les termes d&#39;Audiences personnalisées de Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) dans votre compte Facebook ! Sans cela, les mises à jour des audiences échoueront.

>[!MORELIKETHIS]
>
>* [Création d’une Audience personnalisée dans Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
   >
   >
* [Configurer des annonces de pistes Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

