---
unique-page-id: 12983619
description: Ajouter un Slack en tant que service LaunchPoint - Marketo Docs - Documentation sur le produit
title: Ajouter un Slack en tant que service LaunchPoint
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Ajouter un Slack en tant que service LaunchPoint {#add-slack-as-a-launchpoint-service}

L’intégration du Slack comprend deux types de notification :

* **Notifications** système : Recevez des notifications de Slack concernant les événements importants de votre instance de marketing, tels que des alertes concernant les états de la campagne actuelle et tout problème nécessitant une attention immédiate (erreurs de gestion de la relation client et limites de l’API).
* **Moments** intéressants : Lorsqu&#39;une personne connue d&#39;un compte client a déclenché un Insight Marketo, les propriétaires de pistes peuvent être avertis via un Slack. Les notifications incluent des informations de piste ainsi que des détails sur le compte client.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>Si les notifications système Slack ne sont pas activées, contactez le [Support marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Accédez à **LaunchPoint**, puis sous **New** cliquez sur **New Service**.

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. Entrez un nom d&#39;affichage pour votre intégration de Slack. Dans la liste déroulante **Service**, sélectionnez **Slack**. Cliquez sur **Créer**.

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. Cliquez sur **Autoriser**. Le Slack s’ouvre alors dans un nouvel onglet, dans lequel vous allez compléter l’autorisation et accorder l’autorisation Marketo pour extraire les informations du Slack.

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. Dans le nouvel onglet Slack, saisissez l’URL de votre espace de travail et cliquez sur **Continuer**.

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. Entrez vos informations d’identification de Slack et cliquez sur **Se connecter**.

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. Dans la liste déroulante **Publier sur**, sélectionnez le canal dans lequel vous souhaitez que les notifications de Marketo soient publiées. Vérifiez les autorisations demandées, puis cliquez sur **Autoriser**.

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. L’écran de confirmation s’affiche ci-dessous. L&#39;onglet se ferme automatiquement.

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. Actualisez l’onglet Marketo et vérifiez que le Slack est désormais répertorié comme un service principal dans LaunchPoint.

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   Les notifications commenceront maintenant à être publiées sur le canal sélectionné à l’étape 6. Ils ressembleront à quelque chose comme ça :

   ![](assets/samplenotification.png)
