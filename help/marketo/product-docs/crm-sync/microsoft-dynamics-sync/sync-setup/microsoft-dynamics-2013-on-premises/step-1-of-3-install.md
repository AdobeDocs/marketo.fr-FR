---
unique-page-id: 3571813
description: Étape 1 sur 3 - Installation de la solution Marketo dans Dynamics (local 2013) - Documentation sur le marché - Documentation sur le produit
title: Étape 1 sur 3 - Installation de la solution Marketo dans Dynamics (local 2013)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Étape 1 sur 3 : Installer la solution Marketo dans Dynamics (local 2013) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Avant de pouvoir synchroniser Microsoft Dynamics On-Premises et Marketo, vous devez d&#39;abord installer la solution Marketo dans Dynamics.

>[!NOTE]
>
>Une fois que vous avez synchronisé Marketo sur un service de gestion de la relation client, vous ne pouvez pas effectuer une nouvelle synchronisation sans remplacer l’instance.

>[!PREREQUISITES]
>
>Vous devez avoir un déploiement [](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) Internet Facing [(IFD) avec les services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) de fédérationPrincipale Directory 2.0, 2.1 ou 3.0 (ADFS) configurés. Remarque : Le document IFD se télécharge automatiquement lorsque vous cliquez sur le lien.
>
>[Téléchargez la solution](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) marketing avant de début.

>[!NOTE]
>
>**Autorisations d&#39;administrateur Dynamics requises.**
>
>Vous avez besoin de droits d’administrateur CRM pour effectuer cette synchronisation.

1. Connectez-vous à **Dynamics**. Cliquez sur le menu déroulant **Microsoft Dynamics CRM** et sélectionnez **PARAMÈTRES**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Sous **PARAMÈTRES**, sélectionnez **SOLUTIONS**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Cliquez sur **Importer**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Cliquez sur **Parcourir** et sélectionnez la solution [](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)téléchargée. Cliquez sur **Suivant**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Vue les Informations sur la solution et cliquez sur Détails **du package de la solution** Vue.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Lorsque vous avez terminé de vérifier tous les détails, cliquez sur **Fermer**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. De nouveau sur la page Informations sur la solution, cliquez sur **Suivant**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Assurez-vous que l’option SDK est cochée. Cliquez sur **Importer**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Attendez la fin de l’importation.

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles de votre navigateur pour terminer le processus d’installation.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Téléchargez un fichier journal (si vous le souhaitez) et cliquez sur **Fermer**.

   >[!NOTE]
   >
   >Un message indiquant &quot;Gestion des pistes marketing terminée avec un avertissement&quot; peut s’afficher. On s&#39;y attend pleinement.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. La gestion des pistes marketing s’affiche désormais sur la page **Toutes les solutions** .

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Sélectionnez la solution Marketo et cliquez sur **Publier toutes les personnalisations**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

N&#39;était-ce pas un mauvais droit ? Allez, je continuerai à vous faire traverser le reste.

>[!CAUTION]
>
>La désactivation de l’un des processus de messagerie du SDK de Marketo entraîne une panne de l’installation !

>[!NOTE]
>
>**Articles connexes**
>
>* [Étape 2 sur 3 : Configurer l&#39;utilisateur de synchronisation pour Marketo (local 2013)](step-2-of-3-configure.md)

>



