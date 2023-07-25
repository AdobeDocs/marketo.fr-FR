---
unique-page-id: 15695874
description: "Connexion [!DNL BrightTALK] vers Marketo - Documents Marketo - Documentation du produit"
title: "Connexion [!DNL BrightTALK] à Marketo"
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 1%

---

# Connexion [!DNL BrightTALK] vers Marketo {#connect-brighttalk-to-marketo}

Découvrez comment connecter votre [!DNL BrightTALK] vers votre instance Marketo. Pour ce faire, vous devez être un administrateur pour les deux.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Étapes dans [!DNL BrightTALK] {#steps-in-brighttalk}

1. Connectez-vous à [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} et cliquez sur **[!UICONTROL Se connecter maintenant]**.
1. Sous [!UICONTROL Connecteur Marketo avancé], cliquez sur **[!UICONTROL Connexion]**.
1. Vous accédez à l’écran des informations d’identification, ce qui vous demande : ID client, secret client, URL du service d’identité et URL du service REST. Pour obtenir ces informations, connectez-vous à Marketo.

## Étapes dans Marketo {#steps-in-marketo}

>[!NOTE]
>
>À ce stade, vous devrez configurer une [!DNL API Only User Role] et [!DNL API User] afin de restreindre les autorisations [!DNL BrightTALK] aura dans votre instance Marketo. Parce que nous avons déjà des articles pour ces étapes, nous allons vous y relier.

1. Créez un [Rôle d’utilisateur de l’API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [Création d’un utilisateur API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}, à l’aide de la fonction [!DNL BrightTALK] Rôle d’API que vous avez créé à l’étape 4.

1. Revenez au **[!UICONTROL Administration]** zone.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Sous **[!UICONTROL Intégration]**, cliquez sur **[!UICONTROL LaunchPoint]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Cliquez sur le bouton **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouveau service]**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Saisissez un **[!UICONTROL Nom d’affichage]** de votre choix. Cliquez sur le bouton **[!UICONTROL Service]** et sélectionnez **[!UICONTROL Personnalisé]** (do) _not_ select [!DNL BrightTALK]).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >N’oubliez pas de ne pas sélectionner [!DNL BrightTALK] dans la liste déroulante. Il s’agit d’un champ que nous sommes en train de supprimer. Sa sélection peut créer des problèmes importants avec votre [!DNL Marketo/BrightTALK] intégration.

1. Saisissez un [!UICONTROL Description] de votre choix. Cliquez sur le bouton **[!UICONTROL Utilisateur API uniquement]** et sélectionnez l’option [!DNL BrightTALK API User] vous avez créé pendant l’étape 5. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Cliquez sur **[!UICONTROL Afficher les détails]** pour le service personnalisé que vous venez de créer.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Copiez (et enregistrez) la variable **[!UICONTROL ID client]** et **[!UICONTROL Secret du client]**. Cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Sous **[!UICONTROL Intégration]**, sélectionnez **[!UICONTROL Services web]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Sous **[!UICONTROL API REST]**, copiez (et enregistrez) la variable **[!UICONTROL Point d’entrée]** et **[!UICONTROL Identité]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Étapes supplémentaires dans [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. Revenez au [!DNL BrightTALK] écran de configuration du connecteur de l’étape 3, et saisissez les informations d’identification que vous avez enregistrées à partir des étapes 12 et 14.

Une fois les informations d’identification authentifiées, vous êtes officiellement connecté. [!DNL BrightTALK] à Marketo. L’étape suivante consiste à déterminer [les champs de données que vous souhaitez synchroniser ;](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}.
