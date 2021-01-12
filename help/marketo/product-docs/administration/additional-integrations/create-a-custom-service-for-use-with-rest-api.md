---
unique-page-id: 2360350
description: Création d’un service personnalisé à utiliser avec l’API ReST - Documentation marketing - Documentation du produit
title: Création d’un service personnalisé à utiliser avec l’API ReST
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---


# Créer un service personnalisé à utiliser avec l&#39;API ReST {#create-a-custom-service-for-use-with-rest-api}

Si vous souhaitez effectuer une intégration avec Marketo via l&#39;API ReST, vous souhaiterez créer un service personnalisé. Voici comment.

>[!PREREQUISITES]
>
>* [Création d’un rôle utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Créer un utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!TIP]
>
>Consultez la documentation destinée aux développeurs pour en savoir plus sur l&#39;[API ReST](http://developers.marketo.com/documentation/rest/). Nous avons également l&#39;[API SOAP](http://developers.marketo.com/documentation/soap/) si c&#39;est ce dont vous avez besoin.

>[!NOTE]
>
>Vous ne pouvez pas créer de service personnalisé si vous disposez du niveau Spark de Marketo.

## Créer un service personnalisé {#create-custom-service}

1. Accédez à **Admin** et cliquez sur **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. Sous **New**, cliquez sur **New Service**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Saisissez un **nom d’affichage** pour le service. Sélectionnez **API Uniquement utilisateur** [précédemment créé](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   >[!NOTE]
   >
   >Notez que nous disposons déjà d’une intégration native pour les services de webinaires populaires.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Cliquez sur **Créer**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   Oh oui ! Le service est maintenant créé, allons de l&#39;avant et obtenons toutes les informations d&#39;identification pour fournir l&#39;accès.

## Informations d&#39;identification pour l&#39;accès à l&#39;API {#credentials-for-api-access}

1. Accédez à **Admin** et cliquez sur **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Cliquez sur **Détails de la Vue** pour le service LaunchPoint personnalisé créé ci-dessus.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Cliquez sur **Obtenir le jeton**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Fournissez le **ID client**, **Secret client**, **Utilisateur autorisé** et **Jeton** à la personne chargée d&#39;établir la connexion.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>Ne partagez pas ces informations ; c&#39;est la porte de derrière de vos données. Gardez-le en sécurité !
