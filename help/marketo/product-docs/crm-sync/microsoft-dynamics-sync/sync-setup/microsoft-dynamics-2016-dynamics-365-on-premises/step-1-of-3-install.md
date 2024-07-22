---
description: Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise 1 sur 3 - Documents Marketo - Documentation du produit
title: Installation de Marketo pour Microsoft Dynamics 2016/Dynamics 365 On-Premise Étape 1 sur 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Étape 1 sur 3 : configuration de l’utilisateur de synchronisation pour Marketo (2016 On-Prem /Dynamics 365 On-Premise) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Avant de pouvoir synchroniser Microsoft Dynamics 2016 On-Prem/Dynamics 365 avec Marketo Engage, vous devez installer la solution Marketo dans Dynamics.

>[!NOTE]
>
>Une fois que vous avez synchronisé Marketo avec un CRM, vous ne pouvez pas synchroniser un nouveau CRM avec l’instance Marketo existante.

>[!PREREQUISITES]
>
>Si vous utilisez Microsoft Dynamics On-Premise, vous devez avoir [Déploiement Internet Face](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) avec [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0+ (ADFS) configuré. Remarque : le document IFD se télécharge automatiquement lorsque vous cliquez sur le lien.
>
>[Téléchargez la solution de gestion des pistes Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} avant de commencer.

>[!NOTE]
>
>**Autorisations d’administrateur Dynamics requises**.
>
>Pour effectuer cette synchronisation, vous avez besoin des privilèges d’administrateur CRM.

1. Connectez-vous à Dynamics. Cliquez sur le menu déroulant **[!UICONTROL Microsoft Dynamics CRM]** et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Sous **[!UICONTROL Settings]**, sélectionnez **[!UICONTROL Solutions]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Cliquez sur **[!UICONTROL Parcourir]** et sélectionnez la solution que vous avez [téléchargée](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Cliquez sur **Suivant**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Affichez les informations sur la solution et cliquez sur **[!UICONTROL Afficher les détails du package de solution]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Lorsque vous avez terminé de vérifier tous les détails, cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/step6.png)

1. De retour sur la page Informations sur la solution, cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Assurez-vous que la case à cocher de l’option SDK est cochée. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Patientez jusqu’à la fin de l’importation.

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles de votre navigateur pour terminer le processus d’installation.

   ![](assets/image2015-3-11-11-34-9.png)

1. Téléchargez un fichier journal (si vous le souhaitez) et cliquez sur **[!UICONTROL Fermer]**.

   >[!NOTE]
   >
   >Un message peut s’afficher indiquant &quot;Gestion des pistes Marketo terminée avec un avertissement&quot;. Cela est tout à fait attendu.

   ![](assets/image2015-3-13-9-54-39.png)

1. La gestion des pistes Marketo apparaît désormais sur la page **[!UICONTROL Toutes les solutions]**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Sélectionnez la solution Marketo et cliquez sur **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-3-19-8-41-21.png)

   Cinq heures de haut ! L’installation est terminée.

   >[!CAUTION]
   >
   >La désactivation de l’un des processus de messagerie du SDK Marketo entraînera une mauvaise installation.

   >[!MORELIKETHIS]
   >
   >[Installation de Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}
