---
unique-page-id: 7511512
description: Installer et configurer Marketo Sales Insight dans Salesforce1 - Marketo Docs - Documentation sur les produits
title: Installer et configurer Marketo Sales Insight dans Salesforce1
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Installer et configurer Marketo Sales Insight dans Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clients existants, [Mettez à niveau votre package MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) avant de continuer !

>[!PREREQUISITES]
>
>Si vous possédez Salesforce Enterprise/Unlimited :
>
>* [Étape 1 sur 3 : Ajouter les champs du marketing à Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Étape 2 sur 3 : Créer un utilisateur Salesforce pour Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Étape 3 sur 3 : Connecter Marketing et Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

>
>
Si vous possédez Salesforce Professional :
>
>* [Configuration de Marketo Sales Insight dans Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)

>



>[!NOTE]
>
>Marketo Sales Insight in Salesforce1 inclut : Meilleurs paris, Flux de pistes, Moments intéressants et Ajoute à Marketing Campaign.

## Activation de l’application mobile Salesforce1 {#enable-the-salesforce1-mobile-app}

1. Cliquez sur **Configuration**, puis sur **Administration mobile**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Cliquez sur **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Cliquez sur **Paramètres Salesforce1**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Cliquez sur **Activer l’application de navigateur mobile Salesforce1**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Sélectionnez **Administration mobile**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Cliquez sur **Gérer le menu de navigation mobile**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Sélectionnez **Marketo** et **Ajouter** dans les options de menu **Sélectionné**.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Sélectionnez **Marketo**, déplacez **Haut** vers une zone souhaitée, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Masquer l&#39;objet personnalisé Marketo obsolète {#hide-outdated-marketo-custom-object}

1. Cliquez sur **Configuration**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Sélectionnez **Gérer les utilisateurs**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Sélectionnez **Profils**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Cliquez pour **modifier** les profils de votre choix.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Sous **Paramètres d&#39;onglet**, sélectionnez _first_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Sélectionnez **Onglet Masqué**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Veillez à masquer l’onglet Marketo pour tous les profils de votre choix !

## Personnaliser les onglets {#customize-tabs}

1. Cliquez sur **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Cliquez sur **Personnaliser mes onglets**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Sélectionnez **Marketo** et **Ajouter** à l&#39;onglet Sélectionné.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Sélectionnez **Marketo**, déplacez **Haut** vers une zone souhaitée, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personnaliser les mises en page {#customize-page-layouts}

1. Cliquez sur **Configuration**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Cliquez sur **Configuration**, tapez **Mise en page**, puis cliquez sur **Mise en page** sous Pistes.

   >[!NOTE]
   >
   >Répétez les étapes pour chaque mise en page utilisée par votre entreprise (marketing, ventes, etc.). pour les objets Contact, Compte et Opportunité.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Cliquez sur **Modifier** pour apporter des modifications à la disposition des pistes.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Cliquez sur **Visualforce Pages**, puis faites glisser **Lead Mobile** vers la section Mobile Cards.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Remplacez la Hauteur par 66, puis cliquez sur **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Cliquez sur **Champs** et faites glisser **Ajouter à Marketo Campaign** vers la section **Marketo Sales Insight**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Tapez &quot;Ajouter à&quot; dans la Recherche rapide pour faciliter l&#39;Ajoute à Marketo Campaign.

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Ouf ! Vous avez enfin terminé d&#39;installer Marketo Sales Insight for Salesforce1 ! Allez-y et donnez-vous une tape sur le dos.

>[!MORELIKETHIS]
>
>* [Meilleurs paris dans Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Moments intéressants à Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Envoyer un courrier électronique marketing et des actions Campaign et Watchlist dans Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)

