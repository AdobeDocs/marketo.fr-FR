---
description: Étape 4 sur 4 - Connexion de la solution Marketo à la connexion de contrôle de mot de passe du propriétaire de la ressource - Documents Marketo - Documentation du produit
title: Étape 4 sur 4 - Connexion de la solution Marketo à la connexion du contrôle de mot de passe du propriétaire de la ressource
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
source-git-commit: f72f195e53d63e37ef2ed53980b9bffc59391430
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 1%

---

# Étape 4 sur 4 : Connexion de la solution Marketo à la connexion de contrôle de mot de passe du propriétaire des ressources {#step-4-of-4-connect-the-marketo-solution-ropc}

Il s’agit de la dernière étape de la synchronisation. Vous y êtes presque !

>[!PREREQUISITES]
>
>* [Étape 1 sur 4 : Installation de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire des ressources](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Étape 2 sur 4 : Configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire des ressources](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [Étape 3 sur 4 : Configuration de l’application cliente sur MS Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)


>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!IMPORTANT]
>
>Si vous effectuez une mise à niveau de l’authentification de base vers OAuth, vous devrez contacter [Prise en charge de Marketo](https://nation.marketo.com/t5/support/ct-p/Support) pour obtenir de l’aide sur la mise à jour des paramètres supplémentaires. L’activation de cette fonction interrompt temporairement la synchronisation jusqu’à ce que de nouvelles informations d’identification soient saisies et que la synchronisation soit réactivée. La fonctionnalité peut être désactivée (jusqu’à avril 2022) si vous souhaitez revenir à l’ancien mode d’authentification.

## Entrer les informations sur l’utilisateur de synchronisation Dynamics {#enter-dynamics-sync-user-information}

1. Connectez-vous à Marketo et cliquez sur **Administration**.

   ![](assets/login-admin.png)

1. Cliquez sur **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Sélectionner **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Cliquez sur **Modifier** in **Étape 1 : Saisie des informations d’identification**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Assurez-vous que votre URL d’organisation est correcte, car nous ne pouvons pas annuler les modifications de schéma suivantes après envoi. Si une URL d’organisation incorrecte est utilisée, vous devrez obtenir un nouvel abonnement Marketo. Si vous ne connaissez pas l’URL, [découvrez comment le trouver ici](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

   >[!NOTE]
   >
   >Avant de saisir de nouvelles informations d’identification, vous pouvez [valider ici](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

1. Saisissez le **Nom d’utilisateur**, **Mot de passe**, **ID client**, **Secret du client**, et Microsoft Dynamics **URL**. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/step-4-of-4-connect-the-marketo-solution-ropc-5.png)

   >[!NOTE]
   >
   >Le nom d’utilisateur dans Marketo doit correspondre au nom d’utilisateur de l’utilisateur synchronisé dans le CRM. Le format peut être `user@domain.com` ou DOMAIN\user.

## Sélectionner les champs à synchroniser {#select-fields-to-sync}

1. Cliquez sur **Modifier** in **Étape 2 : Sélectionner les champs à synchroniser**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Sélectionnez les champs que vous souhaitez synchroniser avec Marketo afin qu’ils soient pré-sélectionnés. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans Dynamics, nous vous recommandons de le faire avec la variable [sync désactivé](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Actualisez ensuite le schéma dans Marketo en modifiant et en enregistrant le [Sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Champs de synchronisation pour un filtre personnalisé {#sync-fields-for-a-custom-filter}

Si vous avez créé un filtre personnalisé, veillez à entrer et sélectionner les nouveaux champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **Modifier** sur Détails de synchronisation du champ.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler l’écran jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto, mais le nom d’affichage peut être de n’importe quel type. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Activer la synchronisation {#enable-sync}

1. Cliquez sur **Modifier** in **Étape 3 : Activer la synchronisation**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo ne procède pas automatiquement à la déduplication par rapport à une synchronisation Microsoft Dynamics, ou lorsque vous saisissez manuellement des personnes ou des pistes.

1. Lisez tout ce qui se trouve dans la fenêtre contextuelle, entrez votre adresse électronique, puis cliquez sur **Démarrer la synchronisation**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La première synchronisation peut prendre quelques heures. Une fois cette opération terminée, vous recevrez une notification par e-mail.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Excellent travail !
