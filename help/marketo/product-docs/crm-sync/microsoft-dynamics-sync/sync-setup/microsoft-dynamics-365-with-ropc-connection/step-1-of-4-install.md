---
description: Étape 1 sur 4 - Installation de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource - Documents Marketo - Documentation du produit
title: Étape 1 sur 4 - Installation de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Étape 1 sur 4 : Installation de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire des ressources {#step-1-of-4-install-the-marketo-solution-ropc}

Avant de pouvoir synchroniser Microsoft Dynamics 365 et Marketo, vous devez installer la solution Marketo dans Dynamics. **Les autorisations d’administrateur Dynamics sont requises.**

>[!CAUTION]
>
>* N’activez pas la synchronisation des entités personnalisées avant l’exécution de la synchronisation initiale. Une fois la synchronisation initiale terminée, vous en serez informé par e-mail.
>* Si l’authentification à plusieurs facteurs (MFA) est activée pour votre synchronisation Dynamics, vous devez la désactiver pour que Dynamics se synchronise correctement avec Marketo. Pour plus d’informations, veuillez contacter [Prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>Après avoir synchronisé Marketo avec un CRM, vous ne pouvez pas effectuer de nouvelle synchronisation sans remplacer l’instance.

>[!PREREQUISITES]
>
>[Téléchargement de la solution de gestion des leads Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Connectez-vous à **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Cliquez sur ![](assets/image2015-3-16-16-3a1-3a13.png) et sélectionnez **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Cliquez sur ![](assets/image2015-5-13-10-3a5-3a8.png) . Dans le menu déroulant, sélectionnez **Paramètres** puis sélectionnez **Solutions**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Cliquez sur **Importez.**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Cliquez sur **Sélectionnez Fichier.** Sélectionnez la solution de gestion des pistes Marketo que vous souhaitez [téléchargé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Cliquez sur **Suivant**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Affichez les informations sur la solution et cliquez sur **Afficher les détails du module de solution**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Lorsque vous avez terminé de vérifier tous les détails, cliquez sur **Fermer**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Maintenant, de retour sur la page Informations sur la solution, cliquez sur **Suivant**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Assurez-vous que la case à cocher de l’option SDK est cochée. Cliquez sur **Importer**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles de votre navigateur pour terminer le processus d’installation.

1. Maintenant, attendez la fin de l’importation. Lève-toi et fais des étirements.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Cliquez sur **Fermer.**

   >[!NOTE]
   >
   >Un message peut s’afficher indiquant &quot;Gestion des pistes Marketo terminée avec un avertissement&quot;. Cela est tout à fait attendu.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. La Gestion des prospects Marketo apparaît désormais dans la liste des solutions.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Sélectionner **Gestion des leads Marketo** et cliquez sur **Publier toutes les personnalisations.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Cinq heures de haut ! L’installation est terminée.

   >[!MORELIKETHIS]
   >
   >[Étape 2 sur 4 : Configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire des ressources](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
