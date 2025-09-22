---
unique-page-id: 11382122
description: Activer le journal d'audit - Documents Marketo - Documentation du produit
title: Activer le journal d’audit
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 4%

---

# Activer le journal d’audit {#enable-audit-trail}

Le journal d&#39;audit est disponible pour tous les clients et contrôlé par deux autorisations d&#39;administrateur.

>[!NOTE]
>
>Par défaut, les deux autorisations sont activées pour tous les rôles d’administrateur système.

## Activer le journal d&#39;audit pour un rôle {#enable-audit-trail-for-a-role}

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/enable-audit-trail-1.png)

1. Sélectionnez **[!UICONTROL Utilisateurs et rôles]** et cliquez sur **[!UICONTROL Rôles]**.

   ![](assets/enable-audit-trail-2.png)

1. Sélectionnez le rôle pour lequel activer le journal d’audit et cliquez sur **[!UICONTROL Modifier le rôle]**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >Vous avez également la possibilité ici de créer un nouveau rôle et de lui accorder l&#39;accès au journal d&#39;audit.

1. Développez l’autorisation **[!UICONTROL Accéder à l’administrateur]**. Sélectionnez **[!UICONTROL Accéder au journal d’audit]** et/ou **[!UICONTROL Accéder à l’historique de connexion]**, selon vos besoins. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >**[!UICONTROL Journal d’audit d’accès]** : permet aux utilisateurs d’accéder au [!UICONTROL Journal d’audit des ressources] et au [!UICONTROL Journal d’audit d’administration].
   >
   >**[!UICONTROL Accéder à l’historique de connexion]** : permet aux utilisateurs d’accéder à [l’historique de connexion utilisateur](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Affectation d&#39;un rôle de journal d&#39;audit à un utilisateur {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Créer](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) ou [activer](#enable-audit-trail) un rôle existant, en lui donnant les autorisations de journal d’audit.

1. Dans **[!UICONTROL Utilisateurs et rôles]**, cliquez sur **[!UICONTROL Utilisateurs]**.

   ![](assets/enable-audit-trail-5.png)

1. Sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès au journal d’audit et cliquez sur **[!UICONTROL Modifier l’utilisateur]**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Ce processus s’applique également lorsque vous créez un utilisateur.

1. Sélectionnez les rôles de journal d’audit que vous avez créés. Dans cet exemple, nous avons créé « Journal d’audit - Ressource et administrateur » et « Journal d’audit - Avec historique de connexion ».

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Si les espaces de travail sont activés, veillez à cocher la case du rôle qui sélectionne tous les espaces de travail. La désélection d’un espace de travail individuel masque le journal d’audit. Cela signifie que vous verrez les données du journal d’audit pour chaque espace de travail. Vous avez la possibilité de masquer les espaces de travail lors du [filtrage](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/enable-audit-trail-8.png)
