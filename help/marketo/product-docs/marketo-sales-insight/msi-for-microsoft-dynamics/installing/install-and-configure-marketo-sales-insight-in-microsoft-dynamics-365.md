---
unique-page-id: 3571739
description: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 365 - Marketo Docs - Documentation sur les produits
title: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 365
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Installer et configurer Marketo Sales Insight dans Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketing Sales Insight est un outil fantastique qui permet à votre équipe commerciale de découvrir la richesse des données dont dispose l’équipe marketing. Voici comment installer et configurer.

>[!PREREQUISITES]
>
>Effectuez votre intégration Marketo-Microsoft.
>
>[Téléchargez la bonne ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) solution pour votre version de Microsoft Dynamics CRM.

## Importer la solution {#import-solution}

1. Connectez-vous à [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Cliquez sur le menu ![—](assets/image2015-3-16-16-1-13.png) et sélectionnez **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Cliquez sur le menu ![—](assets/image2015-5-13-10-5-8.png). Dans la liste déroulante, sélectionnez **Paramètres**, puis **Solutions**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >[vous devez déjà avoir installé et configuré la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) avant de passer à l&#39;étape suivante.

1. Cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Dans la nouvelle fenêtre, cliquez sur **Parcourir**. Sélectionnez la solution [Marketing Sales Insight que vous avez téléchargée à l’étape 1](#msi). Cliquez sur **Suivant**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. La solution sera chargée. Vous pouvez vue le contenu du package si vous le souhaitez. Cliquez sur **Suivant**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Veillez à laisser la case **cochée** et cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. N’hésitez pas à télécharger le fichier journal. Cliquez sur **Fermer**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Super ! Vous devriez voir la solution maintenant. S&#39;il n&#39;y est pas, actualisez votre écran.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Cliquez sur **Publier toutes les personnalisations**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connecter Marketing et Sales Insight {#connect-marketo-and-sales-insight}

Lions votre instance Marketo à Sales Insight in Dynamics. Voici comment procéder :

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous à Marketo et accédez à la section **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Sous la section **Sales Insight**, cliquez sur **Modifier la configuration de l&#39;API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiez l&#39;**hôte marketing**, **URL de l&#39;API** et **ID utilisateur de l&#39;API** pour l&#39;utiliser ultérieurement. Saisissez une **clé secrète API** de votre choix et cliquez sur **Enregistrer**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Pour que Sales Insight fonctionne, les champs suivants doivent être synchronisés avec Marketo pour _à la fois prospect et contact_ :
   >
   > * Priorité
   > * Urgence
   > * Note relative

   >
   >Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour corriger ce problème, effectuez [cette procédure](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De retour dans Microsoft Dynamics, cliquez sur l&#39;icône ![](assets/image2015-5-13-15-3a49-3a19.png) en regard de Paramètres, puis sélectionnez **Configuration de l&#39;API de marketing** dans la liste déroulante.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Cliquez sur **Configuration par défaut**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Saisissez les informations que vous avez copiées précédemment à partir de Marketo.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Cliquez sur l&#39;icône ![](assets/image2015-5-13-16-3a8-3a51.png) dans le coin inférieur droit pour enregistrer les modifications.

## Définir l&#39;accès utilisateur {#set-user-access}

Vous devez accorder aux utilisateurs les autorisations nécessaires pour utiliser Sales Insight.

1. Cliquez sur le menu ![](assets/image2015-5-13-10-3a5-3a8.png). Dans le menu déroulant, sélectionnez **Paramètres**, puis **Sécurité**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Cliquez sur **Utilisateurs**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Sélectionnez le ou les utilisateurs auxquels vous souhaitez donner accès à Sales Insight et cliquez sur **Gérer les rôles**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Sélectionnez le rôle **Analyse commerciale** et cliquez sur **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Et vous devriez avoir terminé ! Enfin, pour tester, connectez-vous à Dynamics en tant qu&#39;utilisateur qui a accès à Marketo Sales Insight et regardez un prospect ou un contact.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Vous avez déverrouillé la puissance de Marketing Cloud Sales Insight pour votre équipe commerciale.

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
