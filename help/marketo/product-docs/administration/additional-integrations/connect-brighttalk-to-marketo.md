---
unique-page-id: 15695874
description: Connectez BrightTALK à Marketo - Marketo Docs - Documentation du produit
title: Connecter BrightTALK à Marketo
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Connectez BrightTALK à Marketo {#connect-brighttalk-to-marketo}

Découvrez comment connecter votre canal BrightTALK à votre instance Marketo. Pour ce faire, vous devez être un administrateur pour les deux.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Étapes de BrightTALK {#steps-in-brighttalk}

1. Connectez-vous à [business.brighttalk.com/demandcentral](http://business.brighttalk.com/demandcentral/login) et cliquez sur **Se connecter maintenant**.
1. Sous Connecteur marketing avancé, cliquez sur **Connexion**.
1. Vous accédez à l’écran d’identification pour demander : ID de client, clé secrète client, URL du service d’identité et URL du service de repos. Pour obtenir ces informations, connectez-vous à Marketo.

## Étapes du marketing {#steps-in-marketo}

>[!NOTE]
>
>A ce stade, vous devrez configurer un rôle d&#39;utilisateur API uniquement et un utilisateur API afin de limiter les autorisations que BrightTALK aura dans votre instance Marketo. Parce que nous avons déjà des articles pour ces étapes, nous allons vous y relier.

1. Créez un [rôle utilisateur API uniquement](http://docs.marketo.com/x/iwMk).
1. [Créez un utilisateur](http://docs.marketo.com/x/jwMk) API, à l’aide du rôle API BrightTALK que vous avez créé lors de l’étape 4.
1. Revenez à la zone Admin.

   ![](assets/one.png)

1. Sous Intégration, cliquez sur **LaunchPoint**.

   ![](assets/two.png)

1. Cliquez sur la liste déroulante **New** et sélectionnez **New Service**.

   ![](assets/three.png)

1. Saisissez le nom d’affichage de votre choix. Cliquez sur la liste déroulante Service et sélectionnez **Personnalisé** (n **pas** sélectionnez BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Pensez à ne pas sélectionner BrightTALK dans la liste déroulante. Il s’agit d’un champ que nous sommes en train de supprimer, et sa sélection pourrait créer des problèmes importants avec votre intégration Marketo/BrightTALK.

1. Saisissez une description de votre choix. Cliquez sur la liste déroulante Utilisateur API uniquement et sélectionnez l’utilisateur API BrightTALK que vous avez créé lors de l’étape 5. Cliquez sur **Créer**.

   ![](assets/five.png)

1. Cliquez sur **Détails de la Vue** pour le service personnalisé que vous venez de créer.

   ![](assets/six.png)

1. Copiez (et enregistrez) les **ID client** et **Secret client**. Cliquez sur **Fermer**.

   ![](assets/eight-1.png)

1. Sous Intégration, sélectionnez **Services Web**.

   ![](assets/nine-1.png)

1. Sous Reest API, copiez (et enregistrez) le **point de terminaison** et **identité**.

   ![](assets/ten.png)

## Étapes de BrightTALK {#steps-in-brighttalk-1}

1. Revenez à l&#39;écran de configuration du connecteur BrightTALK à l&#39;étape 3, puis saisissez les informations d&#39;identification que vous avez enregistrées à partir des étapes 12 et 14.

   Une fois les informations d’identification authentifiées, vous avez officiellement connecté BrightTALK à Marketo. L&#39;étape suivante consiste à déterminer [quels champs de données vous souhaitez synchroniser](http://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync).

