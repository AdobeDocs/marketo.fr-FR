---
description: Installer Marketo for [!DNL Microsoft Dynamics] 2016/Dynamics 365 On-Premise 1 de 3 - Documents Marketo - Documentation du produit
title: Installez Marketo for [!DNL Microsoft Dynamics] 2016/Dynamics 365 On-Premise Étape 1 de 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Étape 1 de 3 : configurer l&#39;utilisateur de synchronisation pour Marketo (2016 On-Prem /Dynamics 365 On-Premise) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Avant de pouvoir synchroniser [!DNL Microsoft Dynamics] 2016 On-Prem/Dynamics 365 avec Marketo, vous devez d’abord installer la solution Marketo dans Dynamics.

>[!NOTE]
>
>Après avoir synchronisé Marketo avec un CRM, vous ne pouvez pas synchroniser un nouveau CRM avec l’instance Marketo existante.

>[!PREREQUISITES]
>
>Si vous utilisez [!DNL Microsoft Dynamics] On-Premise, vous devez avoir configuré [Déploiement par Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) avec [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS). Remarque : le document IFD est téléchargé automatiquement lorsque vous cliquez sur le lien.
>
>[Téléchargez la solution de gestion des prospects de Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} avant de commencer.

>[!NOTE]
>
>Autorisations d’administrateur **[!DNL Dynamics]requises.**
>
>Vous avez besoin de privilèges d’administrateur CRM pour effectuer cette synchronisation.

1. Connectez-vous à **[!DNL Dynamics].** Cliquez sur le menu déroulant **[!DNL Microsoft Dynamics]CRM** et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Sous **[!UICONTROL Paramètres]**, sélectionnez **[!UICONTROL Solutions]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Cliquez sur **[!UICONTROL Parcourir]** et sélectionnez la solution que vous [téléchargée](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Affichez les informations sur la solution et cliquez sur **[!UICONTROL Afficher les détails du package de solution]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Une fois la vérification de tous les détails terminée, cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/step6.png)

1. De retour sur la page Informations sur la solution, cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Assurez-vous que la case option SDK est cochée. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Attendez la fin de l’importation.

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles sur votre navigateur pour terminer le processus d’installation.

   ![](assets/image2015-3-11-11-34-9.png)

1. Téléchargez un fichier journal (si vous le souhaitez) et cliquez sur **[!UICONTROL Fermer]**.

   >[!NOTE]
   >
   >Il se peut qu’un message indiquant « Marketo Lead Management terminé avec un avertissement » s’affiche. Cela est tout à fait prévu.

   ![](assets/image2015-3-13-9-54-39.png)

1. La gestion des prospects Marketo apparaît désormais sur la page **[!UICONTROL Toutes les solutions]**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Sélectionnez la solution Marketo et cliquez sur **[!UICONTROL Publier toutes les personnalisations]**.

   ![](assets/image2015-3-19-8-41-21.png)

   Cinq ans ! L&#39;installation est terminée.

   >[!CAUTION]
   >
   >La désactivation de l’un des processus de messagerie SDK de Marketo entraînera une installation interrompue.

   >[!MORELIKETHIS]
   >
   >[Installation de Marketo for [!DNL Dynamics] 2015 On-Prem et 2016 365 On-Prem Étape 2 sur 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
