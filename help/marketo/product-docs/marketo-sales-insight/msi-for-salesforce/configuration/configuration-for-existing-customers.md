---
unique-page-id: 42762519
description: Configuration pour les clients existants - Documents Marketo - Documentation du produit
title: Configuration pour les clients existants
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Configuration pour les clients existants {#configuration-for-existing-customers}

Configurez la configuration suivante afin de commencer à utiliser le nouveau tableau de bord des statistiques.

>[!PREREQUISITES]
>
>Vérifiez que vous avez mis à niveau votre package Salesforce vers la dernière version.

## Configuration de Sales Insight dans Marketo {#configure-sales-insight-in-marketo}

1. Ouvrez un nouvel onglet dans votre navigateur pour obtenir les informations d’identification Marketo Sales Insights de votre compte Marketo.

1. Accédez à la zone **Admin**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Cliquez sur **Sales Insight**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Cliquez sur **Afficher** pour renseigner les informations d’identification de l’API REST.

   ![](assets/configuration-for-existing-customers-3.png)

1. Vous verrez une fenêtre contextuelle de confirmation. Cliquez sur **OK**.

## Configuration de Sales Insight dans Salesforce {#configure-sales-insight-in-salesforce}

1. Dans Salesforce, cliquez sur **Setup**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Recherchez et sélectionnez **Paramètres du site distant**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Cliquez sur **Nouveau site distant**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Saisissez le nom du site distant (il peut s’agir de &quot;MarketoRestAPI&quot;) et l’URL du site distant (l’URL de votre API depuis le panneau Configuration de l’API REST dans Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/configuration-for-existing-customers-8.png)

   Vous avez maintenant créé un paramètre de site distant pour l’API REST.

## Accès Sales Insight de Marketo {#access-marketo-sales-insight}

1. Copiez les informations d’identification du panneau API REST dans la page d’administration des statistiques sur les ventes de Marketo. Collez-les dans la section API REST de la page de configuration des statistiques sur les ventes de Salesforce.

1. Saisissez la clé secrète de l’API.

   ![](assets/configuration-for-existing-customers-9.png)
