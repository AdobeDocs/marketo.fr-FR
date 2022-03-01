---
unique-page-id: 2359909
description: Gestion des rôles et autorisations des utilisateurs - Documents Marketo - Documentation du produit
title: Gestion des rôles et des autorisations des utilisateurs
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: a360b46ab1cd7149f609d139590124dcfcda8dad
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Gestion des rôles et des autorisations des utilisateurs {#managing-user-roles-and-permissions}

Définissez, créez et modifiez des rôles utilisateur et affectez-les aux utilisateurs. Vous pouvez ainsi contrôler les zones et fonctionnalités auxquelles chaque utilisateur de Marketo a accès.

Par exemple, un utilisateur marketing a généralement besoin d’un large accès dans l’application pour créer, modifier et déployer des emails, des landing pages et des programmes. En revanche, un concepteur web passe presque tout son temps dans Design Studio, en créant des ressources à utiliser dans les emails et les landing pages. Et bien que les chefs d’entreprise utilisent largement les rapports de Marketo dans la zone Analytics, ils n’ont peut-être pas besoin de créer ni de piloter eux-mêmes les ressources ou les programmes.

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

Si vous utilisez Marketo avec l’identité de l’Adobe, la liste des descriptions de profil [peut être consulté ici](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md#profile-levels).

## Affectation de rôles à un utilisateur {#assign-roles-to-a-user}

Vous pouvez affecter des rôles à un utilisateur lorsque vous [créer des utilisateurs pour la première fois ;](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) ou [modification d’un utilisateur existant](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Pour modifier un utilisateur existant, accédez à **Administration** et cliquez sur **Utilisateurs et rôles**.

   ![](assets/image2014-9-9-18-3a7-3a32.png)

1. Dans la liste, sélectionnez l’utilisateur que vous souhaitez modifier, puis cliquez sur **Modifier l’utilisateur**.

   ![](assets/image2014-9-9-18-3a7-3a42.png)

1. Sous **Rôles**, sélectionnez les rôles à affecter à l’utilisateur, en fonction des autorisations dont il a besoin, puis cliquez sur **Enregistrer**.

   ![](assets/image2014-9-9-18-3a7-3a57.png)

   >[!NOTE]
   >
   >Pour en savoir plus sur chaque rôle, voir  [Descriptions des autorisations de rôle](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md).

## Création d’un rôle {#create-a-new-role}

Parfois, votre entreprise comporte des employés occupant des rôles très spécifiques qui nécessitent une combinaison personnalisée d’autorisations.

1. Pour créer un rôle utilisateur, accédez à Admin et cliquez sur **Utilisateurs et rôles**.

   ![](assets/image2014-9-9-18-3a8-3a12.png)

1. Cliquez sur le bouton **Rôles** .

   ![](assets/image2014-9-9-18-3a8-3a22.png)

1. Cliquez sur **Nouveau rôle**.

   ![](assets/image2014-9-9-18-3a8-3a38.png)

1. Saisissez un **Nom du rôle**, un **Description** (facultatif), puis sélectionnez les autorisations dont les utilisateurs de ce rôle auront besoin.

   ![](assets/image2014-9-9-18-3a9-3a3.png)

## Modification d’un rôle {#edit-a-role}

Si vous devez modifier les autorisations associées à un rôle existant, vous pouvez modifier ce rôle.

1. Accédez à **Administration** et cliquez sur **Utilisateurs et rôles**.

   ![](assets/image2014-9-9-18-3a9-3a15.png)

1. Cliquez sur le bouton **Rôles** .

   ![](assets/image2014-9-9-18-3a9-3a26.png)

1. Dans la liste, sélectionnez le rôle à modifier, puis cliquez sur **Modifier le rôle**.

   ![](assets/image2014-9-9-18-3a9-3a40.png)

1. Modifiez la variable **Nom du rôle** et **Description** si nécessaire, puis modifiez la sélection de l’objet associé **Autorisations**.

   ![](assets/image2014-9-9-18-3a10-3a3.png)

   >[!NOTE]
   >
   >Les utilisateurs qui disposent du rôle que vous avez modifié recevront les autorisations modifiées après leur déconnexion puis leur reconnexion.

## Suppression d’un rôle {#delete-a-role}

Si un rôle devient inutile, vous pouvez le supprimer.

1. Accédez à Admin et cliquez sur **Utilisateurs et rôles**.

   ![](assets/image2014-9-9-18-3a10-3a15.png)

1. Cliquez sur le bouton **Rôles** .

   ![](assets/image2014-9-9-18-3a10-3a27.png)

1. Dans la liste, sélectionnez le rôle à supprimer, puis cliquez sur **Supprimer le rôle**.

   ![](assets/image2014-9-9-18-3a10-3a39.png)

1. Cliquez sur **Supprimer** pour confirmer.

   ![](assets/image2014-9-9-18-3a10-3a50.png)
