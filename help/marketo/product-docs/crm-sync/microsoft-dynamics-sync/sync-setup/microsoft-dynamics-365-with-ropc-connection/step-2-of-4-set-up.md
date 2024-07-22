---
description: Étape 2 sur 4 - Configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire des ressources - Documents Marketo - Documentation du produit
title: Étape 2 sur 4 - Configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 2eb61d43f2f470d42e1b50ab8edc99e4e25c23cf
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Étape 2 sur 4 : configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource {#step-2-of-4-set-up-the-marketo-solution-ropc}

Commençons par créer un compte utilisateur.

>[!PREREQUISITES]
>
>[Étape 1 sur 4 : installation de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## Création d’un utilisateur {#create-a-new-user}

1. Connectez-vous à Dynamics. Cliquez sur l’icône Paramètres et sélectionnez **[!UICONTROL Paramètres avancés]**.

   ![](assets/one.png)

1. Cliquez sur **[!UICONTROL Paramètres]** et sélectionnez **[!UICONTROL Sécurité]**.

   ![](assets/two.png)

1. Cliquez sur **[!UICONTROL Users]**.

   ![](assets/three.png)

1. Cliquez sur **[!UICONTROL New]**.

   ![](assets/four.png)

1. Cliquez sur **[!UICONTROL Ajouter et acquérir sous licence des utilisateurs]** dans la nouvelle fenêtre.

   ![](assets/five.png)

1. Un nouvel onglet s’ouvre. Cliquez sur **[!UICONTROL Admin]** en haut de la page.

   ![](assets/six.png)

1. Un autre nouvel onglet s’ouvre. Cliquez sur **[!UICONTROL Ajouter un utilisateur]**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >L’utilisateur de synchronisation doit disposer d’une autorisation en lecture sur la configuration Marketo.

1. Saisissez toutes vos informations. Une fois que vous avez terminé, cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Ce nom doit être un utilisateur de synchronisation dédié et non un compte d’utilisateur CRM existant. Il ne doit pas nécessairement s’agir d’une adresse électronique réelle.

1. Saisissez l’e-mail pour recevoir les nouvelles informations d’identification de l’utilisateur, puis cliquez sur **[!UICONTROL Envoyer un e-mail et fermer]**.

   ![](assets/nine.png)

## Attribution d’un rôle d’utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur de synchronisation Marketo uniquement à l’utilisateur de synchronisation Marketo. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Cela s’applique à Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent disposer du rôle d’utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Le paramètre linguistique de l’utilisateur de synchronisation [ doit être défini sur Anglais](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Revenez à l’onglet **[!UICONTROL Utilisateurs activés]** et actualisez la liste des utilisateurs.

   ![](assets/ten.png)

1. Passez la souris sur l’utilisateur de synchronisation Marketo nouvellement créé pour afficher une case à cocher. Cliquez pour le sélectionner.

   ![](assets/eleven.png)

1. Cliquez sur **[!UICONTROL Gérer les rôles]**.

   ![](assets/twelve.png)

1. Cochez **[!UICONTROL Marketo Sync User]** et cliquez sur **[!UICONTROL OK]**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de synchronisation _not_ seront resynchronisées sur Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque là ! Il ne nous reste plus qu’à informer la solution Marketo sur le nouvel utilisateur créé.

1. Revenez à la section Paramètres avancés et cliquez sur l’icône ![](assets/image2015-5-13-15-3a49-3a19.png) en regard de Paramètres, puis sélectionnez **[!UICONTROL Configuration Marketo]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Si vous ne voyez pas **[!UICONTROL Configuration Marketo]** dans le menu Paramètres, actualisez la page. Si cela ne fonctionne pas, essayez de [publier à nouveau la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"} ou déconnectez-vous et reconnectez-vous.

1. Cliquez sur **[!UICONTROL Default]**.

   ![](assets/fifteen.png)

1. Cliquez sur le bouton de recherche dans le champ **[!UICONTROL Utilisateur Marketo]** et sélectionnez l’utilisateur de synchronisation que vous avez créé.

   ![](assets/sixteen.png)

1. Cliquez sur l’icône ![](assets/image2015-3-13-15-3a10-3a11.png) dans le coin inférieur droit pour enregistrer les modifications.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Cliquez sur le **X** en haut à droite pour fermer l’écran.

   ![](assets/seventeen.png)

1. Cliquez sur l’icône ![](assets/image2015-5-13-15-3a49-3a19-1.png) en regard de Paramètres, puis sélectionnez **[!UICONTROL Solutions]**.

   ![](assets/eighteen.png)

1. Cliquez sur le bouton **[!UICONTROL Toutes les personnalisations de Publish]** .

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[Étape 3 sur 4 : Connecter la solution Marketo à la connexion de contrôle de mot de passe du propriétaire de ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
