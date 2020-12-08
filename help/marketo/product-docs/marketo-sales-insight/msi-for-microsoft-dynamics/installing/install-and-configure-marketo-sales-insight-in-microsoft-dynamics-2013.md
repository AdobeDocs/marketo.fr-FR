---
unique-page-id: 3571737
description: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2013 - Marketo Docs - Documentation sur les produits
title: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2013
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketing Sales Insight est un outil fantastique pour donner à votre équipe commerciale une &quot;fenêtre&quot; sur la richesse des données dont dispose l&#39;équipe marketing. Voici comment l&#39;installer et le configurer.

>[!NOTE]
>
>**Conditions préalables**
>
>Effectuez votre intégration [](http://docs.marketo.com/x/EIA2)Marketo-Microsoft.
>
>[Téléchargez la solution](http://docs.marketo.com/x/LoJo) appropriée pour votre version de Microsoft Dynamics CRM.

## Importer la solution {#import-solution}

OK, maintenant il est temps d&#39;importer la solution Marketing Sales Insight dans Microsoft Dynamics.

1. Sous **Microsoft Dynamics CRM** , cliquez sur **Paramètres**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Sous **Paramètres**, cliquez sur **Personnalisations**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Cliquez sur **Solutions**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >Vous devez déjà avoir installé et configuré Marketo avant de poursuivre.

1. Cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Dans la nouvelle fenêtre, cliquez sur **Parcourir**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Recherchez et sélectionnez la solution que vous avez téléchargée ci-dessus.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Cliquez sur **Suivant**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. La solution sera chargée. Vous pouvez vue le contenu du package si vous le souhaitez. Cliquez sur **Suivant**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Assurez-vous de laisser la case cochée et cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. N’hésitez pas à télécharger le fichier journal. Cliquez sur **Fermer**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Super ! Vous devriez voir la solution maintenant. S&#39;il n&#39;y est pas, actualisez votre écran.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connexion à Marketing et à Sales Insight {#connect-marketo-and-sales-insight}

Lions votre instance Marketo à Sales Insight in Dynamics.

>[!NOTE]
>
>Droits d’administration requis.

1. Connectez-vous à Marketing et accédez à la section **Admin** .

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Sous la section **Sales Insight** , cliquez sur **Modifier la configuration** de l&#39;API.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiez l’hôte **** marketing, l’URL **** API et l’ID **d’utilisateur** API pour l’utiliser ultérieurement. Saisissez une clé **secrète** API de votre choix et cliquez sur **ENREGISTRER**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

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

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Sous **Paramètres**, cliquez sur Configuration **de l’API** Marketo.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Cliquez sur **Nouveau**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Saisissez les informations que vous avez reçues de Marketo plus tôt et cliquez sur **Enregistrer**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Définir l&#39;accès utilisateur {#set-user-access}

Enfin, vous pouvez donner aux utilisateurs spécifiques l’accès à Marketing Cloud Sales Insight.

1. Accédez à **Paramètres**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Sélectionnez le ou les utilisateurs auxquels vous souhaitez donner accès à Sales Insight, puis cliquez sur **Gérer les rôles**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Sélectionnez le rôle **Marketo Sales Insight** et cliquez sur **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Et vous devriez avoir terminé ! Enfin, pour tester, connectez-vous à Dynamics en tant qu&#39;utilisateur qui a accès à Marketo Sales Insight et consultez un prospect ou un contact.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Vous avez déverrouillé la puissance de Marketing Cloud Sales Insight pour votre équipe commerciale.

>[!NOTE]
>
>**Articles connexes**
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](http://docs.marketo.com/x/BICMAg)

