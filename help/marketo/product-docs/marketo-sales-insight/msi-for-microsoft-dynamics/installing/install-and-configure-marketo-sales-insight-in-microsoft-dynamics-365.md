---
unique-page-id: 3571739
description: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 365 - Documents Marketo - Documentation du produit
title: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 365
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 1%

---

# Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight est un outil fantastique pour offrir à votre équipe de vente une &quot;fenêtre&quot; sur la richesse des données de l’équipe marketing. Voici comment installer et configurer.

>[!PREREQUISITES]
>
>Terminez votre intégration Marketo-Microsoft.
>
>[Téléchargez la solution correcte](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) pour votre version de Microsoft Dynamics CRM.

## Importer la solution {#import-solution}

1. Connectez-vous à [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Cliquez sur le menu ![—](assets/image2015-3-16-16-1-13.png) et sélectionnez **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Cliquez sur le menu ![—](assets/image2015-5-13-10-5-8.png) . Dans la liste déroulante, sélectionnez **Paramètres**, puis **Solutions**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >[ doit déjà être installé et configuré pour la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) avant de passer à l’étape suivante.

1. Cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Dans la nouvelle fenêtre, cliquez sur **Parcourir**. Sélectionnez la [solution Marketo Sales Insight que vous avez téléchargée à l’étape 1](#msi). Cliquez sur **Suivant**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. La solution sera chargée. Vous pouvez afficher le contenu du module si vous le souhaitez. Cliquez sur **Suivant**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Veillez à laisser la case **cochée** et cliquez sur **Importer**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. N’hésitez pas à télécharger le fichier journal. Cliquez sur **Fermer**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Super ! Vous devriez voir la solution maintenant. Si ce n’est pas le cas, actualisez votre écran.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Cliquez sur **Publish Toutes les personnalisations**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connexion de Marketo et de Sales Insight {#connect-marketo-and-sales-insight}

Lions votre instance Marketo à Sales Insight dans Dynamics. Voici comment :

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous à Marketo et accédez à la section **Admin** .

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Dans la section **Sales Insight** , cliquez sur **Edit API Configuration**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiez l’ **hôte Marketo**, l’ **URL de l’API** et l’ **ID de l’utilisateur de l’API** à utiliser à une étape ultérieure. Saisissez une **clé secrète API** de votre choix et cliquez sur **Enregistrer**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Les champs suivants doivent être synchronisés avec Marketo pour _Lead et Contact_ afin que Sales Insight fonctionne :
   >
   > * Priorité
   > * Urgence
   > * Évaluation relative
   >
   >Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour résoudre ce problème, effectuez [cette procédure](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De retour dans Microsoft Dynamics, cliquez sur l’icône ![](assets/image2015-5-13-15-3a49-3a19.png) en regard de Paramètres, puis sélectionnez **Marketo API Config** dans la liste déroulante.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Cliquez sur **Configuration par défaut**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Saisissez les informations que vous avez copiées à partir de Marketo précédemment.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Cliquez sur l’icône ![](assets/image2015-5-13-16-3a8-3a51.png) dans le coin inférieur droit pour enregistrer les modifications.

## Définition de l’accès utilisateur {#set-user-access}

Vous devez accorder aux utilisateurs les autorisations nécessaires pour utiliser Sales Insight.

1. Cliquez sur le menu ![](assets/image2015-5-13-10-3a5-3a8.png) . Dans le menu déroulant, sélectionnez **Paramètres**, puis **Sécurité**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Cliquez sur **Users**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Sélectionnez le ou les utilisateurs auxquels vous souhaitez donner accès à Sales Insight et cliquez sur **Gérer les rôles**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Sélectionnez le rôle **Marketo Sales Insight** et cliquez sur **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Et tout devrait être fait ! Enfin, pour tester, connectez-vous à Dynamics en tant qu’utilisateur ayant accès à Marketo Sales Insight et examinez un prospect ou un contact.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Vous avez désormais déverrouillé la puissance de Marketo Sales Insight pour votre équipe commerciale.

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
