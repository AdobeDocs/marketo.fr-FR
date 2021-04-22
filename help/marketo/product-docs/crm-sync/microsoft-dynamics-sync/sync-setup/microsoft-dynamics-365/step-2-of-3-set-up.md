---
unique-page-id: 3571827
description: Étape 2 sur 3 - Configurer l'utilisateur Marketo Sync dans Dynamics - Marketo Docs - Documentation du produit
title: Étape 2 sur 3 - Configurer l'utilisateur Marketo Sync dans Dynamics
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Étape 2 sur 3 : Configurer l&#39;utilisateur Marketo Sync dans Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Commençons par créer un compte utilisateur.

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : Installation de la solution Marketo (en ligne)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)

## Créer un utilisateur {#create-a-new-user}

1. Connexion à Dynamics. Cliquez sur l&#39;icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres** et sélectionnez **Sécurité**.

   ![](assets/two.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/three.png)

1. Cliquez sur **Nouveau.**

   ![](assets/four.png)

1. Cliquez sur **Ajouter et License Users** dans la nouvelle fenêtre.

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

1. Saisissez le courrier électronique pour recevoir les nouvelles informations d’identification de l’utilisateur, puis cliquez sur **Envoyer un courrier électronique et fermez**.

   ![](assets/nine.png)

## Affecter le rôle utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur Marketo Sync uniquement à l’utilisateur Marketo Sync. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Ceci s’applique à Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent avoir le rôle utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. Revenez à l’onglet Utilisateurs activés et actualisez la liste des utilisateurs.

   ![](assets/ten.png)

1. Passez la souris sur l’utilisateur Marketo Sync nouvellement créé pour afficher une case à cocher. Cliquez pour le sélectionner.

   ![](assets/eleven.png)

1. Cliquez sur **Gérer les rôles**.

   ![](assets/twelve.png)

1. Cochez **Utilisateur Marketo Sync** et cliquez sur **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Toute mise à jour effectuée dans votre gestion de la relation client par l’utilisateur de synchronisation **ne** sera  synchronisée à Marketo.

## Configurer la solution Marketo {#configure-marketo-solution}

Presque là ! Il ne nous reste plus qu&#39;à informer Marketo Solution sur le nouvel utilisateur créé.

1. Revenez à la section Paramètres avancés et cliquez sur l&#39;icône ![](assets/image2015-5-13-15-3a49-3a19.png) en regard de Paramètres, puis sélectionnez **Marketo Config**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Si **Marketo Config** ne s’affiche pas dans le menu Paramètres, actualisez la page. Si cela ne fonctionne pas, essayez de [publier à nouveau la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) ou de vous déconnecter puis de vous reconnecter.

1. Cliquez sur **Par défaut**.

   ![](assets/fifteen.png)

1. Cliquez sur le bouton de recherche dans le champ **Utilisateur Marketo** et sélectionnez l’utilisateur de synchronisation que vous avez créé.

   ![](assets/sixteen.png)

1. Cliquez sur l&#39;icône ![](assets/image2015-3-13-15-3a10-3a11.png) dans le coin inférieur droit pour enregistrer les modifications.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Cliquez sur le **X** dans l’angle supérieur droit pour fermer l’écran.

   ![](assets/seventeen.png)

1. Cliquez sur l&#39;icône ![](assets/image2015-5-13-15-3a49-3a19-1.png) en regard de Paramètres, puis sélectionnez **Solutions**.

   ![](assets/eighteen.png)

1. Cliquez sur le bouton **Publier toutes les personnalisations**.

   ![](assets/nineteen.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

    * Si vous souhaitez limiter le nombre d&#39;enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) maintenant.
    * Exécutez le processus [Valider Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Il vérifie que vos premières configurations ont été effectuées correctement.
    * Connectez-vous à Marketo Sync User dans Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : Connexion de Microsoft Dynamics à Marketo (en ligne)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
