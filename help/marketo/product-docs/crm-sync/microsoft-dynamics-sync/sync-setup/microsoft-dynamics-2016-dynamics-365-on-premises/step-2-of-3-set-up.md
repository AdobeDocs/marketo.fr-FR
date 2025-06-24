---
description: Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 2 sur 3 - Documents Marketo - Documentation du produit
title: Installez Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 2 sur 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Étape 2 sur 3 Configurer Marketo pour Dynamics (2016 On-Prem/Dynamics 365 On-Premise){#step-of-set-up-for-marketo-on-premises-2016}

Excellent travail pour terminer les étapes précédentes. Continuons à avancer dans ce dossier.

>[!PREREQUISITES]
>
>[Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}

## Créer un nouvel utilisateur {#create-a-new-user}

1. Connectez-vous à Dynamics. Cliquez sur l’icône Paramètres et sélectionnez Paramètres avancés .

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Cliquez sur **[!UICONTROL Paramètres]** et sélectionnez **[!UICONTROL Sécurité]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Cliquez sur **[!UICONTROL Utilisateurs]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Cliquez sur **[!UICONTROL Nouveau]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Cliquez sur **[!UICONTROL Ajouter des utilisateurs et obtenir une licence]**. Un nouvel onglet doit s’ouvrir.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Cliquez sur **[!UICONTROL Admin]** en haut de la page. Un autre nouvel onglet doit s’ouvrir.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Cliquez sur **[!UICONTROL Ajouter un utilisateur]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Saisissez toutes vos informations. Lorsque vous avez terminé, cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Ce nom doit être un utilisateur de synchronisation dédié et non un compte d’utilisateur CRM existant. Il ne doit pas nécessairement s’agir d’une adresse e-mail réelle.

1. Saisissez l’adresse e-mail pour recevoir les nouvelles informations d’identification de l’utilisateur et cliquez sur Envoyer un e-mail et fermer.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Créer une application cliente {#create-a-new-client-application}

Suivez les étapes décrites dans [cet article de Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later){target="_blank"} pour créer une application cliente et accorder des autorisations. Notez l’ID client/le secret de l’application cliente Dynamics.

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

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l’[étape 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) et importez la solution.

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de la synchronisation ne _pas_ seront resynchronisées avec Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque terminé ! Nous avons juste quelques derniers éléments de configuration avant de passer à l’article suivant.

1. Sous **[!UICONTROL Paramètres]**, cliquez sur **[!UICONTROL Configuration Marketo]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si la configuration de Marketo est manquante, essayez d’actualiser la page. Si le problème persiste, [publiez la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"} ou essayez de vous déconnecter puis de vous reconnecter.

1. Cliquez sur **[!UICONTROL Par défaut]**.

   ![](assets/configure2.png)

1. Cliquez sur le champ **[!UICONTROL Utilisateur Marketo]** et sélectionnez l’utilisateur de synchronisation.

   ![](assets/configure3.png)

1. Cliquez sur l’icône d’enregistrement dans le coin inférieur droit.

   ![](assets/configure4.png)

1. Cliquez sur **[!UICONTROL Publier toutes les personnalisations]**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d’enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} maintenant.
* Exécutez le processus [Valider la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Il vérifie que vos configurations initiales ont été correctement effectuées.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 3 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md){target="_blank"}
