---
unique-page-id: 2360350
description: Créez un service LaunchPoint personnalisé lié à un utilisateur API uniquement pour l’intégration de l’API ReST.
title: Créer un service personnalisé à utiliser avec l’API REST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
TQID: https://experienceleague.adobe.com/7RYZTS-1WiaU0A8ThqHvk01S7GLIIP65xyKI3SIuPyo
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 15%

---

# Créer un service personnalisé à utiliser avec l’API REST {#create-a-custom-service-for-use-with-rest-api}

Si vous souhaitez intégrer à Marketo via l’API ReST, vous devez créer un service personnalisé.

>[!PREREQUISITES]
>
>* [Créer un rôle d’utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Créer un utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md)
>

>[!NOTE]
>
>**Autorisations d’administration requises**

>[!TIP]
>
>Consultez la documentation destinée aux développeurs pour plus d’informations sur l’[API REST](https://developer.adobe.com/marketo-apis/).

## Créer un service personnalisé {#create-custom-service}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Cliquez sur **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Sélectionnez **[!UICONTROL Nouveau]** puis **[!UICONTROL Nouveau service]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Saisissez un **[!UICONTROL Nom d’affichage]** pour le service. Sélectionnez l’**[!UICONTROL Utilisateur API uniquement]** [précédemment créé](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Le service est maintenant créé. Récupérez les informations d’identification à fournir pour l’accès.

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
>Ne partagez pas ces informations, car elles permettent d’accéder à vos données .
