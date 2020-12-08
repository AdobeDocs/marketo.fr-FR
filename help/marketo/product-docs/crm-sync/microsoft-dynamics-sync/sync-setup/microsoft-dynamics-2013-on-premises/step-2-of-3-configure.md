---
unique-page-id: 3571816
description: Étape 2 sur 3 - Configurer l'utilisateur de synchronisation pour Marketo (2013 sur site) - Documentation sur le marketing - Documentation du produit
title: Étape 2 sur 3 - Configurer l'utilisateur de synchronisation pour Marketo (local 2013)
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---


# Étape 2 sur 3 : Configurer l&#39;utilisateur de synchronisation pour Marketo (local 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Excellent travail de réalisation des étapes précédentes, continuons à passer à travers ceci.

>[!NOTE]
>
>**Conditions préalables**
>
>* [Étape 1 sur 3 : Installer la solution Marketo dans Dynamics (local 2013)](step-1-of-3-install.md)


## Attribuer un rôle utilisateur de synchronisation {#assign-sync-user-role}

Affectez le rôle Utilisateur de synchronisation du marketing uniquement à l’utilisateur de synchronisation du marketing. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Ceci s’applique au module externe Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent avoir le rôle utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Sous **Paramètres**, cliquez sur **Administration**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Sélectionnez **Utilisateurs**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Vous verrez ici une liste d&#39;utilisateurs. Sélectionnez votre utilisateur Marketo Sync dédié ou contactez votre [administrateur des services de fédération](https://msdn.microsoft.com/en-us/library/bb897402.aspx) Principale Directory (AFDS) [pour créer un nouvel utilisateur dédié à Marketo.](http://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Sélectionnez l’utilisateur de synchronisation. Cliquez ![](assets/image2015-3-26-11-3a16-3a22.png)et sélectionnez **Gérer les rôles.**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Cochez **Marketo Sync User** et cliquez sur **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l’ [étape 1 sur 3](step-1-of-3-install.md) et importez la solution.

   >[!NOTE]
   >
   >Les mises à jour effectuées dans votre gestion de la relation client par l’utilisateur de synchronisation **ne seront pas** synchronisées à nouveau sur Marketing Cloud.

## Configurer la solution marketing {#configure-marketo-solution}

Presque terminé ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sous **Paramètres**, cliquez sur **Marketo Config**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Si **la configuration** de Marketo est manquante, essayez d’actualiser la page. Si le problème persiste, [publiez à nouveau la solution](https://docs.marketo.com/pages/viewpage.action?pageId=3571813#Step1of3:InstalltheMarketoSolutioninDynamics(2013On-Premises)-PublishAllCustomizations) Marketo ou essayez de vous déconnecter puis de vous reconnecter.

1. Cliquez sur **Par défaut**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Cliquez sur le champ Utilisateur **** marketing et sélectionnez l’utilisateur de synchronisation.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Cliquez ![](assets/image2015-3-13-15-3a10-3a11.png) dans le coin inférieur droit pour enregistrer les modifications.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Cliquez sur **Publier toutes les personnalisations**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d’enregistrements synchronisés, [configurez maintenant un filtre](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) de synchronisation personnalisé.
* Exécutez le processus [Valider Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) . Il vérifie que vos premières configurations ont été effectuées correctement.
* Connectez-vous à l&#39;utilisateur de synchronisation du marketing dans Microsoft Dynamics CRM.

Super boulot !

>[!NOTE]
>
>**Articles connexes**
>
>* [Étape 3 sur 3 : Connect Marketo and Dynamics (2013 sur site)](step-3-of-3-connect.md)

