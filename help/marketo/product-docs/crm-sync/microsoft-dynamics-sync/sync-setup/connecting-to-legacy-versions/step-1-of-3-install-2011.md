---
unique-page-id: 3571805
description: Étape 1 sur 3 - Installation de la solution Marketo (2011 sur site) - Documents Marketo - Documentation du produit
title: Étape 1 sur 3 - Installation de la solution Marketo (2011 sur site)
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Étape 1 sur 3 : installation de la solution Marketo (2011 sur site) {#step-of-install-the-marketo-solution-on-premises}

Avant de pouvoir synchroniser Microsoft Dynamics On-Premise et Marketo Engage, vous devez installer la solution Marketo dans Dynamics.

>[!NOTE]
>
>Une fois que vous avez synchronisé Marketo avec un CRM, vous ne pouvez pas effectuer une nouvelle synchronisation sans remplacer l’instance.

>[!PREREQUISITES]
>
>Vous devez avoir [Déploiement Internet Face](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) avec [ Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 ou 3.0 (ADFS) configuré. **Remarque** : le document IFD se télécharge automatiquement lorsque vous cliquez sur le lien.
>
>[Téléchargez la solution de gestion des pistes Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} avant de commencer.

>[!NOTE]
>
>**Autorisations d’administrateur Dynamics requises**.
>
>Pour effectuer cette synchronisation, vous avez besoin des privilèges d’administrateur CRM.

1. Connectez-vous à Dynamics et sélectionnez **[!UICONTROL Paramètres]** dans le menu inférieur gauche.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Sélectionnez **[!UICONTROL Solutions]** dans l’arborescence.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Cliquez sur **[!UICONTROL Parcourir]**. Sélectionnez la solution Marketo Lead Management que vous avez [ téléchargée ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Affichez les informations sur la solution et cliquez sur **[!UICONTROL Afficher les détails du package de solution]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Lorsque vous avez terminé de vérifier tous les détails, cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. De retour sur la page Informations sur la solution, cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Assurez-vous que la case Option de message du SDK est cochée. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles de votre navigateur pour terminer le processus d’installation.

1. Maintenant, attendez la fin de l’importation. Lève-toi et fais des étirements.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Cliquez sur **[!UICONTROL Fermer]**.

   >[!NOTE]
   >
   >Un message peut s’afficher indiquant &quot;Gestion des pistes Marketo terminée avec un avertissement&quot;. Cela est tout à fait attendu.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. La gestion des pistes Marketo apparaît désormais sur la page **Toutes les solutions**.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Sélectionnez Gestion des pistes Marketo et cliquez sur **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>La désactivation de l’un des processus de messagerie du SDK Marketo entraînera une mauvaise installation.

>[!MORELIKETHIS]
>
>[Étape 2 sur 3 : configuration de l’utilisateur de synchronisation Marketo dans Dynamics (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}
