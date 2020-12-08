---
unique-page-id: 3571827
description: Étape 2 sur 3 - Configurer l'utilisateur Marketo Sync dans Dynamics - Docs Marketo - Documentation sur les produits
title: Étape 2 sur 3 - Configurer l'utilisateur Marketo Sync dans Dynamics
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Étape 2 sur 3 : Configurer un utilisateur de synchronisation de marketing dans Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Commençons par créer un compte utilisateur.

>[!NOTE]
>
>**Conditions préalables**
>
>[Étape 1 sur 3 : Installation de la solution Marketo (en ligne)](step-1-of-3-install.md)

## Créer un utilisateur {#create-a-new-user}

1. Connexion à Dynamics. Cliquez sur l’icône Paramètres et sélectionnez Paramètres **** avancés.

   ![](assets/one.png)

1. Cliquez sur** Paramètres** et sélectionnez **Sécurité**.

   ![](assets/two.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/three.png)

1. Cliquez sur **Nouveau.**

   ![](assets/four.png)

1. Cliquez sur **Ajouter et Licence Utilisateurs** dans la nouvelle fenêtre.

   ![](assets/five.png)

1. Un nouvel onglet s’ouvre. Cliquez sur **Admin** en haut de la page.

   ![](assets/six.png)

1. Un autre nouvel onglet s&#39;ouvre. Cliquez sur **Ajouter un utilisateur**.

   ![](assets/seven.png)

1. Saisissez toutes vos informations. Lorsque vous avez terminé, cliquez sur **Ajouter**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Ce nom doit être un utilisateur de synchronisation dédié et non un compte d’utilisateur CRM existant. Il n’est pas nécessaire qu’il s’agisse d’une adresse électronique réelle.

1. Saisissez le courrier électronique pour recevoir les informations d’identification du nouvel utilisateur, puis cliquez sur **Envoyer un courrier électronique et fermez**.

   ![](assets/nine.png)

## Attribuer un rôle utilisateur de synchronisation {#assign-sync-user-role}

Affectez le rôle Utilisateur de synchronisation du marketing uniquement à l’utilisateur de synchronisation du marketing. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Ceci s’applique à Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent avoir le rôle utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Revenez à l’onglet Utilisateurs activés et actualisez la liste des utilisateurs.

   ![](assets/ten.png)

1. Passez la souris sur l’utilisateur Marketo Sync nouvellement créé et une case à cocher s’affiche. Cliquez pour le sélectionner.

   ![](assets/eleven.png)

1. Cliquez sur **Gérer les rôles**.

   ![](assets/twelve.png)

1. Cochez **Marketo Sync User** et cliquez sur **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Les mises à jour effectuées dans votre gestion de la relation client par l’utilisateur de synchronisation **ne seront pas** synchronisées à nouveau sur Marketing Cloud.

## Configurer la solution marketing {#configure-marketo-solution}

Presque là ! Il ne nous reste plus qu’à informer Marketing Solution sur le nouvel utilisateur créé.

1. Revenez à la section Paramètres avancés et cliquez sur l’ ![](assets/image2015-5-13-15-3a49-3a19.png)icône en regard de Paramètres, puis sélectionnez **Configuration du marketing**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Si vous ne voyez pas **la configuration** de Marketo dans le menu Paramètres, actualisez la page. Si cela ne fonctionne pas, essayez de [publier à nouveau la solution](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) [](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) Marketo ou de vous déconnecter puis de vous reconnecter.

1. Cliquez sur **Par défaut**.

   ![](assets/fifteen.png)

1. Cliquez sur le bouton de recherche dans le champ Utilisateur **** marketing et sélectionnez l’utilisateur de synchronisation que vous avez créé.

   ![](assets/sixteen.png)

1. Cliquez sur l’ ![](assets/image2015-3-13-15-3a10-3a11.png)icône située dans l’angle inférieur droit pour enregistrer les modifications.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Cliquez sur le **X** dans l’angle supérieur droit pour fermer l’écran.

   ![](assets/seventeen.png)

1. Cliquez sur l’ ![](assets/image2015-5-13-15-3a49-3a19-1.png)icône en regard de Paramètres, puis sélectionnez **Solutions**.

   ![](assets/eighteen.png)

1. Cliquez sur le bouton **Publier toutes les personnalisations** .

   ![](assets/nineteen.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

    * Si vous souhaitez limiter le nombre d&#39;enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) maintenant.
    * Exécutez le processus [Valider Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Il vérifie que vos premières configurations ont été effectuées correctement.
    * Connectez-vous à l&#39;utilisateur de synchronisation du marketing dans Microsoft Dynamics CRM.

>[!NOTE]
>
>**Articles connexes**
>
>
>[Étape 3 sur 3 : Connexion de Microsoft Dynamics avec Marketo (en ligne)](step-3-of-3-connect.md)
