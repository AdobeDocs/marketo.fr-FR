---
description: Étape 2 sur 3 - Configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource - Documents Marketo - Documentation du produit
title: Étape 2 sur 3 - Configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource
source-git-commit: 598390517dea96b0503fd9c0cdfd47bd7617b48a
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Étape 2 sur 3 : Configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire des ressources {#step-2-of-3-set-up-the-marketo-solution-ropc}

Commençons par créer un compte utilisateur.

>[!PREREQUISITES]
>
>[Étape 1 sur 4 : Installation de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire des ressources](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)

## Création d’un utilisateur {#create-a-new-user}

1. Connectez-vous à Dynamics. Cliquez sur l’icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres** et sélectionnez **Sécurité**.

   ![](assets/two.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/three.png)

1. Cliquez sur **Nouveau.**

   ![](assets/four.png)

1. Cliquez sur **Ajout d’utilisateurs et licence** dans la nouvelle fenêtre.

   ![](assets/five.png)

1. Un nouvel onglet s’ouvre. Cliquez sur **Administration** en haut de la page.

   ![](assets/six.png)

1. Un autre nouvel onglet s’ouvre. Cliquez sur **Ajout d’un utilisateur**.

   ![](assets/seven.png)

1. Saisissez toutes vos informations. Lorsque vous avez terminé, cliquez sur **Ajouter**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Ce nom doit être un utilisateur de synchronisation dédié et non un compte d’utilisateur CRM existant. Il n’est pas nécessaire qu’il s’agisse d’une adresse électronique réelle.

1. Saisissez l’e-mail de réception des nouvelles informations d’identification de l’utilisateur, puis cliquez sur **Envoyer un email et fermer**.

   ![](assets/nine.png)

## Attribution d’un rôle d’utilisateur de synchronisation {#assign-sync-user-role}

Attribuez le rôle Utilisateur de synchronisation Marketo uniquement à l’utilisateur de synchronisation Marketo. Vous n’avez pas besoin de l’affecter à d’autres utilisateurs.

>[!NOTE]
>
>Cela s’applique à Marketo version 4.0.0.14 et ultérieure. Pour les versions antérieures, tous les utilisateurs doivent disposer du rôle d’utilisateur de synchronisation. Pour mettre à niveau Marketo, voir [Mise à niveau de la solution Marketo pour Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Paramètre de langue de l’utilisateur de synchronisation [doit être défini sur Anglais.](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Revenez à l’onglet Utilisateurs activés et actualisez la liste des utilisateurs.

   ![](assets/ten.png)

1. Passez la souris sur l’utilisateur de synchronisation Marketo nouvellement créé pour afficher une case à cocher. Cliquez pour le sélectionner.

   ![](assets/eleven.png)

1. Cliquez sur **Gestion des rôles**.

   ![](assets/twelve.png)

1. Vérifier **Utilisateur de synchronisation Marketo** et cliquez sur **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Toutes les mises à jour effectuées dans votre CRM par l’utilisateur de synchronisation **not** être synchronisé à nouveau avec Marketo.

## Configuration de la solution Marketo {#configure-marketo-solution}

Presque là ! Il ne nous reste plus qu’à informer la solution Marketo sur le nouvel utilisateur créé.

1. Revenez à la section Paramètres avancés et cliquez sur le bouton ![](assets/image2015-5-13-15-3a49-3a19.png) en regard de Paramètres, sélectionnez **Configuration Marketo**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Si vous ne voyez pas **Configuration Marketo** dans le menu Paramètres , actualisez la page. Si cela ne fonctionne pas, essayez de [publier la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) de nouveau ou de se déconnecter puis de se reconnecter.

1. Cliquez sur **Par défaut**.

   ![](assets/fifteen.png)

1. Cliquez sur le bouton de recherche dans la **Utilisateur Marketo** et sélectionnez l’utilisateur de synchronisation que vous avez créé.

   ![](assets/sixteen.png)

1. Cliquez sur le bouton ![](assets/image2015-3-13-15-3a10-3a11.png) dans le coin inférieur droit pour enregistrer les modifications.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Cliquez sur le bouton **X** dans le coin supérieur droit pour fermer l’écran.

   ![](assets/seventeen.png)

1. Cliquez sur le bouton ![](assets/image2015-5-13-15-3a49-3a19-1.png) en regard de Paramètres, sélectionnez **Solutions**.

   ![](assets/eighteen.png)

1. Cliquez sur le bouton **Publier toutes les personnalisations** bouton .

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[Étape 3 sur 4 : Connexion de la solution Marketo à la connexion de contrôle de mot de passe du propriétaire des ressources](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)
