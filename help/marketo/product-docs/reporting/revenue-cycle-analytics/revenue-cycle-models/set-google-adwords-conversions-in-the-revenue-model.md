---
unique-page-id: 6095029
description: Définir les conversions Google AdWords dans le modèle de recettes - Documents marketing - Documentation du produit
title: Définir les conversions Google AdWords dans le modèle de recettes
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---


# Définir les conversions Google AdWords dans le modèle de recettes {#set-google-adwords-conversions-in-the-revenue-model}

Liez votre compte Google AdWords à Marketo pour télécharger automatiquement les données de conversion hors ligne de Marketo vers Google AdWords. Ensuite, à partir de l’interface utilisateur d’AdWords, vous pourrez identifier facilement les clics qui ont généré des pistes qualifiées, des opportunités et de nouveaux clients (ou les étapes de recettes dont vous souhaitez effectuer le suivi) après avoir [ajouté des colonnes personnalisées](https://support.google.com/adwords/answer/3073556) dans AdWords.

>[!NOTE]
>
>Il s’agit d’une intégration Push de Marketo vers Google AdWords. Les données de conversion s’affichent *uniquement* dans votre portail Google AdWords,** pas dans l’interface utilisateur de Marketing. **

En savoir plus sur [la fonction d&#39;importation de conversion hors ligne de Google](https://support.google.com/adwords/answer/2998031?hl=en).  Faites correspondre les conversions hors ligne d’AdWords à une ou plusieurs étapes d’un modèle de recettes. Il existe trois méthodes pour effectuer la cartographie :

* Conversion d’AdWords
* Action d’état
* Mappage des mots publicitaires

Vous pouvez créer une conversion hors ligne d’AdWords à partir de Marketo si vous utilisez l’action d’étape.

>[!PREREQUISITES]
>
>* [Ajouter Google AdWords comme service LaunchPoint](../../../../product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

>



## Utiliser la conversion AdWords {#use-adwords-conversion}

1. Accédez à la zone **Analytics**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Sélectionnez un modèle.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Cliquez sur **Modifier le brouillon**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Sélectionnez l’étape de recettes à mapper à une conversion AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Sélectionnez la **conversion AdWords** que vous souhaitez mapper à votre étape Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Sympa ! Vos données de conversion AdWords seront téléchargées dans vos Google AdWords à la cadence que vous avez sélectionnée.

## Utiliser l&#39;action d&#39;état {#use-stage-action}

Vous pouvez également mapper une conversion AdWords sous Actions d’étape.

1. Sélectionnez l’étape à mapper à une conversion AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Dans la liste déroulante **Actions d’étape**, sélectionnez **Définir la conversion des mots publicitaires**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Sélectionnez une **conversion AdWords**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Conseil** : Si vous n’avez pas de conversions AdWords, créez-en une en cliquant sur  **+Nouvelle conversion**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Une fois que vous avez terminé de mapper toutes vos conversions AdWords aux étapes des recettes, revenez à la page de résumé. Sélectionnez **Actions du modèle** et choisissez **Approuver les étapes**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Conseil professionnel : Ajouter une nouvelle conversion {#pro-tip-add-a-new-conversion}

Conseil professionnel ! Une nouvelle conversion hors ligne d’AdWords peut être créée à partir de Marketo.

>[!CAUTION]
>
>Le paramètre &quot;optimisation&quot; est activé pour les nouvelles conversions créées à partir de Marketing. Cela signifie que les stratégies d’offres AdWords sont autorisées à optimiser vos offres pour ces conversions. Vous pouvez modifier ce paramètre à partir de votre compte AdWords.

1. Dans la liste déroulante **Actions d’étape**, sélectionnez **Définir la conversion des mots publicitaires**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Sélectionnez **Nouvelle conversion**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Saisissez un **nom de conversion**. Cliquez sur **Enregistrer**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Excellent ! Cette nouvelle conversion apparaîtra dans votre compte AdWords.

## Utiliser le mappage AdWords {#use-adwords-mapping}

Vous pouvez associer toutes les étapes de votre modèle à votre conversion AdWords en un seul endroit à l’aide des mappages AdWords.

1. Sélectionnez **Modifier les mappages AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Sélectionnez la **conversion AdWords** de votre choix pour chaque étape dont vous souhaitez effectuer le suivi.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Une fois que vous avez mappé vos étapes, cliquez sur **Enregistrer**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Une fois que vous avez terminé de mapper toutes vos conversions AdWords aux étapes des recettes, revenez à la page de résumé. Sélectionnez **Actions du modèle** et choisissez **Approuver les étapes**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Pour vue des données de conversion hors ligne, vous devez vous connecter à votre compte AdWords. Nous vous recommandons d&#39;utiliser la fonction [Colonnes personnalisées](https://support.google.com/adwords/answer/3073556) pour créer des colonnes de nombre de conversions pour chaque conversion hors ligne importée à partir de Marketing.
