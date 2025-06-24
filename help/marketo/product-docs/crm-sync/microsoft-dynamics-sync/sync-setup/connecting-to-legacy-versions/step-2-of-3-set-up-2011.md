---
unique-page-id: 3571807
description: Étape 2 sur 3 - Configurer l’utilisateur de synchronisation Marketo dans Dynamics (2011 On-Premise) - Documents Marketo - Documentation du produit
title: Étape 2 sur 3 - Configurer l'utilisateur de synchronisation Marketo dans Dynamics (2011 On-Premise)
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Étape 2 sur 3 : configurer l&#39;utilisateur de synchronisation Marketo dans Dynamics (2011 On-Premise) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Excellent travail pour terminer les étapes précédentes, continuons à avancer dans ce dossier.

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : installation de la solution Marketo (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}

## Affecter un rôle d&#39;utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur de synchronisation Marketo uniquement à l’utilisateur de synchronisation Marketo. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Cela s’applique aux versions 4.0.0.14 et ultérieures du plug-in Marketo. Pour les versions antérieures, tous les utilisateurs doivent disposer du rôle d’utilisateur de synchronisation . Pour mettre à niveau Marketo, voir [Mettre à niveau la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Le paramètre de langue de l’utilisateur de synchronisation [doit être défini sur Anglais](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Dans le menu inférieur gauche, sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Dans l’arborescence, sélectionnez **[!UICONTROL Administration]**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Sélectionnez **[!UICONTROL Utilisateurs]**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Une liste des utilisateurs s’affiche ici. Sélectionnez l’utilisateur de synchronisation Marketo dédié ou contactez votre administrateur [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} pour créer un nouvel utilisateur dédié à Marketo. Cliquez sur **[!UICONTROL Gérer les rôles]**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Cochez **[!UICONTROL Utilisateur de synchronisation Marketo]** puis cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l’[étape 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} et importez la solution.

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de la synchronisation ne _pas_ seront resynchronisées avec Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque terminé ! Nous avons juste quelques derniers éléments de configuration avant de passer à l’article suivant.

1. Sélectionnez **[!UICONTROL Paramètres]**. Sélectionnez ensuite **[!UICONTROL Configuration Marketo]** dans l’arborescence.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Si la configuration de Marketo est manquante, essayez d’actualiser la page. Si le problème persiste, [republiez la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} ou déconnectez-vous et reconnectez-vous.

1. Cliquez sur **[!UICONTROL Par défaut]**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Cliquez sur ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Dans la pop-up, sélectionnez l’utilisateur ou l’utilisatrice de synchronisation. Cliquez ensuite sur **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Cliquez sur **[!UICONTROL Enregistrer]** pour enregistrer les modifications.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Cliquez sur **[!UICONTROL Publier toutes les personnalisations]**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d’enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} maintenant.
* Exécutez le processus [Valider la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Il vérifie que vos configurations initiales ont été correctement effectuées.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans Microsoft Dynamics CRM.

  Bon boulot !

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : Connexion de Microsoft Dynamics à Marketo (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md){target="_blank"}
