---
unique-page-id: 3571735
description: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2011 - Documentation Marketo - Documentation du produit
title: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight est un outil fantastique pour votre équipe commerciale. Voici les instructions étape par étape de l’installation et de la configuration dans Microsoft Dynamics 2011 On-Premise.

>[!PREREQUISITES]
>
>Terminez votre intégration Marketo-Microsoft.
>
>[Télécharger la solution appropriée](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) pour votre version de Microsoft Dynamics CRM.

## Importer la solution {#import-solution}

1. Connectez-vous à Microsoft Dynamics CRM. Cliquez sur **Paramètres** dans le menu inférieur gauche.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Sélectionner **Solutions** dans l&#39;arbre.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Cliquez sur **Importer** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Vous devriez déjà avoir [installé et configuré](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la solution Marketo avant de passer à l’étape suivante.

1. Cliquez sur **Parcourir**. Sélectionnez la solution Marketo Sales Insight [téléchargé](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Cliquez sur **Suivant**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Vérifiez les détails de la solution, puis cliquez sur **Suivant**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Assurez-vous que l’option Message du SDK est cochée. Cliquez sur **Suivant**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Maintenant, attendez la fin de l’importation.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Cliquez sur **Fermer**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight apparaît désormais dans la liste des solutions. Oui !

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Sélectionnez Marketo Sales Insight , puis cliquez sur **Publier toutes les personnalisations** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connexion de Marketo et de Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous à Marketo et cliquez sur **Administration**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Sous , **Statistiques des ventes** clic sur la section **Modifier la configuration de l’API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiez le **Hôte Marketo**, **URL de l’API**, et **Identifiant utilisateur de l’API** à utiliser ultérieurement. Saisissez un **Clé secrète API** de votre choix et cliquez sur **Enregistrer**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Les champs suivants doivent être synchronisés avec Marketo pour _prospect et contact_ pour que Sales Insight fonctionne :
   >
   >* Priorité
   >* Urgence
   >* Évaluation relative
   >
   >Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour corriger ce problème, effectuez les opérations suivantes : [cette procédure](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Revenez à Dynamics, sélectionnez **Paramètres**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Sélectionner **Configuration de l’API Marketo** dans l&#39;arbre.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Cliquez sur **Configuration par défaut**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Saisissez les informations que vous avez précédemment saisies dans Marketo.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Définition de l’accès utilisateur {#set-user-access}

Configurez les rôles utilisateur pour donner aux utilisateurs spécifiques un accès à Sales Insight.

1. Sélectionner **Paramètres**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Sélectionner **Administration** dans l&#39;arbre.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Sélectionnez le ou les utilisateurs auxquels vous souhaitez accorder l’accès, puis cliquez sur **Gestion des rôles**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Sélectionnez la **Marketo Sales Insight** rôle et clic **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Et voilà ! Tous les utilisateurs ayant accès à pourront désormais afficher la section des statistiques sur les ventes dans la vue des détails de prospect/contact.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Félicitations. Vous avez désormais libéré la puissance de Marketo Sales Insight.

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
