---
unique-page-id: 3571813
description: Étape 1 sur 3 - Installer la solution Marketo dans Dynamics (2013 On-Premise) - Documents Marketo - Documentation du produit
title: Étape 1 sur 3 - Installer la solution Marketo dans Dynamics (2013 On-Premise)
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Étape 1 sur 3 : Installer la solution Marketo dans Dynamics (2013 On-Premise) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Avant de pouvoir synchroniser Microsoft Dynamics On-Premise et Marketo Engage, vous devez d’abord installer la solution Marketo dans Dynamics.

>[!NOTE]
>
>Après avoir synchronisé Marketo avec un CRM, vous ne pouvez pas effectuer de nouvelle synchronisation sans remplacer l’instance .

>[!PREREQUISITES]
>
>Vous devez avoir configuré [Internet Facing Deployment](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} (IFD) avec [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 ou 3.0 (ADFS). Remarque : le document IFD est téléchargé automatiquement lorsque vous cliquez sur le lien.
>
>[Téléchargez la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} avant de commencer.

>[!NOTE]
>
>**Autorisations d’administrateur Dynamics requises**.
>
>Vous avez besoin de privilèges d’administrateur CRM pour effectuer cette synchronisation.

1. Connectez-vous à Dynamics. Cliquez sur le menu déroulant **[!UICONTROL Microsoft Dynamics CRM]** et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Sous **[!UICONTROL Paramètres]**, sélectionnez **[!UICONTROL Solutions]**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Cliquez sur **[!UICONTROL Parcourir]** et sélectionnez la [solution téléchargée](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Affichez les informations sur la solution et cliquez sur **[!UICONTROL Afficher les détails du package de solution]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Une fois la vérification de tous les détails terminée, cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. De retour sur la page Informations sur la solution, cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Assurez-vous que l’option SDK est cochée. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Attendez la fin de l’importation.

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles sur votre navigateur pour terminer le processus d’installation.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Téléchargez un fichier journal (si vous le souhaitez) et cliquez sur **[!UICONTROL Fermer]**.

   >[!NOTE]
   >
   >Il se peut qu’un message indiquant « Marketo Lead Management terminé avec un avertissement » s’affiche. Cela est tout à fait prévu.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. La gestion des prospects Marketo apparaît désormais sur la page **[!UICONTROL Toutes les solutions]**.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Sélectionnez la solution Marketo et cliquez sur **[!UICONTROL Publier toutes les personnalisations]**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

>[!CAUTION]
>
>La désactivation de l’un des processus de messagerie SDK de Marketo entraînera une installation interrompue.

>[!MORELIKETHIS]
>
>[Étape 2 de 3 : configurer l’utilisateur de synchronisation pour Marketo (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md){target="_blank"}
