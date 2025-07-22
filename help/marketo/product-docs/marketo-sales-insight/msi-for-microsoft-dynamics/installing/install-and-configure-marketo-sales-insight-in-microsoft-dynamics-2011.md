---
unique-page-id: 3571735
description: Installer et configurer Marketo Sales Insight dans Microsoft Dynamics 2011 - Documents Marketo - Documentation du produit
title: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 3%

---

# Installation et configuration d’[!DNL Marketo Sales Insight] dans [!DNL Microsoft Dynamics 2011] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] est un outil fantastique pour votre équipe de vente. Vous trouverez ci-dessous les instructions étape par étape pour l’installer et le configurer dans [!DNL Microsoft Dynamics 2011] On-Premise.

>[!PREREQUISITES]
>
>Terminez votre intégration Marketo-Microsoft.
>
>[Téléchargez la solution appropriée](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) pour votre version de [!DNL Microsoft Dynamics] CRM.

## Importer la solution {#import-solution}

1. Connectez-vous à [!DNL Microsoft Dynamics] CRM. Cliquez sur **[!UICONTROL Paramètres]** dans le menu inférieur gauche.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Sélectionnez **[!UICONTROL Solutions]** dans l’arborescence.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Cliquez sur **Importer** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Vous devez déjà avoir [installé et configuré](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la solution Marketo avant de continuer.

1. Cliquez sur **[!UICONTROL Parcourir]**. Sélectionnez la solution [!DNL Marketo Sales Insight] que vous [téléchargé](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Vérifiez les détails de la solution, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Assurez-vous que l’option Message SDK est cochée. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Attendez maintenant la fin de l’importation.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/crmhand.png)

1. [!DNL Marketo Sales Insight] apparaît désormais dans la liste des solutions. Ouais !

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Sélectionnez [!DNL Marketo Sales Insight] et cliquez sur **Publier toutes les personnalisations** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connecter Marketo et Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous à Marketo et cliquez sur **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Dans la section **[!UICONTROL Insight des ventes]**, cliquez sur **[!UICONTROL Modifier la configuration de l’API]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiez l’**[!UICONTROL hôte Marketo]**, l’**[!UICONTROL URL de l’API]** et l’**[!UICONTROL ID d’utilisateur de l’API]** à utiliser à une étape ultérieure. Saisissez une **[!UICONTROL Clé secrète API]** de votre choix, puis cliquez sur **[!UICONTROL Enregistrer]**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Les champs suivants doivent être synchronisés avec Marketo pour _Lead et Contact_ pour que Sales Insight fonctionne :
   >
   >* Priorité
   >* Urgence
   >* Évaluation relative
   >
   >Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour résoudre ce problème, procédez [comme suit](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Revenez à Dynamics, sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Sélectionnez **[!UICONTROL Configuration de l’API Marketo]** dans l’arborescence.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Cliquez sur **[!UICONTROL Configuration par défaut]**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Saisissez les informations extraites de Marketo précédemment.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Définir l’accès utilisateur {#set-user-access}

Configurez les rôles utilisateur pour permettre à des utilisateurs spécifiques d’accéder aux [!DNL Sales Insight].

1. Sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Sélectionnez **[!UICONTROL Administration]** dans l’arborescence.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Cliquez sur **[!UICONTROL Utilisateurs]**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Sélectionnez le ou les utilisateurs auxquels vous souhaitez accorder l’accès et cliquez sur **[!UICONTROL Gérer les rôles]**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Sélectionnez le rôle **[!UICONTROL Marketo Sales Insight]** et cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Et c&#39;est tout ! Tous les utilisateurs ayant accès pourront désormais voir la section insight des ventes dans la vue des détails du prospect/contact.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Félicitations. Vous avez maintenant libéré la puissance de la [!DNL Marketo Sales Insight].

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de leads/contacts](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
