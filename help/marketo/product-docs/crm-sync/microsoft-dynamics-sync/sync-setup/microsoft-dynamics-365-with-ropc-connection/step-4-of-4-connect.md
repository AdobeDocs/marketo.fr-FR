---
description: Étape 4 sur 4 - Connexion de la solution Marketo à la connexion de contrôle de mot de passe du propriétaire de la ressource - Documents Marketo - Documentation du produit
title: Étape 4 sur 4 - Connexion de la solution Marketo à la connexion de contrôle de mot de passe du propriétaire de la ressource
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 3%

---

# Étape 4 de 4 : connecter la solution Marketo à la connexion de contrôle de mot de passe du propriétaire de la ressource {#step-4-of-4-connect-the-marketo-solution-ropc}

Il s’agit de la dernière étape de la synchronisation. Vous y êtes presque !

>[!PREREQUISITES]
>
>* [Étape 1 de 4 : installer la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Étape 2 de 4 : configurer la solution Marketo avec une connexion de contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [Étape 3 sur 4 : configurer l’application cliente sur MS [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Si vous effectuez une mise à niveau de l’authentification de base vers l’authentification [!DNL OAuth], vous pouvez utiliser [cet article](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) pour reconfigurer votre authentification.

## Saisir les informations sur l’utilisateur de la synchronisation [!DNL Dynamics] {#enter-dynamics-sync-user-information}

1. Connectez-vous à Marketo et cliquez sur **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Cliquez sur **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Sélectionnez **[!UICONTROL Microsoft]**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Cliquez sur **[!UICONTROL Modifier]** à l’étape **[!UICONTROL 1 : Saisie des informations d’identification]**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Assurez-vous que l’URL de votre organisation est correcte, car nous ne pouvons pas annuler les modifications de schéma suivantes après l’envoi. Si une URL d’organisation incorrecte est utilisée, vous devrez obtenir un nouvel abonnement Marketo. Si vous ne connaissez pas l’URL, [apprenez à la trouver ici](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!NOTE]
   >
   >Avant de saisir de nouvelles informations d’identification, vous pouvez [les valider ici](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}.

1. Saisissez les valeurs **[!UICONTROL Nom d’utilisateur]**, **[!UICONTROL Mot de passe]**, [!DNL Microsoft Dynamics] **[!UICONTROL URL]**, **[!UICONTROL Identifiant client]** et **[!UICONTROL Secret client]**. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Le nom d’utilisateur dans Marketo doit correspondre au nom d’utilisateur pour l’utilisateur de synchronisation dans CRM. Le format peut être `user@domain.com` ou DOMAINE\utilisateur.

## Sélectionner les champs à synchroniser {#select-fields-to-sync}

1. Cliquez sur **[!UICONTROL Modifier]** à l’étape **[!UICONTROL 2 : sélection des champs à synchroniser]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Sélectionnez les champs que vous souhaitez synchroniser avec Marketo afin qu’ils soient présélectionnés. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans [!DNL Dynamics], nous vous recommandons de le faire avec la [synchronisation désactivée](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Ensuite, actualisez le schéma dans Marketo en modifiant et en enregistrant le [ Sélectionner les champs à synchroniser ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Synchroniser les champs pour un filtre personnalisé {#sync-fields-for-a-custom-filter}

Si vous avez créé un filtre personnalisé, veillez à y accéder et à sélectionner les nouveaux champs à synchroniser avec Marketo.

1. Accédez à [!UICONTROL Admin] et sélectionnez **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **[!UICONTROL Modifier]** sur [!UICONTROL Détails de la synchronisation des champs].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto mais le Nom d&#39;affichage peut être n&#39;importe quoi. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Activer la synchronisation {#enable-sync}

1. Cliquez sur **[!UICONTROL Modifier]** à l’**[!UICONTROL Étape 3 : activer la synchronisation]**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo ne déduplique pas automatiquement les données par rapport à une synchronisation [!UICONTROL Microsoft Dynamics] ou lorsque vous saisissez manuellement des personnes ou des prospects.

1. Lisez tout ce qui se trouve dans le pop-up, saisissez votre adresse e-mail, puis cliquez sur **[!UICONTROL Démarrer la synchronisation]**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. Selon le nombre d’enregistrements, la synchronisation initiale peut prendre entre quelques heures et quelques jours. Vous recevrez une notification par e-mail une fois l’opération terminée.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

>[!MORELIKETHIS]
>
>[Reconfigure [!DNL Dynamics] Authentication Method](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)
