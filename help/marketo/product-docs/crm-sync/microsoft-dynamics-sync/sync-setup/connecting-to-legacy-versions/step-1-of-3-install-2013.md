---
unique-page-id: 3571813
description: Étape 1 sur 3 - Installation de la solution Marketo dans Dynamics (On-Premise 2013) - Documents Marketo - Documentation du produit
title: Étape 1 sur 3 - Installation de la solution Marketo dans Dynamics (On-Premise 2013)
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
source-git-commit: 64c5f03bd2320bfbffd257684d1482e995def83a
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Étape 1 sur 3 : Installation de la solution Marketo dans Dynamics (2013 On-Premise) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Avant de pouvoir synchroniser Microsoft Dynamics On-Premise et Marketo, vous devez installer la solution Marketo dans Dynamics.

>[!NOTE]
>
>Après avoir synchronisé Marketo avec un CRM, vous ne pouvez pas effectuer de nouvelle synchronisation sans remplacer l’instance.

>[!PREREQUISITES]
>
>Vous devez avoir [Déploiement Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) avec [Services de fédération principale Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 ou 3.0 (ADFS) configurés. Remarque : Le document IFD se télécharge automatiquement lorsque vous cliquez sur le lien.
>
>[Téléchargement de la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) avant de commencer.

>[!NOTE]
>
>**Autorisations d’administrateur Dynamics requises.**
>
>Pour effectuer cette synchronisation, vous avez besoin des privilèges d’administrateur CRM.

1. Se connecter **Dynamics**. Cliquez sur le bouton **Microsoft Dynamics CRM** menu déroulant, puis sélectionnez **Paramètres**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Sous **Paramètres**, sélectionnez **Solutions**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Cliquez sur **Importer**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Cliquez sur **Parcourir** et sélectionnez la variable [solution téléchargée](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Cliquez sur **Suivant**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Affichez les informations sur la solution et cliquez sur **Afficher les détails du module de solution**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Lorsque vous avez terminé de vérifier tous les détails, cliquez sur **Fermer**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. De retour sur la page Informations sur la solution, cliquez sur **Suivant**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Assurez-vous que l’option SDK est cochée. Cliquez sur **Importer**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Attendez que l’importation se termine.

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles de votre navigateur pour terminer le processus d’installation.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Téléchargez un fichier journal (le cas échéant) et cliquez sur **Fermer**.

   >[!NOTE]
   >
   >Un message peut s’afficher indiquant &quot;Gestion des pistes Marketo terminée avec un avertissement&quot;. Cela est tout à fait attendu.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. La Gestion des leads Marketo apparaîtra désormais sur la page **Toutes les solutions** page.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Sélectionnez la solution Marketo et cliquez sur **Publier toutes les personnalisations**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

N&#39;était-ce pas vraiment mal ? Allez, je vais continuer à vous promener à travers le reste.

>[!CAUTION]
>
>La désactivation de l’un des processus de messagerie du SDK Marketo entraînera une mauvaise installation.

>[!MORELIKETHIS]
>
>[Étape 2 sur 3 : Configuration de l’utilisateur de synchronisation pour Marketo (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)
