---
unique-page-id: 2360207
description: Créer un utilisateur API uniquement - Documents Marketo - Documentation du produit
title: Créer un utilisateur API uniquement
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 3%

---

# Créer un utilisateur API uniquement {#create-an-api-only-user}

Si vous souhaitez intégrer à Marketo via l’[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}, vous ne devez créer qu’un utilisateur de l’API. Voici comment procéder.

>[!IMPORTANT]
>
>Si vous créez une API destinée uniquement aux utilisateurs d’un abonnement qui a été intégré à Adobe Identity, vos étapes sont différentes et [vous pouvez les trouver ici](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}.

>[!PREREQUISITES]
>
>[Créer un rôle d’utilisateur API uniquement](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-an-api-only-user-1.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/create-an-api-only-user-2.png)

1. Cliquez sur **[!UICONTROL Inviter un nouvel utilisateur]**.

   ![](assets/create-an-api-only-user-3.png)

1. Saisissez un e-mail, un prénom et un nom pour l’utilisateur ou l’utilisatrice de l’API uniquement. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Ajoutez une date facultative [!UICONTROL Motif] ou [!UICONTROL Expiration de l’accès]. Les dates d&#39;expiration de l&#39;accès sont pratiques pour les employés temporaires.

1. Sélectionnez le rôle **[!UICONTROL API uniquement]** et cochez la case **[!UICONTROL API uniquement]**. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/create-an-api-only-user-5.png)

1. Cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>Le pop-up indique « Aucune invitation n’est requise pour l’API uniquement », mais cela ne signifie pas que vous avez fait quelque chose de mal. Cela signifie simplement que nous allons créer le rôle sans qu’un e-mail d’invitation doive être envoyé.

Très bien, alors ! Créons maintenant le service personnalisé.

>[!MORELIKETHIS]
>
>[Créer un service personnalisé à utiliser avec l’API REST](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
