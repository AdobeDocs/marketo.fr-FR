---
description: Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 3 sur 3 - Documents Marketo - Documentation du produit
title: Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 3 sur 3
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 2%

---

# Étape 3 sur 3 : connexion Marketo Dynamics (2016 On Prem/Dynamics 365 On-Premise) {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 1 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}
>* [Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 2 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Entrer les informations sur l’utilisateur de synchronisation Dynamics {#enter-dynamics-sync-user-information}

1. Connectez-vous à Marketo et cliquez sur **[!UICONTROL Administration]**.

   ![](assets/login-admin.png)

1. Cliquez sur **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Sélectionner **[!DNL Microsoft]**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Cliquez sur **[!UICONTROL Modifier]** in **[!UICONTROL Saisie des informations d’identification]**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Assurez-vous que vos informations d’identification sont correctes, car nous ne pouvons pas annuler les modifications de schéma suivantes après l’envoi. Si des informations d’identification incorrectes sont enregistrées, vous devrez obtenir un nouvel abonnement Marketo.

1. Saisissez le **[!UICONTROL Nom d’utilisateur]**, **[!UICONTROL Password]** Microsoft Dynamics **[!UICONTROL URL]**, et a **Identifiant/secret du client**. Cliquez sur **[!UICONTROL Enregistrer]** une fois terminé.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Si votre Marketo a été configuré avant octobre 2020, l’identifiant du client et le secret sont des champs facultatifs. Sinon, elles sont obligatoires. L’obtention de ces informations dépend de la version de MSD que vous utilisez.
   >* Le nom d’utilisateur dans Marketo doit correspondre au nom d’utilisateur de l’utilisateur synchronisé dans le CRM. Le format peut être `user@domain.com` ou DOMAIN\user.
   >* Si vous ne connaissez pas l’URL, [découvrez comment le trouver ici](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!TIP]
   >
   >Vous ne connaissez pas l&#39;URL ? Nous vous montrerons comment trouver votre [URL du service d’organisation Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) ici.

## Sélectionner les champs à synchroniser {#select-fields-to-sync}

1. Cliquez sur **[!UICONTROL Modifier]** in **[!UICONTROL Sélectionner les champs à synchroniser]**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Sélectionnez les champs que vous souhaitez synchroniser avec Marketo afin qu’ils soient pré-sélectionnés. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans Dynamics, nous vous recommandons de le faire avec la variable [sync désactivé](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Then refresh the schema in Marketo by editing and saving the [Select Fields to Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Champs de synchronisation pour un filtre personnalisé {#sync-fields-for-a-custom-filter}

Si vous avez créé un filtre personnalisé, veillez à entrer et sélectionner les nouveaux champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **[!DNL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **[!UICONTROL Modifier]** sur Détails de synchronisation du champ.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler l’écran jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto, mais le nom d’affichage peut être de n’importe quel type. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Activer la synchronisation {#enable-sync}

1. Cliquez sur **[!UICONTROL Modifier]** in **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo ne procède pas automatiquement à la déduplication par rapport à une synchronisation Microsoft Dynamics, ni lorsque vous saisissez manuellement des personnes.

1. Lisez tout ce qui se trouve dans la fenêtre contextuelle, entrez votre adresse électronique, puis cliquez sur **[!UICONTROL Démarrer la synchronisation]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La première synchronisation peut prendre quelques heures. Une fois cette opération terminée, vous recevrez une notification par e-mail.

   ![](assets/image2015-3-16-9-59-51.png)

Excellent travail !
