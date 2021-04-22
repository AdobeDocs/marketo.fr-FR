---
unique-page-id: 3571822
description: Étape 1 sur 3 - Installation de la solution Marketo (en ligne) - Documents Marketo - Documentation du produit
title: Étape 1 sur 3 - Installation de la solution Marketo (en ligne)
exl-id: 593fc014-db38-42cc-8f9f-0dd8307751e8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Étape 1 sur 3 : Installer la solution Marketo (en ligne) {#step-of-install-the-marketo-solution-online}

Avant de pouvoir synchroniser Microsoft Dynamics 365 et Marketo, vous devez d&#39;abord installer la solution Marketo dans Dynamics. **Les autorisations d&#39;administrateur Dynamics sont requises.**

>[!CAUTION]
>
>* N&#39;activez pas la synchronisation d&#39;entité personnalisée avant la synchronisation initiale. Une fois la synchronisation initiale terminée, vous en serez averti par courrier électronique.
>* Si l&#39;authentification multifacteur (MFA) est activée pour Dynamics Sync, vous devez la désactiver pour que Dynamics se synchronise correctement avec Marketo. Pour de plus amples informations, veuillez contacter le [Support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).


>[!NOTE]
>
>Après avoir synchronisé Marketo avec un service de gestion de la relation client, vous ne pouvez pas effectuer une nouvelle synchronisation sans remplacer l’instance.

>[!PREREQUISITES]
>
>[Téléchargement de la solution Marketo Lead Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Connectez-vous à **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Cliquez sur le menu ![](assets/image2015-3-16-16-3a1-3a13.png) et sélectionnez **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Cliquez sur le menu ![](assets/image2015-5-13-10-3a5-3a8.png). Dans le menu déroulant, sélectionnez **Paramètres**, puis **Solutions**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Cliquez sur **Importer.**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Cliquez sur **Choisir un fichier.** Sélectionnez la solution de gestion des pistes Marketo que vous avez  [téléchargée](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Cliquez sur **Suivant**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Vue les informations de solution et cliquez sur **détails du package de la solution de Vue**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Lorsque vous avez terminé de vérifier tous les détails, cliquez sur **Fermer**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Désormais, de nouveau dans la page Informations sur la solution, cliquez sur **Suivant**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Assurez-vous que la case à cocher de l’option SDK est activée. Cliquez sur **Importer**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Vous devez activer les fenêtres contextuelles de votre navigateur pour terminer le processus d’installation.

1. Attendez maintenant la fin de l’importation. Levez-vous et faites des étirements.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Cliquez sur **Fermer.**

   >[!NOTE]
   >
   >Un message peut s’afficher indiquant que la gestion des pistes Marketo s’est terminée avec un avertissement. On s&#39;y attend pleinement.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. La gestion des pistes de Marketo apparaît désormais dans la liste des solutions.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Sélectionnez **Gestion des pistes Marketo** et cliquez sur **Publier toutes les personnalisations.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Cinq ! L&#39;installation est terminée.

   >[!MORELIKETHIS]
   >
   >[Étape 2 sur 3 : Configurer l&#39;utilisateur Marketo Sync dans Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)
