---
unique-page-id: 3571809
description: Étape 3 sur 3 - Connecter Microsoft Dynamics à Marketo (local 2011) - Marketo Docs - Documentation sur les produits
title: Étape 3 sur 3 - Connecter Microsoft Dynamics à Marketo (local 2011)
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 1%

---

# Étape 3 sur 3 : Connecter Microsoft Dynamics à Marketo (local 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

D&#39;accord ! Nous avons installé la solution et configuré l&#39;utilisateur de synchronisation. Ensuite, nous devons connecter Marketo et Dynamics.

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : Installation de la solution Marketo (local 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)
>* [Étape 2 sur 3 : Configurer un utilisateur Marketo Sync dans Dynamics (local 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Entrer les informations utilisateur de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Connectez-vous à Marketo et cliquez sur **Admin**.

   ![](assets/login-admin.png)

1. Cliquez sur **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Cliquez sur **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Cliquez sur **Modifier** dans **Étape 1 : Entrez les informations d&#39;identification.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Assurez-vous que vos informations d’identification sont correctes car nous ne pouvons pas annuler les modifications de schéma suivantes après l’envoi. Si des informations d’identification incorrectes sont enregistrées, vous devrez obtenir un nouvel abonnement Marketo.

1. Saisissez le **nom d’utilisateur**, **mot de passe** et l’URL **CRM**, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Le nom d’utilisateur dans Marketo doit correspondre au nom d’utilisateur de l’utilisateur synchronisé dans CRM. Le format peut être `user@domain.com` ou DOMAINE\utilisateur.
   >* Si vous ne connaissez pas l&#39;URL, [apprenez comment la trouver ici](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Sélectionner les champs à synchroniser {#select-fields-to-sync}

Maintenant, nous devons sélectionner les champs sur lesquels nous voulons synchroniser.

1. Cliquez sur **Modifier** dans **Étape 2 : Sélectionnez les champs à synchroniser.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Certains champs présélectionnés seront synchronisés. Ajoutez plus si vous le souhaitez, puis cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans Dynamics, nous vous recommandons de le faire avec la [synchronisation désactivée](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Actualisez ensuite le schéma dans Marketo en modifiant et en enregistrant [Sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Champs de synchronisation pour un filtre personnalisé {#sync-fields-for-a-custom-filter}

Si vous avez créé un filtre personnalisé, veillez à entrer et à sélectionner les nouveaux champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **Modifier** sur Détails de synchronisation des champs.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler l’écran jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto, mais le nom d’affichage peut être n’importe quoi. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Activer la synchronisation {#enable-sync}

1. Cliquez sur **Modifier** dans **Étape 3 : Activez Sync**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo ne dédupliquera pas automatiquement une synchronisation Microsoft Dynamics ou lorsque vous entrez manuellement des personnes ou des pistes.

1. Lisez tous les éléments de la fenêtre contextuelle, entrez votre adresse électronique, puis cliquez sur **Début Sync**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La première synchronisation peut prendre quelques heures. Une fois que vous aurez terminé, vous recevrez une notification par courrier électronique.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Excellent travail !
