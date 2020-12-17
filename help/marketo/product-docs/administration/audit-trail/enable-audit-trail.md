---
unique-page-id: 11382122
description: Activer la piste d’audit - Documents marketing - Documentation du produit
title: Activer la piste d'audit
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# Activer la piste d&#39;audit {#enable-audit-trail}

La piste d’audit est disponible pour tous les clients et est contrôlée par deux autorisations d’administrateur.

>[!NOTE]
>
>Par défaut, les deux autorisations sont activées pour tous les rôles d’administration système.

## Activer la piste d&#39;audit pour un rôle {#enable-audit-trail-for-a-role}

1. Cliquez sur **Admin**.

   ![](assets/one-2.png)

1. Sélectionnez **Utilisateurs et rôles** et cliquez sur **Rôles**.

   ![](assets/two-2.png)

1. Sélectionnez le rôle pour lequel vous souhaitez activer la piste d’audit, puis cliquez sur **Modifier le rôle**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Vous avez également la possibilité de créer un nouveau rôle et de lui accorder l’accès Audit Trail.

1. Développez l&#39;autorisation **Access Admin**. Sélectionnez **Chemin d&#39;audit d&#39;accès** et/ou **Historique de connexion d&#39;accès**, en fonction de vos besoins. Cliquez sur **Enregistrer**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >
   >**Chemin d’accès à la piste d’audit :** donne aux utilisateurs l’accès à la piste d’audit des ressources et à la piste d’audit des administrateurs.
   >
   >
   >**Historique de connexion des accès :** donne aux utilisateurs l’accès à l’historique [ de connexion des ](user-login-history.md)utilisateurs.

## Attribuer le rôle de piste d&#39;audit à un utilisateur {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[](http://docs.marketo.com/display/DOCS/Create,+Delete,+Edit+and+Change+a+User+Role#Create,Delete,EditandChangeaUserRole-CreateaRole) Creator  [](#Enable) active un rôle existant, en lui attribuant les autorisations Audit Trail.

1. Dans **Utilisateurs et rôles**, cliquez sur **Utilisateurs**.

   ![](assets/five-1.png)

1. Sélectionnez l’utilisateur auquel vous souhaitez autoriser l’accès à la piste d’audit et cliquez sur **Modifier l’utilisateur**.

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >Ce processus s’applique également lorsque vous créez un utilisateur.

1. Sélectionnez les rôles Audit Trail que vous avez créés. Dans cet exemple, nous avons créé &quot;Audit Trail - Asset and Admin&quot; et &quot;Audit Trail - With Login History&quot;.

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >Si les espaces de travail sont activés, cochez la case du rôle, qui sélectionne tous les espaces de travail. La désélection d’un espace de travail individuel masquera la piste d’audit. Cela signifie que vous verrez les données de piste d’audit pour chaque espace de travail. Vous avez la possibilité de masquer les espaces de travail lorsque [le filtrage](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail) est activé.

1. Cliquez sur **Enregistrer**.

   ![](assets/eight-1.png)

