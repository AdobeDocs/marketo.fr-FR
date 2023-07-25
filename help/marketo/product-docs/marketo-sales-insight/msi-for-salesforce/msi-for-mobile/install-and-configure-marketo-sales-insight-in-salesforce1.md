---
unique-page-id: 7511512
description: Installation et configuration de Marketo Sales Insight dans Salesforce1 - Documents Marketo - Documentation du produit
title: Installation et configuration de Marketo Sales Insight dans Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Installation et configuration de Marketo Sales Insight dans Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clients existants, veuillez [Mettre à niveau votre package MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) avant de continuer !

>[!PREREQUISITES]
>
>Si vous disposez de Salesforce Enterprise/Unlimited :
>
>* [Étape 1 sur 3 : Ajout de champs Marketo à Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Étape 2 sur 3 : Création d’un utilisateur Salesforce pour Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Étape 3 sur 3 : Connexion de Marketo et de Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Si vous disposez de Salesforce Professional :
>
>* [Configuration de Marketo Sales Insight dans Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>Marketo Sales Insight in Salesforce1 comprend : Meilleurs paris, Flux de pistes, Moments intéressants et Ajouter à Marketo Campaign.

## Activation de l’application mobile Salesforce1 {#enable-the-salesforce1-mobile-app}

1. Cliquez sur **Configuration** puis **Administration mobile**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Cliquez sur **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Cliquez sur **Paramètres Salesforce1**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Cliquez sur **Activation de l’application de navigateur mobile Salesforce1**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Sélectionner **Administration mobile**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Cliquez sur **Gestion du menu de navigation mobile**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Sélectionner **Marketo** et **Ajouter** à l’adresse **Sélectionné** éléments de menu.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Sélectionner **Marketo**, déplacez-le **Monter** dans la zone de votre choix, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Masquer l’objet personnalisé Marketo obsolète {#hide-outdated-marketo-custom-object}

1. Cliquez sur **Configuration**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Sélectionner **Gestion des utilisateurs**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Sélectionner **Profils**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Cliquez sur pour **edit** tous les profils souhaités.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Sous **Paramètres d’onglet**, sélectionnez la variable _first_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Sélectionner **Tabulation masquée**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Veillez à masquer l’onglet Marketo pour tous les profils souhaités !

## Personnalisation des onglets {#customize-tabs}

1. Cliquez sur **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Cliquez sur **Personnalisation de mes onglets**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Sélectionner **Marketo** et **Ajouter** dans les onglets sélectionnés.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Sélectionner **Marketo**, déplacez-le **Monter** dans la zone de votre choix, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personnalisation des mises en page {#customize-page-layouts}

1. Cliquez sur **Configuration**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Cliquez sur **Configuration**, type **Disposition de page**, puis cliquez sur **Disposition de page** sous Pistes.

   >[!NOTE]
   >
   >Répétez les étapes pour chaque mise en page utilisée par votre entreprise (marketing, ventes, etc.). pour les objets Contact, Compte et Opportunité.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Cliquez sur **Modifier** pour apporter des modifications à la mise en page des pistes.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Cliquez sur **Pages Visualforce** puis faites glisser **Lead Mobile** à la section Cartes mobiles .

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Définissez la Hauteur sur 66, puis cliquez sur **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Cliquez sur **Champs** et faire glisser **Ajouter à Marketo Campaign** au **Marketo Sales Insight** .

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Saisissez &quot;Ajouter à&quot; dans la recherche rapide pour faciliter la recherche d’Add to Marketo Campaign.

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Ouf ! Vous avez enfin terminé d’installer Marketo Sales Insight for Salesforce1 ! Allez-y et donnez-vous une tape sur le dos.

>[!MORELIKETHIS]
>
>* [Meilleurs paris sur Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Moments intéressants dans Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Envoyer le courrier électronique Marketo et Campaign et les actions de liste de contrôle dans Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
