---
unique-page-id: 37355602
description: Installer et configurer Marketo Sales Insight dans Microsoft Dynamics Online - Marketo Docs - Documentation sur les produits
title: Installer et configurer Marketo Sales Insight dans Microsoft Dynamics Online
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Installer et configurer Marketo Sales Insight dans Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketing Sales Insight est un outil fantastique qui permet à votre équipe commerciale de découvrir la richesse des données dont dispose l’équipe marketing. Voici comment l&#39;installer et le configurer dans Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Effectuez votre intégration [](http://docs.marketo.com/x/E4A2)Marketo-Microsoft.
>
>[Téléchargez la solution](http://docs.marketo.com/x/LoJo) appropriée pour votre version de Microsoft Dynamics CRM.

## Importer la solution {#import-solution}

>[!NOTE]
>
>Si vous utilisez l’interface unifiée, avant l’étape 1 ci-dessous, cliquez sur l’icône Paramètres dans le coin supérieur droit et sélectionnez Paramètres **** avancés.

1. Sous Microsoft Dynamics CRM, cliquez sur **Paramètres**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Sous PARAMÈTRES, cliquez sur **Personnalisations**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Cliquez sur **Solutions**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >Vous devez déjà avoir installé et configuré la solution Marketo avant de poursuivre.

1. Cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Dans la nouvelle fenêtre, cliquez sur **Parcourir**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Sur votre ordinateur, recherchez et installez la solution que vous venez de télécharger.
1. Cliquez sur **Suivant**.

   ![](assets/seven.png)

1. La solution sera chargée. Vous pouvez vue le contenu du package si vous le souhaitez. Cliquez sur **Suivant**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Assurez-vous de laisser la case cochée et cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. N’hésitez pas à télécharger le fichier journal, puis cliquez sur **Fermer**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Super ! Vous devriez voir la solution maintenant. S&#39;il n&#39;y est pas, actualisez votre écran.

   ![](assets/eleven.png)

1. Cliquez sur **Publier la personnalisation**.

   >[!NOTE]
   >
   >Veillez à activer la synchronisation MS Dynamics globale.

## Connexion à Marketing et à Sales Insight {#connect-marketo-and-sales-insight}

Lions votre instance Marketo à Sales Insight in Dynamics. Voici comment :

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous au marketing et accédez à la **section Admin **section.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Sous la section Sales Insight, cliquez sur **Modifier la configuration** de l&#39;API.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copiez l’hôte **** marketing, l’URL **** API et l’ID **d’utilisateur** API pour l’utiliser ultérieurement. Saisissez une clé secrète API de votre choix et cliquez sur **Enregistrer**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

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

1. De retour dans Microsoft Dynamics, accédez à **Paramètres**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Sous **Paramètres**, cliquez sur Configuration **de l’API** Marketo.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Cliquez sur **Nouveau**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Saisissez les informations que vous avez reçues de Marketo plus tôt et cliquez sur **Enregistrer**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Activer la synchronisation {#enable-sync}

1. Dans Marketing, cliquez sur **Admin**.

   ![](assets/enable-one.png)

1. Sous Intégration, sélectionnez **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Cliquez sur **Activer la synchronisation**.

   ![](assets/enable-three.png)

1. Cliquez sur **Modifier** en regard de Détails de synchronisation des champs.

   ![](assets/enable-four.png)

1. Cela permet de sélectionner *automatiquement* les champs MSI précédemment désactivés (Urgence, Score relatif et Priorité). Il vous suffit de cliquer sur **Enregistrer** pour début des données de synchronisation.

   ![](assets/enable-five.png)

## Définir l&#39;accès utilisateur {#set-user-access}

Enfin, vous devez donner aux utilisateurs spécifiques l&#39;accès à l&#39;utilisation de Marketing Cloud Sales Insight.

1. Accédez à **Paramètres**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Accédez à **Sécurité**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Sélectionnez les utilisateurs auxquels vous souhaitez donner accès à Sales Insight, puis cliquez sur **Gérer les rôles**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Sélectionnez le rôle Sales Insight du marketing et cliquez sur **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   Et vous devriez avoir terminé ! Enfin, pour tester, connectez-vous à Dynamics en tant qu&#39;utilisateur qui a accès à Marketo Sales Insight et regardez un prospect ou un contact.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!NOTE]
>
>**Articles connexes**
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](http://docs.marketo.com/x/BICMAg)

