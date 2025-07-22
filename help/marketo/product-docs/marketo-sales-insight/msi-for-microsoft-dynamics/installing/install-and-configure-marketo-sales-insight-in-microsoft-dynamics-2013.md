---
unique-page-id: 3571737
description: Installer et configurer Marketo Sales Insight dans Microsoft Dynamics 2013 - Documents Marketo - Documentation du produit
title: Installation et configuration de Marketo Sales Insight dans Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 2%

---

# Installation et configuration d’[!DNL Marketo Sales Insight] dans [!DNL Microsoft Dynamics 2013] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] est un outil fantastique pour donner à votre équipe de vente une « fenêtre » sur la richesse des données dont dispose l’équipe marketing. Voici comment l’installer et le configurer.

>[!PREREQUISITES]
>
>Terminez votre intégration Marketo-Microsoft.
>
>[Téléchargez la solution appropriée](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) pour votre version de [!DNL Microsoft Dynamics] CRM.

## Importer la solution {#import-solution}

OK, maintenant il est temps d&#39;importer la solution [!DNL Marketo Sales Insight] dans [!DNL Microsoft Dynamics].

1. Sous **[!UICONTROL Microsoft Dynamics CRM]** cliquez sur **[!UICONTROL Paramètres]**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Sous **[!UICONTROL Paramètres]**, cliquez sur **[!UICONTROL Personnalisations]**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Cliquez sur **[!UICONTROL Solutions]**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Vous devez déjà avoir installé et configuré Marketo avant de continuer

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Dans la nouvelle fenêtre, cliquez sur **[!UICONTROL Parcourir]**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Recherchez et sélectionnez la solution que vous avez téléchargée ci-dessus.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. La solution sera chargée. Vous pouvez afficher le contenu du package si vous le souhaitez. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Veillez à laisser la case cochée et à cliquer sur **[!UICONTROL Importer]**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. N’hésitez pas à télécharger le fichier journal. Cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Génial ! Vous devriez voir la solution maintenant. S&#39;il n&#39;y en a pas, rafraîchissez votre écran.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connecter Marketo et Sales Insight {#connect-marketo-and-sales-insight}

Lions votre instance Marketo à [!DNL Sales Insight] dans [!DNL Dynamics].

>[!NOTE]
>
>Droits d’administrateur requis.

1. Connectez-vous à Marketo et accédez à la section **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Dans la section **[!UICONTROL Insight des ventes]**, cliquez sur **[!UICONTROL Modifier la configuration de l’API]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiez l’**[!UICONTROL hôte Marketo]**, l’**[!UICONTROL URL de l’API]** et l’**[!UICONTROL ID d’utilisateur de l’API]** à utiliser à une étape ultérieure. Saisissez une **[!UICONTROL Clé secrète API]** de votre choix, puis cliquez sur **[!UICONTROL Enregistrer]**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Les champs suivants doivent être synchronisés avec Marketo pour _Lead et Contact_ pour que Sales Insight fonctionne :
   >
   >* Priorité
   >* Urgence
   >* Évaluation relative
   >
   >Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour résoudre ce problème, procédez [comme suit](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De retour dans [!DNL Microsoft Dynamics], accédez à **[!UICONTROL Paramètres]**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Sous **[!UICONTROL Paramètres]**, cliquez sur **[!UICONTROL Configuration API Marketo]**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Cliquez sur **[!UICONTROL Nouveau]**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Saisissez les informations extraites de Marketo précédemment et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Définir l’accès utilisateur {#set-user-access}

Enfin, vous pouvez donner à des utilisateurs et utilisatrices spécifiques l’accès à [!DNL Marketo Sales Insight].

1. Accédez à **[!UICONTROL Paramètres]**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Cliquez sur **[!UICONTROL Utilisateurs]**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Sélectionnez le ou les utilisateurs auxquels vous souhaitez accorder l’accès à Sales Insight et cliquez sur **[!UICONTROL Gérer les rôles]**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Sélectionnez le rôle **[!UICONTROL Marketo Sales Insight]** et cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   Et vous devriez en avoir fini ! Enfin, pour effectuer un test, connectez-vous à [!DNL Dynamics] en tant qu’utilisateur ayant accès à [!DNL Marketo Sales Insight] et recherchez un prospect ou un contact.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Vous avez maintenant libéré la puissance de [!DNL Marketo Sales Insight] pour votre équipe de vente.

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de leads/contacts](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
