---
unique-page-id: 3571807
description: Étape 2 sur 3 - Configurer l'utilisateur Marketo Sync dans Dynamics (2011 On-Premises) - Marketo Docs - Documentation du produit
title: Étape 2 sur 3 - Configurer l'utilisateur Marketo Sync dans Dynamics (local 2011)
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Étape 2 sur 3 : Configurer un utilisateur Marketo Sync dans Dynamics (local 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Excellent travail de réalisation des étapes précédentes, continuons à passer à travers ceci.

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : Installation de la solution Marketo (local 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

## Affecter le rôle utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur Marketo Sync uniquement à l’utilisateur Marketo Sync. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Ceci s’applique au module externe Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent avoir le rôle utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. Dans le menu inférieur gauche, sélectionnez **Paramètres**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Dans l’arborescence, sélectionnez **Administration**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Sélectionnez **Utilisateurs**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Vous verrez ici une liste d&#39;utilisateurs. Sélectionnez votre utilisateur de synchronisation Marketo dédié ou contactez votre administrateur [Principale Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) pour créer un utilisateur dédié à Marketo. Cliquez sur **Gérer les rôles**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Cochez **Utilisateur Marketo Sync** et cliquez sur **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l&#39;[étape 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) et importez la solution.

   >[!NOTE]
   >
   >Toute mise à jour effectuée dans votre gestion de la relation client par l’utilisateur de synchronisation **ne** sera  synchronisée à Marketo.

## Configurer la solution Marketo {#configure-marketo-solution}

Presque terminé ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sélectionnez **Paramètres**. Sélectionnez ensuite **Marketo Config** dans l’arborescence.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Si Marketo Config est manquant, essayez d’actualiser la page. Si le problème persiste, [publiez à nouveau la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) ou déconnectez-vous et reconnectez-vous.

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

    * Si vous souhaitez limiter le nombre d&#39;enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) maintenant.
    * Exécutez le processus [Valider Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Il vérifie que vos premières configurations ont été effectuées correctement.
    * Connectez-vous à Marketo Sync User dans Microsoft Dynamics CRM.

Bon boulot !

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : Connecter Microsoft Dynamics à Marketo (local 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
