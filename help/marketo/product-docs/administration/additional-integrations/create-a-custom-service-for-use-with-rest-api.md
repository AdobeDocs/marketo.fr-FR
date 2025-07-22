---
unique-page-id: 2360350
description: Création d’un service personnalisé à utiliser avec l’API ReST - Documents Marketo - Documentation du produit
title: Créer un service personnalisé à utiliser avec l’API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Créer un service personnalisé à utiliser avec l’API ReST {#create-a-custom-service-for-use-with-rest-api}

Si vous souhaitez intégrer à Marketo via l’API ReST, vous devez créer un service personnalisé. Voici comment procéder.

>[!PREREQUISITES]
>
>* [Créer un rôle d’utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Créer un utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!TIP]
>
>Consultez notre documentation destinée aux développeurs pour plus d’informations sur l’[API REST](https://developer.adobe.com/marketo-apis/). Nous disposons également de l’API [SOAP](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/soap/soap-api) si c’est ce dont vous avez besoin.

## Créer un service personnalisé {#create-custom-service}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Cliquez sur **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Sélectionnez **[!UICONTROL Nouveau]** puis **[!UICONTROL Nouveau service]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Saisissez un **[!UICONTROL Nom d’affichage]** pour le service. Sélectionnez l’**[!UICONTROL Utilisateur API uniquement]** [précédemment créé](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Notez que nous disposons déjà d’une intégration native pour les services de webinaire populaires.

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Oh oui ! Le service est maintenant créé, allons-y et obtenons toutes les informations d’identification pour fournir l’accès.

## Informations d’identification pour l’accès à l’API {#credentials-for-api-access}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Cliquez sur **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Cliquez sur **[!UICONTROL Afficher les détails]** pour le service personnalisé [!UICONTROL LaunchPoint] créé ci-dessus.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Cliquez sur **[!UICONTROL Obtenir le jeton]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Fournissez les **[!UICONTROL ID client]**, **[!UICONTROL Secret client]**, **[!UICONTROL Utilisateur autorisé]** et **[!UICONTROL Jeton]** à la personne responsable de l’établissement de la connexion.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Ne partagez pas ces informations ; c&#39;est la porte dérobée vers vos données. Gardez-le en sécurité !
