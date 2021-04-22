---
unique-page-id: 12983619
description: Slack Ajouté en tant que service LaunchPoint - Marketo Docs - Documentation du produit
title: Ajouter un Slack en tant que service LaunchPoint
exl-id: 38c1501d-27ac-4c6c-967d-4decd10e0cb3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Ajouter un Slack en tant que service LaunchPoint {#add-slack-as-a-launchpoint-service}

L’intégration du Slack comprend deux types de notification :

* **Notifications** système : Recevez des notifications de Slack concernant les événements importants de votre instance Marketo, tels que des alertes concernant les états de campagne en cours et tout problème nécessitant une attention immédiate (erreurs de gestion de la relation client et limites de l’API).
* **Moments** intéressants : Lorsqu&#39;un utilisateur connu a déclenché une notification Marketo Insight à partir d&#39;un compte client, les propriétaires de pistes peuvent être avertis par l&#39;intermédiaire d&#39;un Slack. Les notifications incluent des informations de piste ainsi que des détails sur le compte client.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>Si vous n&#39;avez pas encore activé les notifications système Slack, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Accédez à **LaunchPoint**, puis sous **New** cliquez sur **New Service**.

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. Entrez un nom d&#39;affichage pour votre intégration de Slack. Dans la liste déroulante **Service**, sélectionnez **Slack**. Cliquez sur **Créer**.

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. Cliquez sur **Autoriser**. Cela ouvre le Slack dans un nouvel onglet, dans lequel vous allez compléter l&#39;autorisation et accorder à Marketo l&#39;autorisation d&#39;extraire les informations du Slack.

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. Dans le nouvel onglet Slack, saisissez l’URL de votre espace de travail et cliquez sur **Continuer**.

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. Entrez vos informations d’identification de Slack et cliquez sur **Se connecter**.

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. Dans la liste déroulante **Publier sur**, sélectionnez le canal dans lequel les notifications de Marketo doivent être publiées. Vérifiez les autorisations demandées, puis cliquez sur **Autoriser**.

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. L’écran de confirmation s’affiche ci-dessous. L&#39;onglet se ferme automatiquement.

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. Actualisez l’onglet Marketo et vérifiez que le Slack est désormais répertorié comme un service principal dans LaunchPoint.

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   Les notifications commenceront maintenant à être publiées sur le canal sélectionné à l’étape 6. Ils ressembleront à quelque chose comme ça :

   ![](assets/samplenotification.png)
