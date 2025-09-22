---
unique-page-id: 7513771
description: Connexion et gestion des utilisateurs - Documents Marketo - Documentation du produit
title: Gestion des connexions et des utilisateurs et utilisatrices
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 2%

---

# Gestion des connexions et des utilisateurs et utilisatrices {#login-and-user-management}

## Créer un rôle d’utilisateur [!UICONTROL Web Personalization] {#create-a-web-personalization-user-role}

1. Accédez à la section **[!UICONTROL Admin]**, puis cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Cliquez sur **[!UICONTROL Rôles]**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Si le rôle d’utilisateur Web Personalization (WP) existe déjà, assurez-vous qu’il est configuré comme indiqué à l’étape 4.

1. Cliquez sur **[!UICONTROL Nouveau rôle]**.

   ![](assets/three-1.png)

1. Saisissez un [!UICONTROL Nom du rôle] et sélectionnez [!UICONTROL Autorisations]. Cliquez sur **[!UICONTROL Créer]** (ce rôle doit [s’appliquer à tous les espaces de travail](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Pour donner aux utilisateurs l’autorisation d’accéder à toutes les fonctionnalités de Ciblage et de Personalization, veillez à cocher _toutes_ les cases.

## [!UICONTROL Web Personalization] et autorisations d’utilisateur de contenu prédictif {#web-personalization-and-predictive-content-user-permissions}

**[!UICONTROL Ciblage et Personalization]** : l’utilisateur ou l’utilisatrice dispose des autorisations d’affichage uniquement si cette autorisation est uniquement sélectionnée.

**[!UICONTROL Admin Web Personalization + Predictive]** : l’utilisateur n’a accès qu’aux paramètres du compte et au paramètre de contenu de l’application Web Personalization et Contenu prédictif. Les utilisateurs peuvent afficher des pages dans l’application, mais ne disposent d’aucune autorisation de création, de modification, de suppression ou de lancement.

**[!UICONTROL Éditeur de contenu prédictif]** : l’utilisateur dispose d’un accès en éditeur à l’application de contenu prédictif. L’autorisation permet de créer, de modifier et de supprimer des éléments de contenu. Il ne permet pas d’activer le contenu pour une utilisation prédictive sur le web ou par e-mail.

**[!UICONTROL Lanceur de contenu prédictif]** : l’utilisateur a accès à toutes les fonctionnalités de contenu prédictif, à l’exception des paramètres de compte et de contenu. L’autorisation permet de créer, modifier et supprimer des éléments de contenu et de les activer.

**[!UICONTROL Éditeur de campagne web]** : l’utilisateur dispose d’un accès en éditeur à toutes les fonctionnalités de Web Personalization pour créer, modifier et supprimer des campagnes web, mais pas pour les lancer.

**[!UICONTROL Lanceur de campagne web]** : l’utilisateur a accès à toutes les fonctionnalités de l’application Web Personalization, à l’exception des paramètres de compte et de contenu. L’autorisation permet de créer, modifier, supprimer et lancer des campagnes web.

## Affecter un rôle WP à un utilisateur {#assign-wp-role-to-user}

1. Accédez à **[!UICONTROL Utilisateurs]**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Sélectionnez l&#39;utilisateur auquel accorder l&#39;accès WP et cliquez sur **[!UICONTROL Modifier utilisateur]**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Sélectionnez le rôle Utilisateur WP pour tous les espaces de travail.

   ![](assets/seven.png)

1. Les utilisateurs nouvellement activés verront la mosaïque **[!UICONTROL Web Personalization]** dans My Marketo la prochaine fois qu’ils se connecteront.

   ![](assets/eight.png)
