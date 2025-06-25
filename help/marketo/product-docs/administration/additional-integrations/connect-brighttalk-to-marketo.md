---
unique-page-id: 15695874
description: Connexion  [!DNL BrightTALK]  Marketo - Documents Marketo - Documentation du produit
title: Connexion [!DNL BrightTALK] à Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: b95458ffab422901ef5e674756ae5e413ec542fd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Connexion de [!DNL BrightTALK] à Marketo {#connect-brighttalk-to-marketo}

Découvrez comment connecter votre canal [!DNL BrightTALK] à votre instance Marketo. Pour ce faire, vous devez être un administrateur pour les deux.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Étapes dans [!DNL BrightTALK] {#steps-in-brighttalk}

1. Connectez-vous à [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} puis cliquez sur **[!UICONTROL Se connecter maintenant]**.
1. Sous [!UICONTROL  Connecteur Marketo avancé ], cliquez sur **[!UICONTROL Se connecter]**.
1. Vous accédez à l’écran des informations d’identification en demandant : ID client, secret client, URL du service d’identités et URL du service REST. Pour obtenir ces informations, connectez-vous à Marketo.

## Étapes dans Marketo {#steps-in-marketo}

>[!NOTE]
>
>À ce stade, vous devrez configurer un [!DNL API Only User Role] et un [!DNL API User] afin de limiter les autorisations dont [!DNL BrightTALK] disposerez dans votre instance Marketo. Puisque nous avons déjà des articles pour ces étapes, nous vous connecterons à celles-ci.

1. Créez un [Rôle utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [Créez un utilisateur d’API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"} en utilisant le rôle d’API [!DNL BrightTALK] que vous avez créé à l’étape 4.

1. Revenez à la zone **[!UICONTROL Admin]**.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Sous **[!UICONTROL Intégration]**, cliquez sur **[!UICONTROL LaunchPoint]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouveau service]**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Saisissez un **[!UICONTROL Nom d’affichage]** de votre choix. Cliquez sur le menu déroulant **[!UICONTROL Service]** et sélectionnez **[!UICONTROL Personnalisé]** (ne _pas_ sélectionnez [!DNL BrightTALK]).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >N’oubliez pas de ne pas sélectionner [!DNL BrightTALK] dans la liste déroulante. Il s’agit d’un champ que nous sommes en train de supprimer. Le sélectionner pourrait créer des problèmes importants avec votre intégration [!DNL Marketo/BrightTALK].

1. Saisissez la [!UICONTROL Description] de votre choix. Cliquez sur le menu déroulant **[!UICONTROL Utilisateur API uniquement]** et sélectionnez le [!DNL BrightTALK API User] que vous avez créé à l’étape 5. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Cliquez sur **[!UICONTROL Afficher les détails]** pour le service personnalisé que vous venez de créer.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Copiez (et enregistrez) les **[!UICONTROL ID client]** et **[!UICONTROL Secret client]**. Cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Sous **[!UICONTROL Intégration]**, sélectionnez **[!UICONTROL Services Web]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Sous **[!UICONTROL API Rest]**, copiez (et enregistrez) les **[!UICONTROL Point d’entrée]** et **[!UICONTROL Identité]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Étapes supplémentaires dans [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. Revenez à l’écran de configuration du connecteur [!DNL BrightTALK] à partir de l’étape 3 et saisissez les informations d’identification que vous avez enregistrées à partir des étapes 12 et 14.

Une fois les informations d’identification authentifiées, vous avez officiellement connecté [!DNL BrightTALK] à Marketo. L’étape suivante consiste à déterminer les champs de données à synchroniser. Si vous avez besoin d’aide, contactez l’assistance à l’adresse [BrightTALK](https://www.brighttalk.com/){target="_blank"}.
