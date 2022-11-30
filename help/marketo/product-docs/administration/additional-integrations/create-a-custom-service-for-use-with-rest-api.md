---
unique-page-id: 2360350
description: Création d’un service personnalisé à utiliser avec l’API ReST - Documents Marketo - Documentation du produit
title: Création d’un service personnalisé à utiliser avec l’API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 5%

---

# Création d’un service personnalisé à utiliser avec l’API ReST {#create-a-custom-service-for-use-with-rest-api}

Si vous souhaitez intégrer Marketo via l’API ReST, vous souhaiterez créer un service personnalisé. Voici comment.

>[!PREREQUISITES]
>
>* [Création d’un rôle d’utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Création d’un utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>


>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!TIP]
>
>Consultez la documentation destinée aux développeurs pour plus d’informations sur [API ReST](https://developers.marketo.com/documentation/rest/). Nous avons également le [API SOAP](https://developers.marketo.com/documentation/soap/) si c&#39;est ce dont vous avez besoin.

## Créer un service personnalisé {#create-custom-service}

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Cliquez sur **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Sélectionner **Nouveau** puis **Nouveau service**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Saisissez un **Nom d’affichage** pour le service. Sélectionnez la **Utilisateur API uniquement** [précédemment créé](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Notez que nous disposons déjà d’une intégration native pour les services de webinaires populaires.

1. Cliquez sur **Créer**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Oh oui ! Le service est maintenant créé. Allons de l’avant et obtenons toutes les informations d’identification pour l’accès.

## Informations d’identification pour l’accès aux API {#credentials-for-api-access}

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Cliquez sur **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Cliquez sur **Afficher les détails** pour le service LaunchPoint personnalisé créé ci-dessus.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Cliquez sur **Obtenir un jeton**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Fournissez les **ID client**, **Secret du client**, **Utilisateur autorisé**, et **Jeton** au responsable de l&#39;établissement de la connexion.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Ne partagez pas cette information ; c&#39;est la porte dérobée de vos données. Garde-le en sécurité !
