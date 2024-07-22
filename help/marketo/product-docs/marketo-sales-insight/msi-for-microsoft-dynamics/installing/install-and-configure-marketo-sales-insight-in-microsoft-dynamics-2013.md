---
unique-page-id: 3571737
description: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2013 - Documentation Marketo - Documentation du produit
title: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 1%

---

# Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight est un outil fantastique pour offrir à votre équipe de vente une &quot;fenêtre&quot; sur la richesse des données de l’équipe marketing. Voici comment l’installer et le configurer.

>[!PREREQUISITES]
>
>Terminez votre intégration Marketo-Microsoft.
>
>[Téléchargez la solution correcte](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) pour votre version de Microsoft Dynamics CRM.

## Importer la solution {#import-solution}

OK, il est maintenant temps d’importer la solution Marketo Sales Insight dans Microsoft Dynamics.

1. Sous **Microsoft Dynamics CRM**, cliquez sur **Paramètres**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Sous **Paramètres**, cliquez sur **Personnalisations**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Cliquez sur **Solutions**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
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

1. La solution sera chargée. Vous pouvez afficher le contenu du module si vous le souhaitez. Cliquez sur **Suivant**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Veillez à laisser la case cochée et cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. N’hésitez pas à télécharger le fichier journal. Cliquez sur **Fermer**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Super ! Vous devriez voir la solution maintenant. Si ce n’est pas le cas, actualisez votre écran.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connexion de Marketo et de Sales Insight {#connect-marketo-and-sales-insight}

Lions votre instance Marketo à Sales Insight dans Dynamics.

>[!NOTE]
>
>Droits d’administrateur requis.

1. Connectez-vous à Marketo et accédez à la section **Admin** .

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Sous la section **Sales Insight** , cliquez sur **Modifier la configuration de l’API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiez l’ **hôte Marketo**, l’ **URL de l’API** et l’ **ID de l’utilisateur de l’API** pour l’utiliser ultérieurement. Saisissez une **clé secrète API** de votre choix et cliquez sur **Enregistrer**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Les champs suivants doivent être synchronisés avec Marketo pour _Lead et Contact_ afin que Sales Insight fonctionne :
   >
   >* Priorité
   >* Urgence
   >* Évaluation relative
   >
   >Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour résoudre ce problème, effectuez [cette procédure](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De retour dans Microsoft Dynamics, accédez à **Paramètres**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Sous **Settings**, cliquez sur **Marketo API Config**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Cliquez sur **New**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Saisissez les informations que vous avez précédemment récupérées de Marketo et cliquez sur **Enregistrer**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Définition de l’accès utilisateur {#set-user-access}

Enfin, vous pouvez donner à des utilisateurs spécifiques un accès à Marketo Sales Insight.

1. Accédez à **Paramètres**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Cliquez sur **Users**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Sélectionnez le ou les utilisateurs auxquels vous souhaitez donner accès à Sales Insight et cliquez sur **Gérer les rôles**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Sélectionnez le rôle **Marketo Sales Insight** et cliquez sur **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Et tout devrait être fait ! Enfin, pour tester, connectez-vous à Dynamics en tant qu’utilisateur ayant accès à Marketo Sales Insight et consultez un prospect ou un contact.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Vous avez désormais déverrouillé la puissance de Marketo Sales Insight pour votre équipe commerciale.

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
