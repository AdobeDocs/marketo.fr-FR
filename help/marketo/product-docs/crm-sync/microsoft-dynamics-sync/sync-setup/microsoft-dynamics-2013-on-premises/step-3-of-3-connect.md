---
unique-page-id: 3571819
description: Étape 3 sur 3 - Connecter le marketing et la dynamique (local 2013) - Documents marketing - Documentation du produit
title: Étape 3 sur 3 - Connecter le marketing et la dynamique (local 2013)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Étape 3 sur 3 : Connect Marketo and Dynamics (2013 sur site) {#step-of-connect-marketo-and-dynamics-on-premises}

D&#39;accord ! Nous avons installé la solution et configuré l&#39;utilisateur de synchronisation. Ensuite, nous devons connecter Marketing et Dynamics.

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : Installer la solution Marketo dans Dynamics (local 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)
>* [Étape 2 sur 3 : Configurer l&#39;utilisateur de synchronisation pour Marketo (local 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)


>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Entrer les informations utilisateur de Dynamics Sync {#enter-dynamics-sync-user-information}

1. Connectez-vous à Marketing et cliquez sur **Admin**.

   ![](assets/login-admin.png)

1. Cliquez sur **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Sélectionnez **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Cliquez sur **Modifier** dans **Étape 1 : Saisissez les informations d’identification**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Assurez-vous que vos informations d’identification sont correctes car nous ne pouvons pas annuler les modifications de schéma suivantes après l’envoi. Si des informations d’identification incorrectes sont enregistrées, vous devrez obtenir un nouvel abonnement Marketo.

1. Entrez **Nom d’utilisateur**, **Mot de passe** et Microsoft Dynamics **URL**, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Le nom d’utilisateur dans Marketo doit correspondre au nom d’utilisateur de l’utilisateur synchronisé dans CRM. Le format peut être user@domain.com ou DOMAINE\utilisateur.

   >[!TIP]
   >
   >Vous ne connaissez pas l&#39;URL ? Nous vous montrerons comment trouver [Dynamics Organization Service URL](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) ici.

## Sélectionner les champs à synchroniser {#select-fields-to-sync}

Maintenant, nous devons sélectionner les champs sur lesquels nous voulons synchroniser.

1. Cliquez sur **Modifier** dans **Étape 2 : Sélectionnez Champs à synchroniser**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Sélectionnez les champs que vous souhaitez synchroniser avec Marketo afin qu’ils soient présélectionnés. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

## Champs de synchronisation pour un filtre personnalisé {#sync-fields-for-a-custom-filter}

Si vous avez créé un filtre personnalisé, veillez à entrer et à sélectionner les nouveaux champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **Modifier** sur Détails de synchronisation des champs.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler l’écran jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto, mais le nom d’affichage peut être n’importe quoi. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Activer la synchronisation {#enable-sync}

1. Cliquez sur **Modifier** dans **Étape 3 : Activez Sync**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo ne dédupliquera pas automatiquement une synchronisation Microsoft Dynamics ou lorsque vous entrez manuellement des personnes ou des pistes.

1. Lisez tous les éléments de la fenêtre contextuelle, entrez votre adresse électronique, puis cliquez sur **Début Sync**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La première synchronisation peut prendre quelques heures. Une fois que vous aurez terminé, vous recevrez une notification par courrier électronique.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Excellent travail ! Vous venez de libérer la puissance de la synchronisation bidirectionnelle entre Marketo et Microsoft Dynamics. Si vous avez acheté Marketo Sales Insight, il y a plus de plaisir à avoir :

>[!MORELIKETHIS]
>
>[Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
