---
unique-page-id: 42762519
description: Configuration pour les clients existants - Documents Marketo - Documentation du produit
title: Configuration pour les clientes et clients existants
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 9%

---

# Configuration pour les clientes et clients existants {#configuration-for-existing-customers}

Veuillez configurer la configuration suivante pour commencer à utiliser le nouveau tableau de bord d’Insights.

>[!PREREQUISITES]
>
>Assurez-vous d’avoir mis à niveau votre package [!DNL Salesforce] vers la dernière version

## Configuration de [!DNL Sales Insight] dans Marketo {#configure-sales-insight-in-marketo}

1. Ouvrez un nouvel onglet dans votre navigateur pour obtenir les informations d’identification [!DNL Marketo Sales Insights] à partir de votre compte Marketo.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Cliquez sur **[!UICONTROL Ventes Insight]**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Cliquez sur **[!UICONTROL Afficher]** pour renseigner les informations d’identification de l’API REST.

   ![](assets/configuration-for-existing-customers-3.png)

1. Un pop-up de confirmation s’affiche. Cliquez sur **[!UICONTROL OK]**.

## Configuration de [!DNL Sales Insight] dans [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. Dans Salesforce, cliquez sur **[!UICONTROL Configuration]**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Recherchez et sélectionnez **[!UICONTROL Paramètres du site distant]**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Cliquez sur **[!UICONTROL Nouveau site distant]**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Saisissez le [!UICONTROL  Nom du site distant ] (par exemple, « MarketoRestAPI ») et l’[!UICONTROL URL du site distant ] (votre URL d’API à partir du panneau Configuration de l’API REST dans Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/configuration-for-existing-customers-8.png)

   Vous avez maintenant créé un paramètre de site distant pour l’API REST.

## Accès Sales Insight de Marketo {#access-marketo-sales-insight}

1. Copiez les informations d’identification depuis le panneau API Rest de [!DNL Marketo’s Sales Insight] page Admin . Collez-les dans la section API Rest de la page Configuration [!DNL Sales Insight] de Salesforce.

1. Saisissez la [!UICONTROL  Clé secrète API ].

   ![](assets/configuration-for-existing-customers-9.png)
