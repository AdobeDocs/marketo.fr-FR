---
unique-page-id: 4720257
description: Ajout  [!DNL Facebook]  audiences personnalisées en tant que  [!DNL LaunchPoint]  service - Documents Marketo - Documentation du produit
title: Ajout  [!DNL Facebook] ’audiences personnalisées en tant que  [!DNL LaunchPoint]  service
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Ajout d’audiences personnalisées [!DNL Facebook] as a [!DNL LaunchPoint] Service {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Avec cette intégration, vous pouvez envoyer des données d’audience à partir de listes statiques et intelligentes de Marketo pour les [!DNL Facebook] à utiliser comme audiences personnalisées dans les campagnes publicitaires [!DNL Facebook]. Voici comment le configurer.

1. Accédez à Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Accédez à **[!UICONTROL LaunchPoint]**, cliquez sur **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouveau service]**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Saisissez un **[!UICONTROL Nom d’affichage]** pour votre service et sélectionnez le service **[!UICONTROL Audiences personnalisées Facebook]** dans le menu déroulant **[!UICONTROL Service]**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Ouvrez un nouvel onglet dans le même navigateur et accédez à [facebook.com](https://www.facebook.com/). Connectez-vous à [!DNL Facebook] à l’aide du compte que vous souhaitez utiliser pour l’intégration.

   >[!CAUTION]
   >
   >Pour que Marketo envoie des audiences sur plusieurs comptes Ad Manager, l’utilisateur [!DNL Facebook] autorisé lors des étapes suivantes doit avoir accès à *tous* ces comptes.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Une fois la connexion à [!DNL Facebook] effectuée, revenez à Marketo. Cliquez sur **[!UICONTROL Autoriser]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Vous _devez_ utiliser un compte Business Manager [!DNL Facebook] pour que votre intégration des audiences personnalisées fonctionne. Pour savoir comment configurer un compte Business Manager, reportez-vous à [[!DNL Facebook] Aide](https://www.facebook.com/business/help/1710077379203657).

1. Si vous y êtes invité, cliquez sur **[!UICONTROL OK]** pour accepter l’installation de l’application Marketo dans [!DNL Facebook].

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Vous êtes maintenant autorisé ! Sélectionnez un mode correspondant et cliquez sur **[!UICONTROL Créer]**.

   >[!NOTE]
   >
   >**[!UICONTROL Correspondance de base]** utilise uniquement des adresses e-mail. Le **[!UICONTROL Correspondance avancée]** utilise sept champs supplémentaires, ce qui augmente le taux de correspondance pour davantage de conversions. Cependant, si la politique de confidentialité de votre entreprise n’autorise pas le partage de champs supplémentaires ou si vos données ne les incluent pas, sélectionnez [!UICONTROL Correspondance de base].

   ![](assets/fb-custom-adv-matching-hands.png)

   Très bon travail ! Vous pouvez désormais accéder à n’importe quelle liste statique ou dynamique dans Marketo et envoyer les données d’audience à [!DNL Facebook].

   >[!CAUTION]
   >
   >Oh, avant de partir, assurez-vous d’[accepter les conditions personnalisées des audiences [!DNL Facebook] ](https://www.facebook.com/ads/manage/customaudiences/tos.php) dans votre compte [!DNL Facebook] ! Sans cela, les mises à jour de l’audience échoueront.

>[!MORELIKETHIS]
>
>* [Création d’une audience personnalisée dans  [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configurer [!DNL Facebook] les publicités de lead](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
