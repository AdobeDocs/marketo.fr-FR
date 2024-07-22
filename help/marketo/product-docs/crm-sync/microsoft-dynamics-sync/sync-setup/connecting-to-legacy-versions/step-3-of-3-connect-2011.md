---
unique-page-id: 3571809
description: Étape 3 sur 3 - Connexion de Microsoft Dynamics à Marketo (2011 On-Premise) - Documents Marketo - Documentation du produit
title: Étape 3 sur 3 - Connexion de Microsoft Dynamics à Marketo (local 2011)
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 2%

---

# Étape 3 sur 3 : connexion de Microsoft Dynamics à Marketo (On-Premise 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

D&#39;accord ! Nous avons installé la solution et configuré l’utilisateur de synchronisation. Ensuite, nous devons connecter Marketo et Dynamics.

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : installation de la solution Marketo (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}
>* [Étape 2 sur 3 : configuration de l’utilisateur de synchronisation Marketo dans Dynamics (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Entrer les informations utilisateur de synchronisation Dynamics {#enter-dynamics-sync-user-information}

1. Connectez-vous à Marketo et cliquez sur **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Cliquez sur **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Cliquez sur **[!DNL Microsoft]**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Cliquez sur **[!UICONTROL Modifier]** dans **[!UICONTROL Entrer les informations d’identification]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Assurez-vous que vos informations d’identification sont correctes, car nous ne pouvons pas annuler les modifications de schéma suivantes après l’envoi. Si des informations d’identification incorrectes sont enregistrées, vous devrez obtenir un nouvel abonnement Marketo.

1. Saisissez le **[!UICONTROL nom d&#39;utilisateur]**, le **[!UICONTROL mot de passe]** et le CRM **[!UICONTROL URL]**, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Le nom d’utilisateur dans Marketo doit correspondre au nom d’utilisateur de l’utilisateur synchronisé dans le CRM. Le format peut être `user@domain.com` ou DOMAIN\user.
   >* Si vous ne connaissez pas l&#39;URL, [ découvrez comment la trouver ici](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

## Sélectionner les champs à synchroniser {#select-fields-to-sync}

Maintenant, nous devons sélectionner les champs sur lesquels nous voulons effectuer la synchronisation.

1. Cliquez sur **[!UICONTROL Modifier]** dans **[!UICONTROL Sélectionner les champs à synchroniser]**.

   ![](assets/image2015-3-16-9-51-28a.png)

1. Certains champs présélectionnés seront synchronisés. Ajoutez-en davantage si vous le souhaitez, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans Dynamics, nous vous recommandons de le faire avec la [synchronisation désactivée](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Actualisez ensuite le schéma dans Marketo en modifiant et en enregistrant le [champ de sélection à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Champs de synchronisation pour un filtre personnalisé {#sync-fields-for-a-custom-filter}

Si vous avez créé un filtre personnalisé, veillez à entrer et sélectionner les nouveaux champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **[!UICONTROL Modifier]** sur Détails de la synchronisation des champs.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler l’écran jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto, mais le nom d’affichage peut être de n’importe quel type. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Activer la synchronisation {#enable-sync}

1. Cliquez sur **[!UICONTROL Modifier]** dans **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo ne procède pas automatiquement à la déduplication par rapport à une synchronisation Microsoft Dynamics, ou lorsque vous saisissez manuellement des personnes ou des pistes.

1. Lisez tout ce qui se trouve dans la fenêtre contextuelle, entrez votre adresse électronique, puis cliquez sur **[!UICONTROL Démarrer la synchronisation]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La première synchronisation peut prendre quelques heures. Une fois cette opération terminée, vous recevrez une notification par e-mail.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Excellent travail !
