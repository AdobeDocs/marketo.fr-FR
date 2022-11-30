---
unique-page-id: 15695874
description: Connexion de BrightTALK à Marketo - Documents Marketo - Documentation du produit
title: Connexion de BrightTALK à Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Connexion de BrightTALK à Marketo {#connect-brighttalk-to-marketo}

Découvrez comment connecter votre canal BrightTALK à votre instance Marketo. Pour ce faire, vous devez être un administrateur pour les deux.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Étapes de BrightTALK {#steps-in-brighttalk}

1. Connectez-vous à [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target=&quot;_blank&quot;} et cliquez sur **Se connecter maintenant**.
1. Sous Connecteur Marketo avancé, cliquez sur **Connexion**.
1. Vous accédez à l’écran des informations d’identification, ce qui vous demande : ID client, secret client, URL du service d’identité et URL du service REST. Pour obtenir ces informations, connectez-vous à Marketo.

## Étapes dans Marketo {#steps-in-marketo}

>[!NOTE]
>
>À ce stade, vous devrez configurer un rôle d’utilisateur API unique et un utilisateur API afin de restreindre les autorisations dont BrightTALK disposera dans votre instance Marketo. Parce que nous avons déjà des articles pour ces étapes, nous allons vous y relier.

1. Créez un [Rôle d’utilisateur de l’API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target=&quot;_blank&quot;}.

1. [Création d’un utilisateur API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target=&quot;_blank&quot;}, à l’aide du rôle API BrightTALK que vous avez créé à l’étape 4.

1. Revenez à la zone Admin .

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Sous Intégration, cliquez sur **LaunchPoint**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Cliquez sur le bouton **Nouveau** et sélectionnez **Nouveau service**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Saisissez le Nom d’affichage de votre choix. Cliquez sur la liste déroulante Service et sélectionnez **Personnalisé** (do) _not_ Sélectionnez BrightTALK).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >N’oubliez pas de ne pas sélectionner BrightTALK dans la liste déroulante. Il s’agit d’un champ que nous sommes en train de supprimer. Sa sélection peut créer des problèmes importants avec votre intégration Marketo/BrightTALK.

1. Saisissez une Description de votre choix. Cliquez sur la liste déroulante Utilisateur API uniquement et sélectionnez l’utilisateur API BrightTALK que vous avez créé à l’étape 5. Cliquez sur **Créer**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Cliquez sur **Afficher les détails** pour le service personnalisé que vous venez de créer.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Copiez (et enregistrez) la variable **ID client** et **Secret du client**. Cliquez sur **Fermer**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Sous Intégration, sélectionnez **Services web**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Sous l’API REST, copiez (et enregistrez) la variable **Point d’entrée** et **Identité**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Étapes supplémentaires dans BrightTALK {#additional-steps-in-brighttalk}

1. Revenez à l’écran de configuration du connecteur BrightTALK à l’étape 3, puis saisissez les informations d’identification que vous avez enregistrées aux étapes 12 et 14.

   Une fois les informations d’identification authentifiées, vous avez officiellement connecté BrightTALK à Marketo. L’étape suivante consiste à déterminer [les champs de données que vous souhaitez synchroniser ;](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target=&quot;_blank&quot;}.
