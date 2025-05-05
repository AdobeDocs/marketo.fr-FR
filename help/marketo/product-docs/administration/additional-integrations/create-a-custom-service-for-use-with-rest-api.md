---
unique-page-id: 2360350
description: Création d’un service personnalisé à utiliser avec l’API ReST - Documents Marketo - Documentation du produit
title: Création d’un service personnalisé à utiliser avec l’API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Création d’un service personnalisé à utiliser avec l’API ReST {#create-a-custom-service-for-use-with-rest-api}

Si vous souhaitez intégrer Marketo via l’API ReST, vous souhaiterez créer un service personnalisé. Voici comment.

>[!PREREQUISITES]
>
>* [Création d’un rôle d’utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Créer un utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!TIP]
>
>Consultez la documentation destinée aux développeurs pour plus d’informations sur l’ [API REST](https://developer.adobe.com/marketo-apis/). Nous avons également l’ [API SOAP](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/soap/soap-api) si c’est ce dont vous avez besoin.

## Créer un service personnalisé {#create-custom-service}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Cliquez sur **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Sélectionnez **[!UICONTROL New]**, puis **[!UICONTROL New Service]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Saisissez un **[!UICONTROL Nom d’affichage]** pour le service. Sélectionnez l’ **[!UICONTROL utilisateur API uniquement]** [ précédemment créé](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Notez que nous disposons déjà d’une intégration native pour les services de webinaires populaires.

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Oh oui ! Le service est maintenant créé. Allons de l’avant et obtenons toutes les informations d’identification pour l’accès.

## Informations d’identification pour l’accès à l’API {#credentials-for-api-access}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Cliquez sur **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Cliquez sur **[!UICONTROL Afficher les détails]** pour le service [!UICONTROL LaunchPoint] personnalisé créé ci-dessus.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Cliquez sur **[!UICONTROL Obtenir le jeton]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Fournissez l’ **[!UICONTROL ID de client]**, le **[!UICONTROL Secret du client]**, l’ **[!UICONTROL Utilisateur autorisé]** et le **[!UICONTROL Jeton]** au responsable de l’établissement de la connexion.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Ne partagez pas cette information ; c&#39;est la porte dérobée de vos données. Garde-le en sécurité !
