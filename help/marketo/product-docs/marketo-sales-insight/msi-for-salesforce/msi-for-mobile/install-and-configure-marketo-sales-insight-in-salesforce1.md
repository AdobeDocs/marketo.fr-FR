---
unique-page-id: 7511512
description: Installer et configurer Marketo Sales Insight dans Salesforce1 - Documents Marketo - Documentation du produit
title: Installer et configurer Informations sur les ventes Marketo dans Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 3%

---

# Installation et configuration d’[!DNL Marketo Sales Insight] dans [!DNL Salesforce1] {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clients existants, veuillez [mettre à niveau votre package MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) avant de continuer !

>[!PREREQUISITES]
>
>Si vous disposez de Salesforce Enterprise/Unlimited :
>
>* [Étape 1 de 3 : ajouter des champs Marketo à  [!DNL Salesforce] (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Étape 2 sur 3 : création d’un utilisateur  [!DNL Salesforce]  Marketo (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Étape 3 sur 3 : connecter Marketo et [!DNL Salesforce] (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configuration [!DNL Marketo Sales Insight] in [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Si vous disposez de Salesforce Professional :
>
>* [Configuration de Marketo Sales Insight dans Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>[!DNL Marketo Sales Insight] dans [!DNL Salesforce1] comprend : [!DNLBest Bets], Flux de leads, Moments significatifs et Ajouter à la campagne Marketo.

## Activation de l’application mobile [!DNL Salesforce1] {#enable-the-salesforce1-mobile-app}

1. Cliquez sur **[!DNL Setup]**, puis sur **[!DNL Mobile Administration]**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Cliquez sur **[!UICONTROL Salesforce1]**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Cliquez sur **[!UICONTROL Paramètres Salesforce1]**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Cliquez sur **[!UICONTROL Activer l’application de navigateur mobile Salesforce1]**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Sélectionnez **[!UICONTROL Administration mobile]**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Cliquez sur **[!UICONTROL Gérer le menu de navigation mobile]**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Sélectionnez **[!UICONTROL Marketo]** et **[!UICONTROL Ajouter]** dans les éléments de menu **[!UICONTROL Sélectionné]**.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Sélectionnez **[!UICONTROL Marketo]**, déplacez-le **[!UICONTROL vers le haut]** dans la zone souhaitée, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Masquer l’objet personnalisé Marketo obsolète {#hide-outdated-marketo-custom-object}

1. Cliquez sur **[!UICONTROL Configurer]**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Sélectionnez **[!UICONTROL Gérer les utilisateurs]**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Sélectionnez **[!UICONTROL Profils]**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Cliquez pour **[!UICONTROL Modifier]** tous les profils souhaités.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Sous **[!UICONTROL Paramètres de tabulation]**, sélectionnez le _premier_ **[!UICONTROL Marketo]**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Sélectionnez **[!UICONTROL Tabulation masquée]**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Veillez à masquer l’onglet Marketo pour tous les profils souhaités.

## Personnaliser les onglets {#customize-tabs}

1. Cliquez sur **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Cliquez sur **[!UICONTROL Personnaliser mes onglets]**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Sélectionnez **[!UICONTROL Marketo]** et **[!UICONTROL Ajouter]** dans les onglets sélectionnés.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Sélectionnez **[!UICONTROL Marketo]**, déplacez-le **[!UICONTROL vers le haut]** dans la zone souhaitée, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personnaliser les mises en page {#customize-page-layouts}

1. Cliquez sur **[!UICONTROL Configurer]**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Cliquez sur **[!UICONTROL Configuration]**, saisissez **[!UICONTROL Mises en page]**, puis cliquez sur **[!UICONTROL Mises en page]** sous Prospects.

   >[!NOTE]
   >
   >Répétez les étapes pour chaque mise en page que votre entreprise utilise (marketing, ventes, etc.) pour les objets Contact, Compte et Opportunité.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Cliquez sur **[!UICONTROL Modifier]** pour apporter des modifications à la disposition du prospect.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Cliquez sur **[!UICONTROL Pages Visualforce]** puis faites glisser **[!UICONTROL Lead Mobile]** vers la section Cartes mobiles.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Définissez la Hauteur sur 66, puis cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Cliquez sur **[!UICONTROL Champs]** et faites glisser **[!UICONTROL Ajouter à Marketo Campaign]** vers la section **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Saisissez « Ajouter à » dans la recherche rapide pour faciliter la recherche d’Add to Marketo Campaign.

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Ouf ! Vous avez enfin fini d&#39;installer [!DNL Marketo Sales Insight] pour [!DNL Salesforce1] ! Vas-y et tape dans le dos.

>[!MORELIKETHIS]
>
>* [[!DNL Best Bets] in [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Moments significatifs dans  [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Envoi d’e-mails Marketo et actions de campagne et de watchlist dans  [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
