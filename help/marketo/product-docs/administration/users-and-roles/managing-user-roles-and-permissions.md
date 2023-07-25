---
unique-page-id: 2359909
description: Gestion des rôles et autorisations des utilisateurs - Documents Marketo - Documentation du produit
title: Gestion des rôles et des autorisations des utilisateurs
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
feature: Users and Roles
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 4%

---

# Gestion des rôles et des autorisations des utilisateurs {#managing-user-roles-and-permissions}

Définissez, créez et modifiez des rôles utilisateur et affectez-les aux utilisateurs. Vous pouvez ainsi contrôler les zones et fonctionnalités auxquelles chaque utilisateur de Marketo a accès.

Par exemple, un utilisateur marketing a généralement besoin d’un large accès dans l’application pour créer, modifier et déployer des emails, des landing pages et des programmes. En revanche, un concepteur web passe presque tout son temps dans Design Studio, en créant des ressources à utiliser dans les emails et les landing pages. Et bien que les chefs d’entreprise utilisent abondamment les rapports Marketo dans la zone Analytics, ils n’ont peut-être pas besoin de créer ni de piloter eux-mêmes les ressources ou les programmes.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Marketo fournit plusieurs rôles intégrés, avec différents niveaux d’accès :

* **Administration** - toutes les parties de l’application, y compris la section Admin
* **Utilisateur standard** - toutes les parties de l’application, à l’exception de la section Admin
* **Utilisateur marketing** - toutes les parties de l’application, à l’exception de la section Admin
* **Concepteur web** - uniquement Design Studio
* **Utilisateur Analytics** - uniquement la section Analytics ;

Vous ne pouvez pas modifier les rôles d’administrateur et d’utilisateur standard, mais vous pouvez modifier les autres. Vous pouvez également créer de nouveaux rôles personnalisés correspondant aux structures organisationnelles spécifiques de votre entreprise.

## Marketo avec Adobe Identity {#marketo-with-adobe-identity}

Si vous utilisez Marketo avec l’identité de l’Adobe, la liste des descriptions de profil [peut être consulté ici](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md#profile-levels).

## Affectation de rôles à un utilisateur {#assign-roles-to-a-user}

Vous pouvez affecter des rôles à un utilisateur lorsque vous [créer des utilisateurs pour la première fois ;](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) ou [modification d’un utilisateur existant](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/managing-user-roles-and-permissions-1.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/managing-user-roles-and-permissions-2.png)

1. Dans la liste, sélectionnez l’utilisateur que vous souhaitez modifier, puis cliquez sur **[!UICONTROL Modifier l’utilisateur]**.

   ![](assets/managing-user-roles-and-permissions-3.png)

1. Sous **[!UICONTROL Rôles]**, sélectionnez les rôles à affecter à l’utilisateur, en fonction des autorisations dont il a besoin, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/managing-user-roles-and-permissions-4.png)

   >[!NOTE]
   >
   >Pour en savoir plus sur chaque rôle, voir [Descriptions des autorisations de rôle](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md).

## Création d’un rôle {#create-a-new-role}

Parfois, votre entreprise comporte des employés occupant des rôles très spécifiques qui nécessitent une combinaison personnalisée d’autorisations.

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/managing-user-roles-and-permissions-5.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/managing-user-roles-and-permissions-6.png)

1. Cliquez sur le bouton **[!UICONTROL Rôles]** .

   ![](assets/managing-user-roles-and-permissions-7.png)

1. Cliquez sur **[!UICONTROL Nouveau rôle]**.

   ![](assets/managing-user-roles-and-permissions-8.png)

1. Saisissez un **[!UICONTROL Nom du rôle]**, un **[!UICONTROL Description]** (facultatif), puis sélectionnez les autorisations dont les utilisateurs de ce rôle auront besoin.

   ![](assets/managing-user-roles-and-permissions-9.png)

## Modification d’un rôle {#edit-a-role}

Si vous devez modifier les autorisations associées à un rôle existant, vous pouvez modifier ce rôle.

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/managing-user-roles-and-permissions-10.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/managing-user-roles-and-permissions-11.png)

1. Cliquez sur le bouton **[!UICONTROL Rôles]** .

   ![](assets/managing-user-roles-and-permissions-12.png)

1. Dans la liste, sélectionnez le rôle à modifier, puis cliquez sur **[!UICONTROL Modifier le rôle]**.

   ![](assets/managing-user-roles-and-permissions-13.png)

1. Modifiez la variable **[!UICONTROL Nom du rôle]** et **[!UICONTROL Description]** si nécessaire, puis modifiez la sélection de l’objet associé **[!UICONTROL Autorisations]**.

   ![](assets/managing-user-roles-and-permissions-14.png)

   >[!NOTE]
   >
   >Les utilisateurs qui disposent du rôle que vous avez modifié recevront les autorisations modifiées après leur déconnexion puis leur reconnexion.

## Suppression d’un rôle {#delete-a-role}

Si un rôle devient inutile, vous pouvez le supprimer.

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/managing-user-roles-and-permissions-15.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/managing-user-roles-and-permissions-16.png)

1. Cliquez sur le bouton **[!UICONTROL Rôles]** .

   ![](assets/managing-user-roles-and-permissions-17.png)

1. Dans la liste, sélectionnez le rôle à supprimer, puis cliquez sur **[!UICONTROL Supprimer le rôle]**.

   ![](assets/managing-user-roles-and-permissions-18.png)

1. Cliquez sur **[!UICONTROL Supprimer]** pour confirmer.

   ![](assets/managing-user-roles-and-permissions-19.png)
