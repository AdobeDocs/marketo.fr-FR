---
unique-page-id: 3571807
description: Étape 2 sur 3 - Configuration de l’utilisateur de synchronisation Marketo dans Dynamics (2011 On-Premise) - Documents Marketo - Documentation du produit
title: Étape 2 sur 3 - Configuration de l’utilisateur de synchronisation Marketo dans Dynamics (2011 On-Premise)
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Étape 2 sur 3 : configuration de l’utilisateur de synchronisation Marketo dans Dynamics (2011 On-Premise) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Excellent travail en suivant les étapes précédentes, continuons à le faire.

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : installation de la solution Marketo (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}

## Attribution d’un rôle d’utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur de synchronisation Marketo uniquement à l’utilisateur de synchronisation Marketo. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Cela s’applique au module externe Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent disposer du rôle d’utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Le paramètre linguistique de l’utilisateur de synchronisation [ doit être défini sur Anglais](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Dans le menu inférieur gauche, sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Dans l’arborescence, sélectionnez **[!UICONTROL Administration]**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Sélectionnez **[!UICONTROL Users]**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Vous trouverez ici une liste des utilisateurs. Sélectionnez votre utilisateur de synchronisation Marketo dédié ou contactez votre administrateur [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} pour créer un nouvel utilisateur dédié à Marketo. Cliquez sur **[!UICONTROL Gérer les rôles]**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Cochez **[!UICONTROL Marketo Sync User]** et cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Si vous ne voyez pas le rôle, revenez à l’ [étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} et importez la solution.

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de synchronisation _not_ seront resynchronisées sur Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque fini ! Nous n&#39;avons que quelques derniers éléments de configuration avant de passer à l&#39;article suivant.

1. Sélectionnez **[!UICONTROL Paramètres]**. Sélectionnez ensuite **[!UICONTROL Marketo Config]** dans l’arborescence.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Si la configuration Marketo est manquante, essayez d’actualiser la page. Si le problème persiste, [publiez à nouveau la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} ou déconnectez-vous et reconnectez-vous.

1. Cliquez sur **[!UICONTROL Default]**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Cliquez sur ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Dans la fenêtre contextuelle, sélectionnez l’utilisateur de synchronisation. Cliquez ensuite sur **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Cliquez sur **[!UICONTROL Enregistrer]** pour enregistrer les modifications.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Cliquez sur **[!UICONTROL Publish Toutes les personnalisations]**.

   ![](assets/publish-all-customizations1.png)

## Avant de passer à l’étape 3 {#before-proceeding-to-step}

* Si vous souhaitez limiter le nombre d&#39;enregistrements que vous synchronisez, [configurez maintenant un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}.
* Exécutez le processus [Valider la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Il vérifie que vos premières configurations ont été effectuées correctement.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans Microsoft Dynamics CRM.

  Bon boulot !

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : connexion de Microsoft Dynamics à Marketo (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md){target="_blank"}
