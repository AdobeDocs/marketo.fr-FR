---
unique-page-id: 3571816
description: Étape 2 sur 3 - Configurer l'utilisateur de synchronisation pour Marketo (2013 sur site) - Marketo Docs - Documentation du produit
title: Étape 2 sur 3 - Configurer l'utilisateur de synchronisation pour Marketo (local 2013)
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Étape 2 sur 3 : Configurer l&#39;utilisateur de synchronisation pour Marketo (local 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Excellent travail de réalisation des étapes précédentes, continuons à passer à travers ceci.

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : Installer la solution Marketo dans Dynamics (local 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## Affecter le rôle utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur Marketo Sync uniquement à l’utilisateur Marketo Sync. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Ceci s’applique au module externe Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent avoir le rôle utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. Sous **Paramètres**, cliquez sur **Administration**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Sélectionnez **Utilisateurs**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Vous verrez ici une liste d&#39;utilisateurs. Sélectionnez votre utilisateur Marketo Sync dédié ou contactez votre [administrateur des services de fédération Principale Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [pour créer un utilisateur dédié à Marketo.](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Sélectionnez l’utilisateur de synchronisation. Cliquez sur ![](assets/image2015-3-26-11-3a16-3a22.png) et sélectionnez **Gérer les rôles**.

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Cochez **Utilisateur Marketo Sync** et cliquez sur **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l&#39;[étape 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) et importez la solution.

   >[!NOTE]
   >
   >Toute mise à jour effectuée dans votre gestion de la relation client par l’utilisateur de synchronisation **ne** sera  synchronisée à Marketo.

## Configurer la solution Marketo {#configure-marketo-solution}

Presque terminé ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sous **Paramètres**, cliquez sur **Marketo Config**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Si **Marketo Config** est manquant, essayez d’actualiser la page. Si le problème persiste, [publiez à nouveau la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) ou essayez de vous déconnecter puis de vous reconnecter.

1. Cliquez sur **Par défaut**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Cliquez sur le champ **Utilisateur Marketo** et sélectionnez l’utilisateur de synchronisation.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Cliquez sur ![](assets/image2015-3-13-15-3a10-3a11.png) dans le coin inférieur droit pour enregistrer les modifications.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Cliquez sur **Publier toutes les personnalisations**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d&#39;enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) maintenant.
* Exécutez le processus [Valider Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Il vérifie que vos premières configurations ont été effectuées correctement.
* Connectez-vous à Marketo Sync User dans Microsoft Dynamics CRM.

Bon boulot !

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : Connecter Marketo et Dynamics (locaux 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
