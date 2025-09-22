---
unique-page-id: 6095029
description: Set [!DNL Google AdWords] Conversions dans le modèle de chiffre d’affaires - Documents Marketo - Documentation du produit
title: Définition  [!DNL Google AdWords]  conversions dans le modèle de chiffre d’affaires
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Définition [!DNL Google AdWords] conversions dans le modèle de chiffre d’affaires {#set-google-adwords-conversions-in-the-revenue-model}

Liez votre compte [!DNL Google AdWords] à Marketo pour charger automatiquement les données de conversion hors ligne de Marketo vers [!DNL Google AdWords]. Ensuite, à partir de l’interface utilisateur de [!DNL AdWords], vous pourrez facilement voir quels clics ont généré des prospects qualifiés, des opportunités et de nouveaux clients (ou toutes les étapes de chiffre d’affaires que vous souhaitez suivre) après avoir [ajouté des colonnes personnalisées](https://support.google.com/adwords/answer/3073556) dans [!DNL AdWords].

>[!NOTE]
>
>Il s’agit d’une intégration push de Marketo vers [!DNL Google AdWords]. Les données de conversion s’affichent _uniquement_ dans votre portail [!DNL Google AdWords], _pas dans l’interface utilisateur de Marketo_.

En savoir plus sur la fonctionnalité d’importation de conversions hors ligne de [Google](https://support.google.com/adwords/answer/2998031?hl=en). Mappez [!DNL AdWords] conversions hors ligne à une ou plusieurs étapes d’un modèle de chiffre d’affaires. Il existe trois façons d’effectuer le mappage :

* Conversion [!DNL AdWords]
* Action de l’étape
* Mappage [!DNL AdWords]

Vous pouvez créer une conversion hors ligne [!DNL AdWords] à partir de Marketo à l’aide de l’action d’évaluation.

>[!PREREQUISITES]
>
>[Ajouter [!DNL Google AdWords] as a LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Utiliser la conversion [!DNL AdWords] {#use-adwords-conversion}

1. Accédez à la zone **[!UICONTROL Analytics]**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Sélectionnez un modèle.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Sélectionnez l’étape de chiffre d’affaires que vous souhaitez mapper à une conversion de [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Sélectionnez la **[!UICONTROL Conversion AdWords]** à mapper à votre étape Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Joli ! Vos données de conversion [!DNL AdWords] seront chargées dans votre [!DNL Google AdWords] à la cadence que vous avez sélectionnée.

## Utiliser l’action d’évaluation {#use-stage-action}

Vous pouvez également mapper une [!UICONTROL conversion AdWords] sous **[!UICONTROL actions d’évaluation]**.

1. Sélectionnez l’étape à mapper à une conversion [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Dans le menu déroulant **[!UICONTROL Actions de l’étape]**, sélectionnez **[!UICONTROL Définir la conversion AdWords]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Sélectionnez une **[!UICONTROL Conversion AdWords]**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Conseil** : si vous ne disposez d’aucune conversion [!DNL AdWords], créez-en une en cliquant sur **[!UICONTROL +Nouvelle conversion]**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Une fois que vous avez terminé de mapper toutes vos conversions [!DNL AdWords] aux étapes de chiffre d’affaires, revenez à la page de résumé. Sélectionnez **[!UICONTROL Actions du modèle]** et choisissez **[!UICONTROL Approuver les étapes]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Conseil de pro : Ajouter une nouvelle conversion {#pro-tip-add-a-new-conversion}

Conseil de pro ! Une nouvelle conversion hors ligne [!DNL AdWords] peut être créée à partir de Marketo.

>[!CAUTION]
>
>Le paramètre « optimisation » est activé pour les nouvelles conversions créées à partir de Marketo. Cela signifie que [!DNL AdWords] stratégies d’enchères sont autorisées pour optimiser vos enchères pour ces conversions. Vous pouvez modifier ce paramètre à partir de votre compte [!DNL AdWords].

1. Dans le menu déroulant **[!UICONTROL Actions de l’étape]**, sélectionnez **[!UICONTROL Définir la conversion AdWords]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Sélectionnez **[!UICONTROL Nouvelle conversion]**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Saisissez un **[!UICONTROL Nom de conversion]**. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Excellent ! Cette nouvelle conversion apparaîtra dans votre compte [!DNL AdWords].

## Utiliser le mappage de [!DNL AdWords] {#use-adwords-mapping}

Vous pouvez associer toutes vos étapes de modèle à votre [!UICONTROL conversion AdWords] au même endroit à l’aide des mappages [!DNL AdWords].

1. Sélectionnez **[!UICONTROL Modifier les mappages AdWords]**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Sélectionnez la **[!UICONTROL Conversion AdWords]** souhaitée pour chaque étape dont vous souhaitez effectuer le suivi.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Une fois les étapes mappées, cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Une fois que vous avez terminé de mapper toutes vos conversions [!DNL AdWords] aux étapes de chiffre d’affaires, revenez à la page de résumé. Sélectionnez **[!UICONTROL Actions du modèle]** et choisissez **[!UICONTROL Approuver les étapes]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Pour afficher les données de conversion hors ligne, vous devez vous connecter à votre compte [!DNL AdWords]. Nous vous recommandons d’utiliser leur [fonction Colonnes personnalisées](https://support.google.com/adwords/answer/3073556) pour créer des colonnes de nombre de conversions pour chaque conversion hors ligne que vous importez à partir de Marketo.
