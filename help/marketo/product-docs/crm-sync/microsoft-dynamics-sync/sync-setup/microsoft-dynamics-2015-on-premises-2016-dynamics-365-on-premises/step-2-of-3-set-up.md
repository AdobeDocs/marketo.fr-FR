---
unique-page-id: 7504739
description: Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 2 sur 3 - Marketo Docs - Documentation du produit
title: Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 2 sur 3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---


# Étape 2 sur 3 Configuration du marché pour Dynamics (On-Prem 2015 et On-Prem 2016 365){#step-of-set-up-for-marketo-on-premises-and-365}

Excellent travail à la réalisation des étapes précédentes. Continuons à passer à travers ça.

>[!PREREQUISITES]
>
>[Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Affecter le rôle utilisateur de synchronisation {#assign-sync-user-role}

Affectez le rôle Utilisateur de synchronisation du marketing uniquement à l’utilisateur de synchronisation du marketing. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Ceci s’applique à Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent avoir le rôle utilisateur de synchronisation. Pour mettre à niveau votre Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Sous **Paramètres**, cliquez sur **Sécurité**.

   ![](assets/assign1.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/assign2.png)

1. Vous verrez ici une liste d&#39;utilisateurs. Sélectionnez l&#39;utilisateur Marketo Sync dédié ou contactez votre administrateur [Principale Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) pour créer un utilisateur dédié pour Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Sélectionnez l’utilisateur de synchronisation. Cliquez sur **Gérer les rôles**.

   ![](assets/assign4.png)

   Cochez la case Marketo Sync User (Synchroniser l’utilisateur) et cliquez sur OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l&#39;[étape 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) et importez la solution.

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre gestion de la relation client par l’utilisateur de synchronisation **ne** seront  synchronisées de nouveau sur Marketo.

## Configurer la solution marketing {#configure-marketo-solution}

Presque terminé ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sous **Paramètres**, cliquez sur **Marketo Config**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si la configuration du marketing est manquante, essayez d’actualiser la page. Si le problème persiste, [publiez la solution marketing](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) ou essayez de vous déconnecter puis de vous reconnecter.

1. Cliquez sur **Par défaut**.

   ![](assets/configure2.png)

1. Cliquez sur le champ **Utilisateur du marketing** et sélectionnez l’utilisateur de synchronisation.

   ![](assets/configure3.png)

1. Cliquez sur l’icône Enregistrer dans le coin inférieur droit.

   ![](assets/configure4.png)

1. Cliquez sur **Publier toutes les personnalisations**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d&#39;enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) maintenant.
* Exécutez le processus [Valider Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Il vérifie que vos premières configurations ont été effectuées correctement.
* Connectez-vous à l&#39;utilisateur de synchronisation du marketing dans Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 3 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
