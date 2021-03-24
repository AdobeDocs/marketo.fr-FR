---
unique-page-id: 3571830
description: Étape 3 sur 3 - Connecter Microsoft Dynamics à Marketo (en ligne) - Docs marketing - Documentation sur le produit
title: Étape 3 sur 3 - Connecter Microsoft Dynamics avec Marketo (en ligne)
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---


# Étape 3 sur 3 : Connecter Microsoft Dynamics avec Marketo (en ligne) {#step-of-connect-microsoft-dynamics-with-marketo-online}

Il s’agit de la dernière étape de la synchronisation. Nous y sommes presque !

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : Installation de la solution Marketo (en ligne)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)
>* [Étape 2 sur 3 : Configurer un utilisateur de synchronisation de marketing dans Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Entrer les informations utilisateur de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Connectez-vous à Marketing et cliquez sur **Admin**.

   ![](assets/login-admin.png)

1. Cliquez sur **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Sélectionnez **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Cliquez sur **Modifier** dans **Étape 1 : Saisissez les informations d’identification**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Assurez-vous que vos informations d’identification sont correctes car nous ne pouvons pas annuler les modifications de schéma suivantes après l’envoi. Si des informations d’identification incorrectes sont enregistrées, vous devrez obtenir un nouvel abonnement Marketo.

1. Saisissez le **nom d’utilisateur**, **mot de passe** et l’URL de Microsoft Dynamics ****. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >* Si votre Marketo a été configuré avant octobre 2020, l’ID de client et le champ Secret sont des champs facultatifs. Sinon, elles sont obligatoires. L’obtention de ces informations dépendra de la version de MSD que vous utilisez.
   >* Le nom d’utilisateur dans Marketo doit correspondre au nom d’utilisateur de l’utilisateur synchronisé dans CRM. Le format peut être `user@domain.com` ou DOMAINE\utilisateur.
   >* Si vous ne connaissez pas l&#39;URL, [apprenez comment la trouver ici](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Sélectionner les champs à synchroniser {#select-fields-to-sync}

1. Cliquez sur **Modifier** dans **Étape 2 : Sélectionnez Champs à synchroniser**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Sélectionnez les champs que vous souhaitez synchroniser avec Marketo afin qu’ils soient présélectionnés. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans Dynamics, nous vous recommandons de le faire avec la [synchronisation désactivée](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Actualisez ensuite le schéma dans Marketo en modifiant et en enregistrant les [champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Champs de synchronisation pour un filtre personnalisé {#sync-fields-for-a-custom-filter}

Si vous avez créé un filtre personnalisé, veillez à entrer et à sélectionner les nouveaux champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **Modifier** sur Détails de synchronisation des champs.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler l’écran jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto, mais le nom d’affichage peut être n’importe quoi. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Activer la synchronisation {#enable-sync}

1. Cliquez sur **Modifier** dans **Étape 3 : Activez Sync**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo ne dédupliquera pas automatiquement une synchronisation Microsoft Dynamics ou lorsque vous entrez manuellement des personnes ou des pistes.

1. Lisez tout dans la fenêtre contextuelle, entrez votre adresse électronique, puis cliquez sur **Début Sync**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La première synchronisation peut prendre quelques heures. Une fois que c&#39;est fait, vous recevrez une notification par courriel.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Excellent travail !
