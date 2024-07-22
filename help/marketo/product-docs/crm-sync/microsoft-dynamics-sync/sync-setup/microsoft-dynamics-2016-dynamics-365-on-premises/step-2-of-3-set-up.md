---
description: Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 2 sur 3 - Documents Marketo - Documentation du produit
title: Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 2 sur 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '496'
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

1. Cliquez sur **[!UICONTROL Users]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Cliquez sur **[!UICONTROL New]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Cliquez sur **[!UICONTROL Ajouter et acquérir sous licence des utilisateurs]**. Un nouvel onglet doit s’ouvrir.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Cliquez sur **[!UICONTROL Admin]** en haut de la page. Un autre nouvel onglet doit s’ouvrir.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Cliquez sur **[!UICONTROL Ajouter un utilisateur]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Saisissez toutes vos informations. Une fois que vous avez terminé, cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Ce nom doit être un utilisateur de synchronisation dédié et non un compte d’utilisateur CRM existant. Il ne doit pas nécessairement s’agir d’une adresse électronique réelle.

1. Saisissez l’e-mail pour recevoir les nouvelles informations d’identification de l’utilisateur, cliquez sur Envoyer un e-mail , puis fermez-le.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Création d’une application cliente {#create-a-new-client-application}

Suivez les étapes décrites dans [cet article de Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later){target="_blank"} pour créer une demande client et accorder des autorisations. Notez l’ID/le secret client de l’application cliente Dynamics.

## Attribution d’un rôle d’utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur de synchronisation Marketo uniquement à l’utilisateur de synchronisation Marketo. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Cela s’applique à Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent disposer du rôle d’utilisateur de synchronisation. Pour mettre à niveau votre Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Le paramètre linguistique de l’utilisateur de synchronisation [ doit être défini sur Anglais](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Sous **[!UICONTROL Settings]**, cliquez sur **[!UICONTROL Security]**.

   ![](assets/assign1.png)

1. Cliquez sur **[!UICONTROL Users]**.

   ![](assets/assign2.png)

1. Vous trouverez ici une liste des utilisateurs. Sélectionnez l’utilisateur de synchronisation Marketo dédié ou contactez votre administrateur [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS) pour créer un utilisateur dédié pour Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Sélectionnez l’utilisateur de synchronisation. Cliquez sur **[!UICONTROL Gérer les rôles]**.

   ![](assets/assign4.png)

1. Cochez Utilisateur de synchronisation Marketo et cliquez sur **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l’ [étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) et importez la solution.

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de synchronisation _not_ seront resynchronisées sur Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque fini ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sous **[!UICONTROL Settings]**, cliquez sur **[!UICONTROL Marketo Config]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si la configuration Marketo est manquante, essayez d’actualiser la page. Si le problème persiste, [publiez la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"} ou essayez de vous déconnecter et de vous reconnecter.

1. Cliquez sur **[!UICONTROL Default]**.

   ![](assets/configure2.png)

1. Cliquez sur le champ **[!UICONTROL Utilisateur Marketo]** et sélectionnez l’utilisateur de synchronisation.

   ![](assets/configure3.png)

1. Cliquez sur l’icône d’enregistrement dans le coin inférieur droit.

   ![](assets/configure4.png)

1. Cliquez sur **[!UICONTROL Publish Toutes les personnalisations]**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d&#39;enregistrements que vous synchronisez, [configurez maintenant un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}.
* Exécutez le processus [Valider la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Il vérifie que vos premières configurations ont été effectuées correctement.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 3 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md){target="_blank"}
