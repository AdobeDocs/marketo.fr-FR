---
unique-page-id: 2360207
description: Création d’un utilisateur API uniquement - Documents Marketo - Documentation du produit
title: Création d’un utilisateur API uniquement
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Création d’un utilisateur API uniquement {#create-an-api-only-user}

Si vous souhaitez intégrer Marketo via le [API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}, vous devez créer un utilisateur API uniquement. Voici comment.

>[!IMPORTANT]
>
>Si vous créez une API Uniquement pour les utilisateurs dans un abonnement qui a été intégré à Adobe Identity, vos étapes sont différentes et [peut être consulté ici](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}.

>[!PREREQUISITES]
>
>[Création d’un rôle d’utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez au **[!UICONTROL Administration]** zone.

   ![](assets/create-an-api-only-user-1.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/create-an-api-only-user-2.png)

1. Cliquez sur **[!UICONTROL Inviter un nouvel utilisateur]**.

   ![](assets/create-an-api-only-user-3.png)

1. Saisissez un e-mail, un prénom et un nom pour l’utilisateur de l’API uniquement. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Ajoutez un motif facultatif ou une date d’expiration d’accès. Les dates d’expiration d’accès sont pratiques pour les employés de courte durée.

1. Sélectionnez la variable **[!UICONTROL API uniquement]** et vérifiez les **[!UICONTROL API uniquement]** . Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/create-an-api-only-user-5.png)

1. Cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>La fenêtre contextuelle indique, &quot;Une invitation n’est pas requise uniquement pour l’API&quot;, mais cela ne signifie pas que vous avez fait quelque chose de incorrect. Cela signifie simplement que nous allons créer le rôle sans qu’un email d’invitation n’ait à être envoyé.

Bon, alors ! Maintenant, allons de l’avant et créons le service personnalisé.

>[!MORELIKETHIS]
>
>[Créer un service personnalisé à utiliser avec l’API REST](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
