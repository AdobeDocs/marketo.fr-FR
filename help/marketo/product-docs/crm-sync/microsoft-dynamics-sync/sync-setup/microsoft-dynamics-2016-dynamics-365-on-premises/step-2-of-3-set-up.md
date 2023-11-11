---
description: Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 2 sur 3 - Documents Marketo - Documentation du produit
title: Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 2 sur 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Étape 2 sur 3 Configuration de Marketo pour Dynamics (On-Prem/Dynamics 365 On-Premise 2016){#step-of-set-up-for-marketo-on-premises-2016}

Excellent travail lors des étapes précédentes. Continuons à passer à travers ça.

>[!PREREQUISITES]
>
>[Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}

## Création d’un utilisateur {#create-a-new-user}

1. Connectez-vous à Dynamics. Cliquez sur l’icône Paramètres et sélectionnez Paramètres avancés.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Cliquez sur **[!UICONTROL Paramètres]** et sélectionnez **[!UICONTROL Sécurité]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Cliquez sur **[!UICONTROL Utilisateurs]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Cliquez sur **[!UICONTROL Nouveau]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Cliquez sur **[!UICONTROL Ajout d’utilisateurs et licence]**. Un nouvel onglet doit s’ouvrir.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Cliquez sur **[!UICONTROL Administration]** en haut de la page. Un autre nouvel onglet doit s’ouvrir.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Cliquez sur **[!UICONTROL Ajout d’un utilisateur]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Saisissez toutes vos informations. Lorsque vous avez terminé, cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Ce nom doit être un utilisateur de synchronisation dédié et non un compte d’utilisateur CRM existant. Il ne doit pas nécessairement s’agir d’une adresse électronique réelle.

1. Saisissez l’e-mail pour recevoir les nouvelles informations d’identification de l’utilisateur, cliquez sur Envoyer un e-mail , puis fermez-le.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Création d’une application cliente {#create-a-new-client-application}

Suivez les étapes décrites dans la section [cet article Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later){target="_blank"} pour créer une demande client et accorder des autorisations. Notez l’ID/le secret client de l’application cliente Dynamics.

## Attribution d’un rôle d’utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur de synchronisation Marketo uniquement à l’utilisateur de synchronisation Marketo. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Cela s’applique à Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent disposer du rôle d’utilisateur de synchronisation. Pour mettre à niveau votre Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Paramètre de langue de l’utilisateur de synchronisation [doit être défini sur Anglais.](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Sous **[!UICONTROL Paramètres]**, cliquez sur **[!UICONTROL Sécurité]**.

   ![](assets/assign1.png)

1. Cliquez sur **[!UICONTROL Utilisateurs]**.

   ![](assets/assign2.png)

1. Vous trouverez ici une liste des utilisateurs. Sélectionnez l’utilisateur de synchronisation Marketo dédié ou contactez votre [Services de fédération Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS) pour créer un utilisateur dédié à Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Sélectionnez l’utilisateur de synchronisation. Cliquez sur **[!UICONTROL Gestion des rôles]**.

   ![](assets/assign4.png)

1. Cochez Utilisateur de synchronisation Marketo et cliquez sur **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à [étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) et importez la solution.

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de synchronisation _not_ être synchronisé à nouveau avec Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque fini ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sous **[!UICONTROL Paramètres]**, cliquez sur **[!UICONTROL Configuration Marketo]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si la configuration Marketo est manquante, essayez d’actualiser la page. Si le problème persiste, [publier la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"} ou essayez de vous déconnecter puis de vous reconnecter.

1. Cliquez sur **[!UICONTROL Par défaut]**.

   ![](assets/configure2.png)

1. Cliquez sur le bouton **[!UICONTROL Utilisateur Marketo]** et sélectionnez l’utilisateur de synchronisation.

   ![](assets/configure3.png)

1. Cliquez sur l’icône d’enregistrement dans le coin inférieur droit.

   ![](assets/configure4.png)

1. Cliquez sur **[!UICONTROL Publier toutes les personnalisations]**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d&#39;enregistrements synchronisés, [configurer un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} maintenant.
* Exécutez la variable [Validation de la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} processus. Il vérifie que vos premières configurations ont été effectuées correctement.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 3 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md){target="_blank"}
