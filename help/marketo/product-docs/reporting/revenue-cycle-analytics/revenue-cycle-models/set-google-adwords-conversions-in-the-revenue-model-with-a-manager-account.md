---
unique-page-id: 7504923
description: Définition  [!DNL Google AdWords]  conversions dans le modèle de chiffre d’affaires avec un compte Manager - Documents Marketo - Documentation du produit
title: Définition  [!DNL Google AdWords]  conversions dans le modèle de chiffre d’affaires avec un compte Manager
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Définition des conversions [!DNL Google AdWords] dans le modèle de chiffre d’affaires avec un compte Manager {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Liez votre compte [!DNL Google AdWords] à Marketo pour charger automatiquement les données de conversion hors ligne de Marketo vers [!DNL Google AdWords]. Ensuite, à partir de l’interface utilisateur de [!DNL AdWords], vous pourrez facilement voir quels clics ont généré des prospects qualifiés, des opportunités et de nouveaux clients (ou toutes les étapes de chiffre d’affaires que vous souhaitez suivre) après avoir [ajouté des colonnes personnalisées](https://support.google.com/adwords/answer/3073556) dans [!DNL AdWords].

Si vous disposez de plusieurs comptes [!DNL Google Adwords], vous pouvez utiliser un compte [[!DNL Google AdWords] Manager](https://www.google.com/adwords/manager-accounts/) (anciennement appelé Mon centre client) pour les intégrer à Marketo.

Vous pouvez mapper [!DNL AdWords] conversions hors ligne à une ou plusieurs étapes d’un modèle de chiffre d’affaires. Il existe deux méthodes :

* Action de l’étape
* Mappage [!DNL AdWords]

>[!PREREQUISITES]
>
>[Ajouter [!DNL Google AdWords] as a Launchpoint Service avec un compte Manager](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Utiliser l’action d’évaluation {#use-stage-action}

Mappez une conversion [!DNL AdWords] sous Actions d’évaluation.

1. Sélectionnez l’étape à mapper à une conversion [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Dans le menu déroulant **[!UICONTROL Actions de l’étape]**, sélectionnez **[!UICONTROL Définir la conversion AdWords]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Définissez une conversion de **[!DNL AdWords]**.

   >[!NOTE]
   >
   >Une conversion [!DNL AdWords] différente peut être sélectionnée pour chaque compte enfant.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Conseil : si vous n’avez aucune conversion [!DNL AdWords], créez-en une en cliquant sur **[!UICONTROL +Nouvelle conversion]**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Saisissez un **Nom de conversion**. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Excellent ! Cette nouvelle conversion apparaîtra dans votre compte [!DNL AdWords].

## Utiliser le mappage de [!DNL AdWords] {#use-adwords-mapping}

Vous pouvez associer toutes vos étapes de modèle à votre conversion de [!DNL AdWords] en un seul endroit à l’aide de mappages [!DNL AdWords].

1. Sélectionnez **[!UICONTROL Modifier les mappages AdWords]**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Sélectionnez le compte **[!DNL AdWords]souhaité** ainsi que la conversion **[!DNL AdWords]souhaitée** pour chaque étape que vous souhaitez suivre.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Une fois les étapes mappées, cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Une fois que vous avez terminé de mapper toutes vos conversions [!DNL AdWords] aux étapes de chiffre d’affaires, revenez à la page de résumé. Sélectionnez **[!UICONTROL Actions du modèle]** et choisissez **[!UICONTROL Approuver les étapes]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Pour afficher les données de conversion hors ligne, vous devez vous connecter à votre compte [!DNL AdWords]. Nous vous recommandons d’utiliser leur [fonction Colonnes personnalisées](https://support.google.com/adwords/answer/3073556) pour créer des colonnes de nombre de conversions pour chaque conversion hors ligne que vous importez à partir de Marketo.
