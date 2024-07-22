---
unique-page-id: 3571816
description: Étape 2 sur 3 - Configuration de l’utilisateur de synchronisation pour Marketo (2013 On-Premise) - Documents Marketo - Documentation du produit
title: Étape 2 sur 3 - Configuration de l’utilisateur de synchronisation pour Marketo (2013 On-Premise)
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Étape 2 sur 3 : configuration de l’utilisateur de synchronisation pour Marketo (2013 On-Premise) {#step-of-configure-sync-user-for-marketo-on-premises}

Excellent travail en suivant les étapes précédentes, continuons à le faire.

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : installation de la solution Marketo dans Dynamics (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md){target="_blank"}

## Attribution d’un rôle d’utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur de synchronisation Marketo uniquement à l’utilisateur de synchronisation Marketo. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Cela s’applique au module externe Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent disposer du rôle d’utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Le paramètre linguistique de l’utilisateur de synchronisation [ doit être défini sur Anglais](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Sous **Settings**, cliquez sur **Administration**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Sélectionnez **Users**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Vous trouverez ici une liste des utilisateurs. Sélectionnez votre utilisateur de synchronisation Marketo dédié ou contactez votre administrateur [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} pour créer un nouvel utilisateur [dédié à Marketo](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx){target="_blank"}.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Sélectionnez l’utilisateur de synchronisation. Cliquez sur ![](assets/image2015-3-26-11-3a16-3a22.png) et sélectionnez **[!UICONTROL Gérer les rôles]**.

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Cochez **[!UICONTROL Marketo Sync User]** et cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l’ [étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md){target="_blank"} et importez la solution.

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de synchronisation _not_ seront resynchronisées sur Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque fini ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sous **[!UICONTROL Settings]**, cliquez sur **[!UICONTROL Marketo Config]**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Si &quot;Configuration Marketo&quot; est manquante, essayez d’actualiser la page. Si le problème persiste, [publiez à nouveau la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md) ou essayez de vous déconnecter puis de vous reconnecter.

1. Cliquez sur **[!UICONTROL Default]**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Cliquez sur le champ **[!UICONTROL Utilisateur Marketo]** et sélectionnez l’utilisateur de synchronisation.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Cliquez sur ![](assets/image2015-3-13-15-3a10-3a11.png) dans le coin inférieur droit pour enregistrer les modifications.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Cliquez sur **[!UICONTROL Publish Toutes les personnalisations]**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d&#39;enregistrements que vous synchronisez, [configurez maintenant un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}.
* Exécutez le processus [Valider la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Il vérifie que vos premières configurations ont été effectuées correctement.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans Microsoft Dynamics CRM.

Bon boulot !

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : connexion Marketo et Dynamics (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2013.md){target="_blank"}
