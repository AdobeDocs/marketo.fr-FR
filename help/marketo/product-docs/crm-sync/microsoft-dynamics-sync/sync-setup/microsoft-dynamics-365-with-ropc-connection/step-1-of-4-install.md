---
description: Étape 1 sur 4 - Installer la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource - Documents Marketo - Documentation du produit
title: Étape 1 sur 4 - Installer la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 1%

---

# Étape 1 sur 4 : installer la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource {#step-1-of-4-install-the-marketo-solution-ropc}

Avant de pouvoir synchroniser [!DNL Microsoft Dynamics] 365 et Marketo, vous devez d’abord installer la solution Marketo dans [!DNL Dynamics]. **[!DNL Dynamics]autorisations d’administrateur sont requises.**

>[!CAUTION]
>
>* N’activez pas la synchronisation d’entités personnalisées avant la fin de la synchronisation initiale. Vous serez averti par e-mail une fois la synchronisation initiale terminée.
>* Si Multi-Factor Authentication (MFA) est activé pour votre synchronisation [!DNL Dynamics], vous devez la désactiver pour que [!DNL Dynamics] puissiez effectuer correctement la synchronisation avec Marketo. Pour plus d’informations, contactez l’assistance Marketo [](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>Après avoir synchronisé Marketo avec un CRM, vous ne pouvez pas effectuer de nouvelle synchronisation sans remplacer l’instance .

>[!PREREQUISITES]
>
>[Télécharger la solution de gestion des prospects Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Connectez-vous à **[[!DNL Microsoft Office 365]](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Cliquez sur ![](assets/image2015-3-16-16-3a1-3a13.png) menu et sélectionnez **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Cliquez sur ![](assets/image2015-5-13-10-3a5-3a8.png) menu. Dans le menu déroulant, sélectionnez **[!UICONTROL Paramètres]** puis **[!UICONTROL Solutions]**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Cliquez sur **[!UICONTROL Choisir un fichier]**. Sélectionnez la solution Marketo Lead Management que vous [téléchargé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Affichez les informations sur la solution et cliquez sur **[!UICONTROL Afficher les détails du package de solution]**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Une fois la vérification de tous les détails terminée, cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Maintenant, de retour sur la page Informations sur la solution, cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Assurez-vous que la case option SDK est cochée. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles sur votre navigateur pour terminer le processus d’installation.

1. Attendez maintenant la fin de l’importation. Lève-toi et fais des étirements.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Cliquez sur **[!UICONTROL Fermer]**.

   >[!NOTE]
   >
   >Il se peut qu’un message indiquant « Marketo Lead Management terminé avec un avertissement » s’affiche. Cela est tout à fait prévu.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. « Gestion des prospects Marketo » s’affiche désormais dans la liste des solutions.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Sélectionnez **[!UICONTROL Marketo Lead Management]** puis cliquez sur **[!UICONTROL Publier toutes les personnalisations]**.

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Beau travail ! L&#39;installation est terminée.

   >[!MORELIKETHIS]
   >
   >[Étape 2 de 4 : configurer la solution Marketo avec une connexion de contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
