---
unique-page-id: 37355602
description: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics Online - Documents Marketo - Documentation du produit
title: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 1%

---

# Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight est un outil fantastique pour offrir à votre équipe de vente une &quot;fenêtre&quot; sur la richesse des données de l’équipe marketing. Voici comment l’installer et le configurer dans Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Terminez votre intégration Marketo-Microsoft.
>
>[Télécharger la solution appropriée](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) pour votre version de Microsoft Dynamics CRM.

## Importer la solution {#import-solution}

>[!NOTE]
>
>Si vous utilisez l’interface unifiée, avant l’étape 1 ci-dessous, cliquez sur l’icône Paramètres dans le coin supérieur droit et sélectionnez **Paramètres avancés**.

1. Sous Microsoft Dynamics CRM , cliquez sur **Paramètres**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Sous Paramètres, cliquez sur **Personnalisations**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Cliquez sur **Solutions**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Vous devez déjà avoir installé et configuré la solution Marketo avant de poursuivre.

1. Cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Dans la nouvelle fenêtre, cliquez sur **Parcourir**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Sur votre ordinateur, recherchez et installez la solution que vous venez de télécharger.

1. Cliquez sur **Suivant**.

   ![](assets/seven.png)

1. La solution sera chargée. Vous pouvez afficher le contenu du module si vous le souhaitez. Cliquez sur **Suivant**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Laissez la case cochée et cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. N’hésitez pas à télécharger le fichier journal, puis à cliquer sur **Fermer**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Super ! Vous devriez voir la solution maintenant. Si ce n’est pas le cas, actualisez votre écran.

   ![](assets/eleven.png)

1. Cliquez sur **Personnalisation de la publication**.

   >[!NOTE]
   >
   >Veillez à activer la synchronisation MS Dynamics globale.

## Connexion de Marketo et de Sales Insight {#connect-marketo-and-sales-insight}

Lions votre instance Marketo à Sales Insight dans Dynamics. Voici comment :

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous à Marketo et accédez au **Administration** .

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Sous la section Statistiques sur les ventes , cliquez sur **Modifier la configuration de l’API**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copiez le **Hôte Marketo**, **URL de l’API**, et **Identifiant utilisateur de l’API** à utiliser ultérieurement. Saisissez une clé secrète API de votre choix, puis cliquez sur **Enregistrer**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Les champs suivants doivent être synchronisés avec Marketo pour _prospect et contact_ pour que Sales Insight fonctionne :
   >
   >* Priorité
   >* Urgence
   >* Évaluation relative
   >
   >Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour corriger ce problème, effectuez les opérations suivantes : [cette procédure](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De retour dans Microsoft Dynamics, accédez à **Paramètres**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Sous **Paramètres**, cliquez sur **Configuration de l’API Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Cliquez sur **Nouveau**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Saisissez les informations que vous avez précédemment récupérées dans Marketo et cliquez sur **Enregistrer**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Activer la synchronisation {#enable-sync}

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/enable-one.png)

1. Sous Intégration, sélectionnez **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Cliquez sur **Activer la synchronisation**.

   ![](assets/enable-three.png)

1. Cliquez sur **Modifier** en regard de Détails de synchronisation des champs.

   ![](assets/enable-four.png)

1. Cette opération _automatiquement_ Sélectionnez les champs MSI précédemment désactivés (Urgence, Score relatif et Priorité). Cliquez simplement sur **Enregistrer** pour commencer la synchronisation des données.

   ![](assets/enable-five.png)

## Définition de l’accès utilisateur {#set-user-access}

Enfin, vous devez accorder aux utilisateurs spécifiques l’accès pour utiliser Marketo Sales Insight.

1. Accédez à **Paramètres**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Accédez à **Sécurité**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Sélectionnez les utilisateurs auxquels vous souhaitez accorder l’accès à Sales Insight , puis cliquez sur **Gestion des rôles**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Sélectionnez le rôle Marketo Sales Insight , puis cliquez sur **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   Et tout devrait être fait ! Enfin, pour tester, connectez-vous à Dynamics en tant qu’utilisateur ayant accès à Marketo Sales Insight et examinez un prospect ou un contact.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
