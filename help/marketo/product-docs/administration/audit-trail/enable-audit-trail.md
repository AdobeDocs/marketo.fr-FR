---
unique-page-id: 11382122
description: Activer le journal d’audit - Documents Marketo - Documentation du produit
title: Activer le journal d’audit
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
source-git-commit: 73d41904ca74ae265648c3ed91805be7c4d24fe0
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Activer le journal d’audit {#enable-audit-trail}

Le journal d’audit est disponible pour tous les clients et est contrôlé par deux autorisations d’administrateur.

>[!NOTE]
>
>Par défaut, les deux autorisations sont activées pour tous les rôles d’administrateur système.

## Activation du journal d’audit pour un rôle {#enable-audit-trail-for-a-role}

1. Cliquez sur **Administration**.

   ![](assets/enable-audit-trail-1.png)

1. Sélectionner **Utilisateurs et rôles** et cliquez sur **Rôles**.

   ![](assets/enable-audit-trail-2.png)

1. Sélectionnez le rôle pour lequel vous souhaitez activer le journal d’audit, puis cliquez sur **Modifier le rôle**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >Vous avez également la possibilité de créer un nouveau rôle et de lui accorder l’accès Suivi .

1. Développez l’objet **Accès à l’administrateur** autorisation. Sélectionner **Journal d’audit d’accès** et/ou **Historique de connexion des accès**, selon vos besoins. Cliquez sur **Enregistrer**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >**Accédez au journal d’audit :** Permet aux utilisateurs d’accéder au journal d’audit des ressources et au journal d’audit de l’administrateur.
   >
   >**Accéder à l’historique de connexion :** Donne aux utilisateurs l’accès à [Historique de connexion des utilisateurs](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Attribution d’un rôle de journal d’audit à un utilisateur {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Créer](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) ou [enable](#enable-audit-trail) un rôle existant, lui attribuant des autorisations Suivi .

1. Dans **Utilisateurs et rôles**, cliquez sur **Utilisateurs**.

   ![](assets/enable-audit-trail-5.png)

1. Sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès au journal d’audit, puis cliquez sur **Modifier l’utilisateur**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Ce processus s’applique également lorsque vous créez un utilisateur.

1. Sélectionnez les rôles Suivi que vous avez créés. Dans cet exemple, nous avons créé &quot;Suivi - Ressource et administrateur&quot; et &quot;Suivi - Avec historique de connexion&quot;.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Si des espaces de travail sont activés, assurez-vous de cocher la case correspondant au rôle, qui sélectionne tous les espaces de travail. La désélection d’un espace de travail individuel masque le journal d’audit. Cela signifie que vous verrez les données du journal d’audit pour chaque espace de travail. Vous avez la possibilité de masquer les espaces de travail lorsque [filtrage](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Cliquez sur **Enregistrer**.

   ![](assets/enable-audit-trail-8.png)
