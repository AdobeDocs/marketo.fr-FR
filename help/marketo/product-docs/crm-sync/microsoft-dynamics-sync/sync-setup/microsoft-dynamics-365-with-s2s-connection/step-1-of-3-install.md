---
description: Étape 1 sur 3 - Installation de la solution Marketo avec la connexion serveur à serveur - Documents Marketo - Documentation du produit
title: Étape 1 sur 3 - Installation de la solution Marketo avec la connexion serveur à serveur
exl-id: bf6f87c1-5ba5-490b-bcce-365120af3730
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Étape 1 sur 3 : installation de la solution Marketo avec connexion serveur à serveur {#step-1-of-3-install-the-marketo-solution-s2s}

Avant de pouvoir synchroniser Microsoft Dynamics 365 et Marketo, vous devez installer la solution Marketo dans Dynamics. **Les autorisations d’administrateur Dynamics sont requises**.

>[!CAUTION]
>
>N’activez pas la synchronisation des entités personnalisées avant l’exécution de la synchronisation initiale. Une fois la synchronisation initiale terminée, vous en serez informé par e-mail.

>[!NOTE]
>
>Une fois que vous avez synchronisé Marketo avec un CRM, vous ne pouvez pas effectuer une nouvelle synchronisation sans remplacer l’instance.

>[!PREREQUISITES]
>
>[Télécharger la solution Marketo Lead Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}

1. Connectez-vous à [Microsoft Office 365](https://login.microsoftonline.com/){target="_blank"}.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Cliquez sur le menu ![](assets/image2015-3-16-16-3a1-3a13.png) et sélectionnez **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Cliquez sur le menu ![](assets/image2015-5-13-10-3a5-3a8.png) . Dans le menu déroulant, sélectionnez **[!UICONTROL Paramètres]**, puis **[!UICONTROL Solutions]**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Cliquez sur **[!UICONTROL Choisir un fichier]**. Sélectionnez la solution Marketo Lead Management que vous avez [ téléchargée ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Affichez les informations sur la solution et cliquez sur **[!UICONTROL Afficher les détails du package de solution]**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Lorsque vous avez terminé de vérifier tous les détails, cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Maintenant, de retour sur la page Informations sur la solution, cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Assurez-vous que la case à cocher de l’option SDK est cochée. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles de votre navigateur pour terminer le processus d’installation.

1. Maintenant, attendez la fin de l’importation.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Cliquez sur **[!UICONTROL Fermer]**.

   >[!NOTE]
   >
   >Un message peut s’afficher indiquant &quot;Gestion des pistes Marketo terminée avec un avertissement&quot;. Cela est tout à fait attendu.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. &quot;Gestion des prospects Marketo&quot; apparaît désormais dans la liste des solutions.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Sélectionnez **[!UICONTROL Gestion des pistes Marketo]** et cliquez sur **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Cinq heures de haut ! L’installation est terminée.

   >[!MORELIKETHIS]
   >
   >[Étape 2 sur 3 : configuration de la solution Marketo avec la connexion S2S](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
