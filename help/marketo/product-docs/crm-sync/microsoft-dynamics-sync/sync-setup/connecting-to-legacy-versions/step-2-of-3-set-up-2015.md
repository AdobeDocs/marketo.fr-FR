---
unique-page-id: 7504739
description: Installation de Marketo pour Microsoft Dynamics 2015 On-Premise Étape 2 sur 3 - Documentation Marketo - Documentation du produit
title: Installation de Marketo pour Microsoft Dynamics 2015 On-Premise Étape 2 sur 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Étape 2 sur 3 Configuration de Marketo pour Dynamics (On-Prem 2015){#step-of-set-up-for-marketo-on-premises-2015}

Excellent travail lors des étapes précédentes. Continuons à passer à travers ça.

>[!PREREQUISITES]
>
>[Installation de Marketo pour Microsoft Dynamics 2015 On-Premise Étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}

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

   >[!IMPORTANT]
   >
   >L’utilisateur de synchronisation doit disposer d’une autorisation en lecture sur la configuration Marketo.

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l’ [étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} et importez la solution.

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de synchronisation _not_ seront resynchronisées sur Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque fini ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sous **[!UICONTROL Settings]**, cliquez sur **[!UICONTROL Marketo Config]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Si la configuration Marketo est manquante, essayez d’actualiser la page. Si le problème persiste, [publiez la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} ou essayez de vous déconnecter et de vous reconnecter.

1. Cliquez sur **[!UICONTROL Default]**.

   ![](assets/configure2.png)

1. Cliquez sur le champ **[!UICONTROL Utilisateur Marketo]** et sélectionnez l’utilisateur de synchronisation.

   ![](assets/configure3.png)

1. Cliquez sur l’icône d’enregistrement dans le coin inférieur droit.

   ![](assets/configure4.png)

1. Cliquez sur **[!UICONTROL Publish Toutes les personnalisations]**.

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >L’utilisateur de synchronisation doit disposer d’une autorisation en lecture sur la configuration Marketo.

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d&#39;enregistrements que vous synchronisez, [configurez maintenant un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}.
* Exécutez le processus [Valider la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Il vérifie que vos premières configurations ont été effectuées correctement.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installation de Marketo pour Microsoft Dynamics 2015 On-Premise Étape 3 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md){target="_blank"}
