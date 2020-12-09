---
unique-page-id: 3571807
description: Étape 2 sur 3 - Configurer l'utilisateur de synchronisation du marketing dans Dynamics (local 2011) - Documentation du marketing - Documentation du produit
title: Étape 2 sur 3 - Configurer un utilisateur de synchronisation marketing dans Dynamics (local 2011)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---


# Étape 2 sur 3 : Configurer un utilisateur de synchronisation marketing dans Dynamics (local 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Excellent travail de réalisation des étapes précédentes, continuons à passer à travers ceci.

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : Installation de la solution Marketo (2011 sur site)](step-1-of-3-install.md)

>



## Attribuer un rôle utilisateur de synchronisation {#assign-sync-user-role}

Affectez le rôle Utilisateur de synchronisation du marketing uniquement à l’utilisateur de synchronisation du marketing. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Ceci s’applique au module externe Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent avoir le rôle utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Dans le menu inférieur gauche, sélectionnez **Paramètres**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Dans l’arborescence, sélectionnez **Administration**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Sélectionnez **Utilisateurs**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Vous verrez ici une liste d&#39;utilisateurs. Sélectionnez votre utilisateur dédié à Marketo pour synchroniser ou contactez votre administrateur des services de fédération [Principale Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) pour créer un nouvel utilisateur dédié à Marketo. Cliquez sur **Gérer les rôles**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Cochez **Marketo Sync User** et cliquez sur **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l’ [étape 1 sur 3](step-1-of-3-install.md) et importez la solution.

   >[!NOTE]
   >
   >Les mises à jour effectuées dans votre gestion de la relation client par l’utilisateur de synchronisation **ne seront pas** synchronisées à nouveau sur Marketing Cloud.

## Configurer la solution marketing {#configure-marketo-solution}

Presque terminé ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sélectionnez **Paramètres**. Sélectionnez ensuite **Configuration du marketing **dans l’arborescence.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Si la configuration du marketing est manquante, essayez d’actualiser la page. Si le problème persiste, [publiez à nouveau](step-1-of-3-install.md) la solution Marketing Cloud ou déconnectez-vous puis reconnectez-vous.

1. Cliquez sur **Par défaut**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Cliquez sur ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Dans la fenêtre contextuelle, sélectionnez l’utilisateur de synchronisation. Cliquez ensuite sur **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Cliquez sur **Enregistrer** pour enregistrer les modifications.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Cliquez sur **Publier toutes les personnalisations**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

    * Si vous souhaitez limiter le nombre d&#39;enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) maintenant.
    * Exécutez le processus [Valider Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Il vérifie que vos premières configurations ont été effectuées correctement.
    * Connectez-vous à l&#39;utilisateur de synchronisation du marketing dans Microsoft Dynamics CRM.

Super boulot !

>[!NOTE]
>
>**Articles connexes**
>
>[Étape 3 sur 3 : Connecter Microsoft Dynamics au marché (local 2011)](step-3-of-3-connect.md)

