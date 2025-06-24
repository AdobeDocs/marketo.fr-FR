---
unique-page-id: 7504739
description: Installation de Marketo for Microsoft Dynamics 2015 On-Premise Étape 2 sur 3 - Documents Marketo - Documentation du produit
title: Installez Marketo for Microsoft Dynamics 2015 On-Premise Étape 2 sur 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Étape 2 sur 3 Configurer Marketo pour Dynamics (On-Prem 2015){#step-of-set-up-for-marketo-on-premises-2015}

Excellent travail pour terminer les étapes précédentes. Continuons à avancer dans ce dossier.

>[!PREREQUISITES]
>
>[Installation de Marketo pour Microsoft Dynamics 2015 On-Premise Étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}

## Affecter un rôle d&#39;utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur de synchronisation Marketo uniquement à l’utilisateur de synchronisation Marketo. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Cela s’applique aux versions 4.0.0.14 et ultérieures de Marketo. Pour les versions antérieures, tous les utilisateurs doivent disposer du rôle d’utilisateur de synchronisation . Pour mettre à niveau votre Marketo, voir [Mettre à niveau la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Le paramètre de langue de l’utilisateur de synchronisation [doit être défini sur Anglais](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Sous **[!UICONTROL Paramètres]**, cliquez sur **[!UICONTROL Sécurité]**.

   ![](assets/assign1.png)

1. Cliquez sur **[!UICONTROL Utilisateurs]**.

   ![](assets/assign2.png)

1. Une liste des utilisateurs s’affiche ici. Sélectionnez l’utilisateur Marketo Sync dédié ou contactez votre administrateur [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS) pour créer un utilisateur dédié pour Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Sélectionnez l’utilisateur ou l’utilisatrice de synchronisation. Cliquez sur **[!UICONTROL Gérer les rôles]**.

   ![](assets/assign4.png)

1. Vérifiez Utilisateur de synchronisation Marketo et cliquez sur **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >L’utilisateur de la synchronisation doit disposer de l’autorisation de lecture sur la configuration Marketo.

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l’[étape 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} et importez la solution.

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de la synchronisation ne _pas_ seront resynchronisées avec Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque terminé ! Nous avons juste quelques derniers éléments de configuration avant de passer à l’article suivant.

1. Sous **[!UICONTROL Paramètres]**, cliquez sur **[!UICONTROL Configuration Marketo]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si la configuration de Marketo est manquante, essayez d’actualiser la page. Si le problème persiste, [publiez la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} ou essayez de vous déconnecter puis de vous reconnecter.

1. Cliquez sur **[!UICONTROL Par défaut]**.

   ![](assets/configure2.png)

1. Cliquez sur le champ **[!UICONTROL Utilisateur Marketo]** et sélectionnez l’utilisateur de synchronisation.

   ![](assets/configure3.png)

1. Cliquez sur l’icône d’enregistrement dans le coin inférieur droit.

   ![](assets/configure4.png)

1. Cliquez sur **[!UICONTROL Publier toutes les personnalisations]**.

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >L’utilisateur de la synchronisation doit disposer de l’autorisation de lecture sur la configuration Marketo.

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d’enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} maintenant.
* Exécutez le processus [Valider la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Il vérifie que vos configurations initiales ont été correctement effectuées.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installation de Marketo pour Microsoft Dynamics 2015 On-Premise Étape 3 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md){target="_blank"}
