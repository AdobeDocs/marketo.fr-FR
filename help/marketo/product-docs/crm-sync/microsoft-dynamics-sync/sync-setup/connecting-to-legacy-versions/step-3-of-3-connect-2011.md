---
unique-page-id: 3571809
description: Découvrez comment connecter Microsoft Dynamics 2011 local à Marketo à l’étape finale. Saisissez les informations sur l’utilisateur synchronisé dans Marketo Admin et activez la synchronisation.
title: Étape 3 sur 3 - Connexion  [!DNL Microsoft Dynamics]  Marketo (2011 On-Premise)
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/lXIts5epOGhGJLKvIKTOAdOABz15rNAfuSmvHuSC0SI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 379
ht-degree: 2%

---

# Étape 3 sur 3 : Connexion de [!DNL Microsoft Dynamics] à Marketo (2011 On-Premise) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

La solution est installée et l’utilisateur de synchronisation est configuré. Ensuite, connectez Marketo et [!DNL Dynamics].

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : installation de la solution Marketo (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)
>* [Étape 2 de 3 : configurer l’utilisateur de synchronisation Marketo dans  [!DNL Dynamics] (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)

>[!NOTE]
>
>**Autorisations d’administration requises**

## Saisir les informations sur l’utilisateur de la synchronisation [!DNL Dynamics] {#enter-dynamics-sync-user-information}

1. Connectez-vous à Marketo et cliquez sur **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Cliquez sur **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Cliquez sur **&#x200B;**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Cliquez sur **[!UICONTROL Modifier]** à l’étape **[!UICONTROL 1 : saisir les informations d’identification]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Vérifiez que vos informations d’identification sont correctes. Les modifications de schéma suivantes ne peuvent pas être annulées après l’envoi. Si des informations d’identification incorrectes sont enregistrées, un nouvel abonnement Marketo sera nécessaire.

1. Saisissez les **[!UICONTROL Nom d’utilisateur]**, **[!UICONTROL Mot de passe]** et CRM **[!UICONTROL URL]** puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Le [!UICONTROL Nom d’utilisateur] dans Marketo doit correspondre au nom d’utilisateur de l’utilisateur de synchronisation dans CRM. Le format peut être `user@domain.com` ou DOMAINE\utilisateur.
   >* Si vous ne connaissez pas l’URL, [apprenez à la trouver ici](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

## Sélectionner les champs à synchroniser {#select-fields-to-sync}

Sélectionnez les champs à synchroniser.

1. Cliquez sur **[!UICONTROL Modifier]** à l’étape **[!UICONTROL 2 : sélection des champs à synchroniser]**.

   ![](assets/image2015-3-16-9-51-28a.png)

1. Certains champs présélectionnés seront synchronisés. Ajoutez d’autres éléments si vous le souhaitez, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans [!DNL Dynamics], nous vous recommandons de le faire avec la [synchronisation désactivée](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Ensuite, actualisez le schéma dans Marketo en modifiant et en enregistrant le [&#x200B; Sélectionner les champs à synchroniser &#x200B;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Synchroniser les champs pour un filtre personnalisé {#sync-fields-for-a-custom-filter}

Si vous avez créé un filtre personnalisé, accédez à et sélectionnez les nouveaux champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **&#x200B;**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **[!UICONTROL Modifier]** sur [!UICONTROL Détails de la synchronisation des champs].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto mais le Nom d&#39;affichage peut être n&#39;importe quoi. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Activer la synchronisation {#enable-sync}

1. Cliquez sur **[!UICONTROL Modifier]** à l’**[!UICONTROL Étape 3 : activer la synchronisation]**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo ne déduplique pas automatiquement les données par rapport à une synchronisation [!DNL Microsoft Dynamics] ou lorsque vous saisissez manuellement des personnes ou des prospects.

1. Lisez tout ce qui se trouve dans le pop-up, saisissez votre adresse e-mail, puis cliquez sur **[!UICONTROL Démarrer la synchronisation]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Selon le nombre d’enregistrements, la synchronisation initiale peut prendre entre quelques heures et quelques jours. Vous recevrez une notification par e-mail une fois l’opération terminée.

   ![](assets/image2014-12-11-11-3a55-3a15.png)
