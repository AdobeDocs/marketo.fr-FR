---
unique-page-id: 2359906
description: Gestion des utilisateurs de Marketo - Documents Marketo - Documentation du produit
title: Gestion des utilisateurs Marketo
exl-id: 40506d3c-a7cb-45fb-bc10-021bd0c70806
feature: Users and Roles
source-git-commit: ab4358ac1d3e1aa1d3733fa5191c5d59022bdf9f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Gestion des utilisateurs Marketo {#managing-marketo-users}

>[!IMPORTANT]
>
>Cet article est destiné uniquement à ceux qui n’utilisent _pas_ [Marketo avec Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. Si vous le faites, suivez les étapes de [cet article](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}.

## Création d’utilisateurs {#create-users}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/managing-marketo-users-1.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/managing-marketo-users-2.png)

1. Cliquez sur **[!UICONTROL Inviter un nouvel utilisateur]**.

   ![](assets/managing-marketo-users-3.png)

1. Saisissez les **[!UICONTROL Email]**, **[!UICONTROL Prénom]** et **[!UICONTROL Nom]**.

   ![](assets/managing-marketo-users-4.png)

1. Si vous le souhaitez, saisissez un motif pour l’invitation et sélectionnez une date d’expiration dans le champ **[!UICONTROL Access Expires]** à l’aide du sélecteur de date.

   ![](assets/managing-marketo-users-5.png)

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/managing-marketo-users-6.png)

   >[!TIP]
   >
   >Une date d’expiration est idéale pour les parties prenantes externes à court terme ou les consultants qui n’ont besoin de l’accès à Marketo que pour une courte période.

   >[!NOTE]
   >
   >Lorsque la date d’expiration arrive, l’utilisateur reçoit une notification d’expiration et son compte est verrouillé.

1. Sélectionnez le **[!UICONTROL rôle]** de votre choix et cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/managing-marketo-users-7.png)

1. Si nécessaire, modifiez le message d’invitation. Cliquez sur **Send**.

   ![](assets/managing-marketo-users-8.png)

   >[!NOTE]
   >
   >L’e-mail/la connexion doit être unique. Si vous l’avez déjà utilisé dans une instance sandbox, vous devez en utiliser une autre en production et vice versa.

   ![](assets/managing-marketo-users-9.png)

   >[!NOTE]
   >
   >Les invitations expirent trois jours après l’ajout d’un nouvel utilisateur.

Le nouvel utilisateur est maintenant répertorié dans l’onglet Utilisateurs et recevra un e-mail contenant des instructions sur l’activation de son compte.

## Supprimer les utilisateurs {#delete-users}

>[!NOTE]
>
>Si l’utilisateur que vous souhaitez supprimer est également un utilisateur Dynamic Chat, vous devez [le supprimer de Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#remove-a-chat-user){target="_blank"} dans l’Admin Console avant de pouvoir le supprimer dans Marketo Engage.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/managing-marketo-users-10.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/managing-marketo-users-11.png)

1. Sélectionnez l’utilisateur à supprimer, puis cliquez sur **[!UICONTROL Supprimer l’utilisateur]**.

   ![](assets/managing-marketo-users-12.png)

1. Confirmez en cliquant sur **[!UICONTROL OK]**.

   ![](assets/managing-marketo-users-13.png)

## Réinitialisation des mots de passe utilisateur {#reset-user-passwords}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/managing-marketo-users-14.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/managing-marketo-users-15.png)

1. Sélectionnez un utilisateur et cliquez sur **[!UICONTROL Réinitialiser le mot de passe]**.

   ![](assets/managing-marketo-users-16.png)

1. Cliquez sur **[!UICONTROL Fermer]** pour fermer l’invite.

   ![](assets/managing-marketo-users-17.png)

L’utilisateur recevra un courrier électronique contenant des instructions de réinitialisation de mot de passe.

>[!TIP]
>
>Si l&#39;utilisateur ne voit pas l&#39;email dans sa boîte de réception, demandez-lui de vérifier son dossier spam/courrier indésirable.

## Modification des autorisations et modification des informations utilisateur {#change-permissions-and-edit-user-information}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/managing-marketo-users-18.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/managing-marketo-users-19.png)

1. Sélectionnez un utilisateur et cliquez sur **[!UICONTROL Modifier l’utilisateur]**.

   ![](assets/managing-marketo-users-20.png)

1. Vous pouvez modifier les informations utilisateur et modifier le rôle associé. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/managing-marketo-users-21.png)

>[!CAUTION]
>
>Si vous êtes le seul administrateur de Marketo, veillez à ne pas supprimer vos propres droits d’administrateur.

>[!NOTE]
>
>Si un nouvel utilisateur est invité en tant qu’administrateur ou si un administrateur est supprimé, tous les administrateurs actuels reçoivent une notification par courrier électronique.

Super travail ! Vous savez maintenant comment créer un utilisateur, supprimer un utilisateur, réinitialiser le mot de passe d’un utilisateur et modifier des utilisateurs.
