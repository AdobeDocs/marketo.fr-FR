---
unique-page-id: 7504744
description: Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 3 sur 3 - Documentation sur le marketing - Documentation sur le produit
title: Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 3 sur 3
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 3 sur 3 {#install-marketo-for-dynamics-on-prem-and-on-prem-step-of}

>[!PREREQUISITES]
>
>* [Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 1 sur 3](step-1-of-3-install.md)
>* [Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 2 sur 3](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Entrer les informations utilisateur Dynamics Sync {#enter-dynamics-sync-user-information}

1. Connectez-vous à Marketing et cliquez sur **Admin**.

   ![](assets/login-admin.png)

1. Cliquez sur **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Sélectionnez **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Cliquez sur **Modifier** à l’ **étape 1 : Saisissez des informations d’identification**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Assurez-vous que vos informations d’identification sont correctes car nous ne pouvons pas annuler les modifications de schéma suivantes après l’envoi. Si des informations d’identification incorrectes sont enregistrées, vous devrez obtenir un nouvel abonnement Marketo.

1. Saisissez le **nom d&#39;utilisateur**, le **mot de passe** une **URL** Microsoft Dynamics et un ID **de client facultatif.** Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/client-id.png)

   >[!NOTE]
   >
   >Le nom d’utilisateur dans Marketo doit correspondre au nom d’utilisateur de l’utilisateur synchronisé dans CRM. Le format peut être [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#8cf9ffe9fecce8e3e1ede5e2a2efe3e1) ou DOMAINE\utilisateur.

   >[!TIP]
   >
   >Vous ne connaissez pas l&#39;URL ? Nous vous montrerons comment trouver votre URL [de service d&#39;organisation](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) Dynamics ici.

## Sélectionner les champs à synchroniser {#select-fields-to-sync}

1. Cliquez sur **Modifier** à l’ **étape 2 : Sélectionnez Champs à synchroniser**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Sélectionnez les champs que vous souhaitez synchroniser avec Marketo afin qu’ils soient présélectionnés. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

## Champs de synchronisation pour un filtre personnalisé {#sync-fields-for-a-custom-filter}

Si vous avez créé un filtre personnalisé, veillez à entrer et à sélectionner les nouveaux champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **Modifier** dans Détails de synchronisation des champs.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler l’écran jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto, mais le nom d’affichage peut être n’importe quoi. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Activer la synchronisation {#enable-sync}

1. Cliquez sur **Modifier** à l’ **étape 3 : Activez Synchroniser**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo ne dédupliquera pas automatiquement une synchronisation Microsoft Dynamics ou lorsque vous entrez manuellement des personnes.

1. Lisez tout ce qui se trouve dans la fenêtre contextuelle, entrez votre adresse électronique, puis cliquez sur **Début Sync**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La première synchronisation peut prendre quelques heures. Une fois que vous aurez terminé, vous recevrez une notification par courrier électronique.

   ![](assets/image2015-3-16-9-59-51.png)

Excellent travail !
