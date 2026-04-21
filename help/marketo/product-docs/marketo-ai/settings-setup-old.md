---
description: Découvrez comment activer les autorisations de l’IA dédiée à Marketo, configurer les règles d’organisation et gérer les paramètres tels que les intégrations et les notifications.
title: Paramètres et configuration
hide: true
hidefromtoc: true
exl-id: d6f37214-65b9-48c1-bf9f-d64b4eda87b9
source-git-commit: c0854d574b4fc995f249783aebcd15ed7d224851
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Paramètres et configuration {#settings-setup}

Découvrez comment activer des autorisations et utiliser la zone Paramètres pour afficher les détails de connexion, définir des règles d’organisation et configurer des intégrations et des notifications.

## Autorisations {#permissions}

>[!IMPORTANT]
>
>Dans la phase Alpha de l’IA Marketo, _l’accès est activé par défaut_ pour les rôles suivants : administrateur, administrateur de produit Adobe, utilisateur marketing, utilisateur standard. Ainsi, au lieu de l’activer pour les rôles auxquels vous souhaitez avoir accès, vous devez le désactiver pour les rôles auxquels vous n’avez pas accès.

### Accès pour tous {#access-for-all}

Si vous souhaitez que l’IA dédiée au Marketo soit activée pour tous les rôles répertoriés ci-dessus, vous n’avez rien à faire.

### Accès pour certains {#access-for-some}

Si vous souhaitez supprimer l’accès pour des rôles, procédez comme suit.

1. Dans Mon Marketo, cliquez sur **Admin**, puis **Utilisateurs et rôles**.

   ![](assets/settings-setup-1.png)

1. Dans l’onglet _Rôles_, sélectionnez le rôle souhaité, puis cliquez sur **Modifier le rôle**.

   ![](assets/settings-setup-2.png)

1. Faites défiler vers le bas et _décochez_ la case **Accéder à la version avec IA**, puis cliquez sur **Enregistrer**.

   ![](assets/settings-setup-3.png)

Répétez ces étapes pour tous les autres rôles souhaités.

### Rôle personnalisé {#custom-role}

Vous avez également la possibilité de [créer un nouveau rôle](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} et de personnaliser ses autorisations, en ajoutant _Accéder à la version avec IA_, ainsi que tout ce que vous souhaitez, et [en attribuant ce rôle](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} à des utilisateurs spécifiques.

<!-- 
## Permissions {#permissions}

In order to access Marketo AI, Admins must first enable role permissions. 

1. In your My Marketo, click **Admin**, then **Users & Roles**.

   ![](assets/settings-setup-1.png)

1. In the _Roles_ tab, select the desired role and click **Edit Role**.

   ![](assets/settings-setup-2.png)

1. Scroll down and select the **Access Build with AI** checkbox and click **Save**.

   ![](assets/settings-setup-3.png)

-->

## Paramètres {#settings}

1. Dans Mon Marketo, cliquez sur la mosaïque **Créer avec l’IA**.

   ![](assets/settings-setup-4.png)

1. Cliquez sur l’icône d’engrenage.

   ![](assets/settings-setup-5.png)

### Connexion {#connection}

Cet onglet ne contient pas de champs modifiables. Il affiche des informations sur votre compte, telles que votre Munchkin ID et votre organisation IMS.

![](assets/settings-setup-6.png)

### Règles d&#39;organisation {#organizational-rules}

Définissez les directives et contraintes organisationnelles que l’IA dédiée à Marketo suit lors de la création ou de la modification de ressources Marketo Engage.

![](assets/settings-setup-7.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Les règles utilisent le format Markdown avec le frontMATTER YAML. Les règles globales s’appliquent à tous les espaces de travail. Les règles de Workspace remplacent les paramètres globaux.

### Intégrations (bientôt disponibles) {#integrations}

Configurez les connexions aux services externes et aux API.

_Cet onglet peut apparaître dans l’interface utilisateur, mais il n’est pas encore disponible. Consultez les mises à jour_.

### Notifications (bientôt disponible) {#notifications}

Gérez les préférences des alertes et les canaux de notification.

_Cet onglet peut apparaître dans l’interface utilisateur, mais il n’est pas encore disponible. Consultez les mises à jour_.
