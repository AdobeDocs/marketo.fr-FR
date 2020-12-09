---
unique-page-id: 7504736
description: Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 1 sur 3 - Marketo Docs - Documentation du produit
title: Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 1 sur 3
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Étape 1 sur 3

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 1 of 3-->

Avant de pouvoir synchroniser Microsoft Dynamics 2015 On-Premises ou 2016 (Dynamics 365) avec Marketo, vous devez d&#39;abord installer la solution Marketo dans Dynamics.

>[!NOTE]
>
>Une fois que vous avez synchronisé Marketo sur un service de gestion de la relation client, vous ne pouvez plus synchroniser un nouveau service de gestion de la relation client sur l’instance de marché existante.

>[!PREREQUISITES]
>
>Si vous utilisez Microsoft Dynamics On-Premise, vous devez avoir un déploiement [](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) Internet Facing (IFD) avec les services [de fédération](https://msdn.microsoft.com/en-us/library/bb897402.aspx) Principale Directory 2.0+ (ADFS) configurés. Remarque : Le document IFD se télécharge automatiquement lorsque vous cliquez sur le lien.
>
>[Téléchargez la solution](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) de gestion des pistes marketing avant de début.

>[!NOTE]
>
>**Autorisations d&#39;administrateur Dynamics requises.**
>
>Vous avez besoin de droits d’administrateur CRM pour effectuer cette synchronisation.

1. Connectez-vous à **Dynamics.** Cliquez sur le menu déroulant **Microsoft Dynamics CRM** et sélectionnez **Paramètres**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Sous **Paramètres**, sélectionnez **Solutions**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Cliquez sur **Importer**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Cliquez sur **Parcourir** et sélectionnez la solution que vous avez [téléchargée](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Cliquez sur **Suivant**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Vue les Informations sur la solution et cliquez sur Détails **du package de la solution** Vue.

   ![](assets/image2015-11-18-11-12-8.png)

1. Lorsque vous avez terminé de vérifier tous les détails, cliquez sur **Fermer**.

   ![](assets/step6.png)

1. De nouveau sur la page Informations sur la solution, cliquez sur **Suivant**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Assurez-vous que la case à cocher de l’option SDK est activée. Cliquez sur **Importer**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Attendez la fin de l’importation.

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles de votre navigateur pour terminer le processus d’installation.

   ![](assets/image2015-3-11-11-34-9.png)

1. Téléchargez un fichier journal (si vous le souhaitez) et cliquez sur **Fermer**.

   >[!NOTE]
   >
   >Un message indiquant &quot;Gestion des pistes marketing terminée avec un avertissement&quot; peut s’afficher. On s&#39;y attend pleinement.

   ![](assets/image2015-3-13-9-54-39.png)

1. La gestion des pistes marketing s’affiche désormais sur la page **Toutes les solutions** .

   ![](assets/image2015-3-19-8-40-38.png)

1. Sélectionnez la solution Marketo et cliquez sur **Publier toutes les personnalisations**.

   ![](assets/image2015-3-19-8-41-21.png)

   Cinq ! L&#39;installation est terminée.

   >[!CAUTION]
   >
   >La désactivation de l’un des processus de messagerie du SDK de Marketo entraîne une panne de l’installation !

   >[!NOTE]
   >
   >**Articles connexes**
   >
   >
   >[Installer Marketo pour Dynamics 2015 On-Prem et 2016 365 On-Prem Étape 2 sur 3](step-2-of-3-set-up.md)
