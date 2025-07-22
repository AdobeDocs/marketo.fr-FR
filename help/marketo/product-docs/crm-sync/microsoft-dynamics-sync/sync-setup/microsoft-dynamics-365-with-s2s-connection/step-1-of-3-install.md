---
description: Étape 1 sur 3 - Installer la solution Marketo avec une connexion de serveur à serveur - Documents Marketo - Documentation du produit
title: Étape 1 sur 3 - Installer la solution Marketo avec une connexion de serveur à serveur
exl-id: bf6f87c1-5ba5-490b-bcce-365120af3730
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Étape 1 sur 3 : installer la solution Marketo avec une connexion serveur à serveur {#step-1-of-3-install-the-marketo-solution-s2s}

Avant de pouvoir synchroniser [!DNL Microsoft Dynamics 365] et Marketo, vous devez d’abord installer la solution Marketo dans [!DNL Dynamics]. **[!DNL Dynamics]autorisations d’administrateur sont requises.**

>[!CAUTION]
>
>N’activez pas la synchronisation d’entités personnalisées avant la fin de la synchronisation initiale. Vous serez averti par e-mail une fois la synchronisation initiale terminée.

>[!NOTE]
>
>Après avoir synchronisé Marketo avec un CRM, vous ne pouvez pas effectuer de nouvelle synchronisation sans remplacer l’instance .

>[!PREREQUISITES]
>
>[Télécharger la solution de gestion des prospects Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}

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

1. De retour sur la page [!UICONTROL Informations sur la solution], cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Assurez-vous que la case option SDK est cochée. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles sur votre navigateur pour terminer le processus d’installation.

1. Attendez maintenant la fin de l’importation.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Cliquez sur **[!UICONTROL Fermer]**.

   >[!NOTE]
   >
   >Il se peut qu’un message indiquant « Marketo Lead Management terminé avec un avertissement » s’affiche. Cela est tout à fait prévu.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. [!UICONTROL Gestion des leads Marketo] s’affiche désormais dans la liste des solutions.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Sélectionnez **[!UICONTROL Marketo Lead Management]** puis cliquez sur **[!UICONTROL Publier toutes les personnalisations]**.

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Cinq ans ! L&#39;installation est terminée.

   >[!MORELIKETHIS]
   >
   >[Étape 2 de 3 : configurer la solution Marketo avec la connexion S2S](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
