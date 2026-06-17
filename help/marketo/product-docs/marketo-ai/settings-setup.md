---
description: Découvrez comment activer les autorisations de l’IA dédiée à Marketo, configurer les règles d’organisation et gérer les paramètres tels que les intégrations et les notifications.
title: Paramètres et configuration
exl-id: faf642a1-25f0-4566-b35d-074b003835ed
source-git-commit: 3f7d17870cf0d60c716095ae200c003fc8ff0e28
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 3%

---

# Paramètres et configuration {#settings-setup}

Découvrez comment activer des autorisations et utiliser la zone Paramètres pour afficher les détails de connexion, définir des règles d’organisation et configurer des intégrations et des notifications.

>[!AVAILABILITY]
>
>Cette fonctionnalité est en disponibilité limitée. Pour demander l’accès, remplissez [ce formulaire](https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=Wht7-jR7h0OUrtLBeN7O4Y-uSf63sAxCmWyqMJg8eMFUMVZSVExSNDA3T0I4SEcwRDFSVTBGWU01Uy4u&origin=QRCode){target="_blank"}. Assurez-vous que l’identifiant Munchkin de votre abonnement est prêt.

>[!PREREQUISITES]
>
>Pour utiliser cette fonctionnalité, vous devez d’abord accepter les termes [&#x200B; Core Gen-AI et les termes supplémentaires](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Contactez votre gestionnaire de compte pour plus de détails.

## Autorisations et rôles {#permission-and-role}

Il existe une autorisation _Accéder à l’IA Marketo_ et un rôle _Utilisateur de l’IA Marketo_, ce qui permet aux administrateurs et administratrices de mieux contrôler quels utilisateurs et utilisatrices peuvent accéder à la fonctionnalité **IA Marketo**. L’autorisation est affectée au niveau du rôle. Le rôle _Utilisateur Marketo AI_ est fourni avec l’autorisation _Accéder à Marketo AI_ activée par défaut.

>[!IMPORTANT]
>
>L’autorisation _Accéder à l’IA Marketo_ n’est pas activée par défaut pour tous les rôles. Voir le tableau ci-dessous pour plus de détails.

| Rôle | Statut par défaut |
| --- | --- |
| Administration | Activé |
| Administrateur de produits Adobe | Activé |
| Utilisateur marketing | Désactivé |
| Utilisateur standard | Non disponible |
| Utilisateur Marketo AI | Activé |
| Rôles personnalisés | Désactivé |

### Autorisation Accéder à Marketo AI {#access-marketo-ai-permission}

Suivez les étapes ci-dessous pour activer _Accéder à l’IA Marketo_ pour les rôles qualifiés qui ne l’ont pas déjà activé.

1. Dans Mon Marketo, cliquez sur **Admin**, puis **Utilisateurs et rôles**.

   ![](assets/settings-setup-1.png)

1. Dans l’onglet _Rôles_, sélectionnez le rôle souhaité, puis cliquez sur **Modifier le rôle**.

   ![](assets/settings-setup-2.png)

1. Faites défiler vers le bas et cochez la case _Accéder à Marketo AI_, puis cliquez sur **Enregistrer**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >Vous pouvez suivre les mêmes étapes pour supprimer l’autorisation en **décochant** la case _Accéder à l’IA Marketo_.

### Rôle d’utilisateur de l’IA dédiée à Marketo {#marketo-ai-user-role}

Pour affecter un utilisateur spécifique au rôle _Utilisateur de l’IA_, procédez comme suit.

>[!NOTE]
>
>Ce rôle **uniquement** contient l’autorisation _Accéder à l’IA Marketo_.

1. Dans Mon Marketo, cliquez sur **Admin**, puis **Utilisateurs et rôles**.

   ![](assets/settings-setup-4.png)

1. Sélectionnez l’utilisateur souhaité, puis cliquez sur **Modifier l’utilisateur**.

   ![](assets/settings-setup-5.png)

1. Dans _Rôles et espaces de travail_, cochez la case _Utilisateur Marketo AI_. Si vous disposez de plusieurs espaces de travail, vous pouvez spécifier ceux auxquels accéder dans le menu déroulant du signe **+**. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/settings-setup-6.png)

### Rôle personnalisé {#custom-role}

Vous avez également la possibilité de [créer un nouveau rôle](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} et de personnaliser ses autorisations, en ajoutant _Accéder à l’IA Marketo_, ainsi que tout ce que vous souhaitez, et [en attribuant ce rôle](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} à des utilisateurs et utilisatrices spécifiques.

## Paramètres {#settings}

1. Dans Mon Marketo, cliquez sur la mosaïque **Marketo AI**.

   ![](assets/settings-setup-7.png)

1. Cliquez sur l’icône d’engrenage.

   ![](assets/settings-setup-8.png)

### Connexion {#connection}

Cet onglet ne contient pas de champs modifiables. Il affiche des informations sur votre compte, telles que votre Munchkin ID et votre organisation IMS.

![](assets/settings-setup-9.png)

### Règles d&#39;organisation {#organizational-rules}

Définissez les directives et contraintes organisationnelles que l’IA dédiée à Marketo suit lors de la création ou de la modification de ressources Marketo Engage.

![](assets/settings-setup-10.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Les règles utilisent le format Markdown avec le frontMATTER YAML. Les règles globales s’appliquent à tous les espaces de travail. Les règles de Workspace remplacent les paramètres globaux.

### Intégrations (bientôt disponibles) {#integrations}

Configurez les connexions aux services externes et aux API.

_Cet onglet peut apparaître dans l’interface utilisateur, mais il n’est pas encore disponible. Consultez les mises à jour_.

### Notifications (bientôt disponible) {#notifications}

Gérez les préférences des alertes et les canaux de notification.

_Cet onglet peut apparaître dans l’interface utilisateur, mais il n’est pas encore disponible. Consultez cet article pour obtenir des mises à jour_.
