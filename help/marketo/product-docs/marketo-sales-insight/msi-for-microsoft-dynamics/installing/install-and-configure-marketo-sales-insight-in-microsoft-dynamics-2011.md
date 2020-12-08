---
unique-page-id: 3571735
description: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2011 - Marketo Docs - Documentation sur les produits
title: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2011
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketing Sales Insight est un outil fantastique pour votre équipe commerciale. Voici les instructions détaillées d&#39;installation et de configuration dans Microsoft Dynamics 2011 On-Premises.

>[!NOTE]
>
>**Conditions préalables**
>
>Effectuez votre intégration [](http://docs.marketo.com/x/DoA2)Marketo-Microsoft.
>
>[Téléchargez la solution](http://docs.marketo.com/x/LoJo) appropriée pour votre version de Microsoft Dynamics CRM.

## Importer la solution {#import-solution}

1. Connectez-vous à Microsoft Dynamics CRM. Cliquez sur **Paramètres** dans le menu inférieur gauche.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Sélectionnez **Solutions** dans l’arborescence.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Cliquez sur **Importer** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >Vous devez déjà avoir [installé et configuré](install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la solution Marketo avant de passer à l’étape suivante.

1. Cliquez sur **Parcourir**. Sélectionnez la solution Marketing Cloud Sales Insight que vous avez [téléchargée](download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Cliquez sur **Suivant**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Vérifiez les détails de la solution, puis cliquez sur **Suivant**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Assurez-vous que l’option de message SDK est cochée. Cliquez sur **Suivant**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Attendez maintenant la fin de l’importation.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Cliquez sur **Fermer**.

   ![](assets/crmhand.png)

1. Les statistiques commerciales de Marketing Cloud s’affichent désormais dans la liste de solutions. Ouais !

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Sélectionnez Marketing to Sales Insight, puis cliquez sur **Publier toutes les personnalisations** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connexion à Marketing et à Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous à Marketing et cliquez sur **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Sous la section **Sales Insight **cliquez sur **Modifier la configuration** de l&#39;API.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiez l’hôte **** marketing, l’URL **** API et l’ID **d’utilisateur** API pour l’utiliser ultérieurement. Saisissez une clé **secrète** API de votre choix et cliquez sur **ENREGISTRER**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Les champs suivants doivent être synchronisés avec Marketo pour que le prospect et le contact *pour que Sales Insight fonctionnent* à la fois :
   >
   >    
   >    
   >    * Priorité
   >    * Urgence
   >    * Note relative

   >    
   >    
   >Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour corriger ce problème, effectuez [cette procédure](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Revenez à Dynamics, sélectionnez **Settings**(Paramètres).

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Sélectionnez Configuration **de l’API** Marketo dans l’arborescence.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Cliquez sur Configuration **** par défaut.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Entrez les informations que vous avez reçues de Marketo plus tôt.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Cliquez sur **Enregistrer.**

   ** ![](assets/image2015-5-4-11-3a28-3a13.png)

   **

## Définir l&#39;accès utilisateur {#set-user-access}

Configurez des rôles d&#39;utilisateur pour permettre à des utilisateurs spécifiques d&#39;accéder à Sales Insight.

1. Sélectionnez **Paramètres**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Sélectionnez **Administration** dans l’arborescence.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Sélectionnez le ou les utilisateurs auxquels vous souhaitez accorder l’accès et cliquez sur **Gérer les rôles**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Sélectionnez le rôle **Marketo Sales Insight** et cliquez sur **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Et c&#39;est tout ! Tous les utilisateurs ont accès à la section commerciale de la vue des détails de prospect/contact.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Félicitations. Vous avez maintenant libéré la puissance de Marketo Sales Insight.

>[!NOTE]
>
>**Articles connexes**
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](http://docs.marketo.com/x/BICMAg)

