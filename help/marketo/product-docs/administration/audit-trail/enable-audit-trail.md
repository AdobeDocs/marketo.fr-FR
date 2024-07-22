---
unique-page-id: 11382122
description: Activer le journal d’audit - Documents Marketo - Documentation du produit
title: Activer le journal d’audit
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 1%

---

# Activer le journal d’audit {#enable-audit-trail}

Le journal d’audit est disponible pour tous les clients et est contrôlé par deux autorisations d’administrateur.

>[!NOTE]
>
>Par défaut, les deux autorisations sont activées pour tous les rôles d’administrateur système.

## Activation du journal d’audit pour un rôle {#enable-audit-trail-for-a-role}

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/enable-audit-trail-1.png)

1. Sélectionnez **[!UICONTROL Utilisateurs et rôles]** et cliquez sur **[!UICONTROL Rôles]**.

   ![](assets/enable-audit-trail-2.png)

1. Sélectionnez le rôle pour lequel vous souhaitez activer le journal d’audit, puis cliquez sur **[!UICONTROL Modifier le rôle]**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >Vous avez également la possibilité de créer un nouveau rôle et de lui accorder l’accès Suivi .

1. Développez l’autorisation **[!UICONTROL Accéder à l’administrateur]**. Sélectionnez **[!UICONTROL Accéder au journal d’audit]** et/ou **[!UICONTROL Accéder à l’historique de connexion]**, en fonction de vos besoins. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >**[!UICONTROL Accéder au journal d’audit]** : donne aux utilisateurs l’accès à [!UICONTROL Suivi des ressources] et [!UICONTROL Journal d’audit d’administration].
   >
   >**[!UICONTROL Historique de connexion des accès]** : permet aux utilisateurs d’accéder à l’ [historique de connexion des utilisateurs](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Attribution d’un rôle de journal d’audit à un utilisateur {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Créez](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) ou [activez](#enable-audit-trail) un rôle existant, en lui attribuant des autorisations de suivi.

1. Dans **[!UICONTROL Utilisateurs et rôles]**, cliquez sur **[!UICONTROL Utilisateurs]**.

   ![](assets/enable-audit-trail-5.png)

1. Sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès au journal d’audit et cliquez sur **[!UICONTROL Modifier l’utilisateur]**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Ce processus s’applique également lorsque vous créez un utilisateur.

1. Sélectionnez les rôles Suivi que vous avez créés. Dans cet exemple, nous avons créé &quot;Suivi - Ressource et administrateur&quot; et &quot;Suivi - Avec historique de connexion&quot;.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Si des espaces de travail sont activés, assurez-vous de cocher la case correspondant au rôle, qui sélectionne tous les espaces de travail. La désélection d’un espace de travail individuel masque le journal d’audit. Cela signifie que vous verrez les données du journal d’audit pour chaque espace de travail. Vous avez la possibilité de masquer les espaces de travail lors du [filtrage](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/enable-audit-trail-8.png)
