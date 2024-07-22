---
unique-page-id: 3571813
description: Étape 1 sur 3 - Installation de la solution Marketo dans Dynamics (On-Premise 2013) - Documents Marketo - Documentation du produit
title: Étape 1 sur 3 - Installation de la solution Marketo dans Dynamics (On-Premise 2013)
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Étape 1 sur 3 : installation de la solution Marketo dans Dynamics (On-Premise 2013) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Avant de pouvoir synchroniser Microsoft Dynamics On-Premise et Marketo Engage, vous devez installer la solution Marketo dans Dynamics.

>[!NOTE]
>
>Une fois que vous avez synchronisé Marketo avec un CRM, vous ne pouvez pas effectuer une nouvelle synchronisation sans remplacer l’instance.

>[!PREREQUISITES]
>
>Vous devez avoir [Déploiement Internet Face](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) avec [ Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 ou 3.0 (ADFS) configuré. Remarque : le document IFD se télécharge automatiquement lorsque vous cliquez sur le lien.
>
>[Téléchargez la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} avant de commencer.

>[!NOTE]
>
>**Autorisations d’administrateur Dynamics requises**.
>
>Pour effectuer cette synchronisation, vous avez besoin des privilèges d’administrateur CRM.

1. Connectez-vous à Dynamics. Cliquez sur le menu déroulant **[!UICONTROL Microsoft Dynamics CRM]** et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Sous **[!UICONTROL Settings]**, sélectionnez **[!UICONTROL Solutions]**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Cliquez sur **[!UICONTROL Parcourir]** et sélectionnez la [solution téléchargée](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Affichez les informations sur la solution et cliquez sur **[!UICONTROL Afficher les détails du package de solution]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Lorsque vous avez terminé de vérifier tous les détails, cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. De retour sur la page Informations sur la solution, cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Assurez-vous que l’option SDK est cochée. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Patientez jusqu’à la fin de l’importation.

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles de votre navigateur pour terminer le processus d’installation.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Téléchargez un fichier journal (si vous le souhaitez) et cliquez sur **[!UICONTROL Fermer]**.

   >[!NOTE]
   >
   >Un message peut s’afficher indiquant &quot;Gestion des pistes Marketo terminée avec un avertissement&quot;. Cela est tout à fait attendu.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. La gestion des pistes Marketo apparaît désormais sur la page **[!UICONTROL Toutes les solutions]**.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Sélectionnez la solution Marketo et cliquez sur **[!UICONTROL Publish all Customizations]**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

>[!CAUTION]
>
>La désactivation de l’un des processus de messagerie du SDK Marketo entraînera une mauvaise installation.

>[!MORELIKETHIS]
>
>[Étape 2 sur 3 : configuration de l’utilisateur de synchronisation pour Marketo (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md){target="_blank"}
