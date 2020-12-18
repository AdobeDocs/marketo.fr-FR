---
unique-page-id: 7504923
description: Définir les conversions Google AdWords dans le modèle de recettes avec un compte de gestionnaire - Documents marketing - Documentation du produit
title: Définir les conversions Google AdWords dans le modèle Recettes avec un compte de gestionnaire
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---


# Définir les conversions Google AdWords dans le modèle de recettes avec un compte de gestionnaire {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Liez votre compte Google AdWords à Marketo pour télécharger automatiquement les données de conversion hors ligne de Marketo vers Google AdWords. Ensuite, à partir de l’interface utilisateur d’AdWords, vous pourrez identifier facilement les clics qui ont généré des pistes qualifiées, des opportunités et de nouveaux clients (ou les étapes de recettes dont vous souhaitez effectuer le suivi) après avoir [ajouté des colonnes personnalisées](https://support.google.com/adwords/answer/3073556) dans AdWords.

Si vous disposez de plusieurs comptes Google Adwords, vous pouvez utiliser un [compte Google AdWords Manager](https://www.google.com/adwords/manager-accounts/) (anciennement appelé My Client Center) pour les intégrer à Marketo.

Vous pouvez mapper des conversions hors ligne AdWords à une ou plusieurs étapes d’un modèle de recettes. Il existe deux façons :

* Action d’état
* Mappage des mots publicitaires

>[!PREREQUISITES]
>
>* [Ajouter Google AdWords en tant que service de point de lancement avec un compte de gestionnaire](../../../../product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

>



## Utiliser l&#39;action d&#39;état {#use-stage-action}

Faites correspondre une conversion AdWords sous Actions d’étape.

1. Sélectionnez l’étape à mapper à une conversion AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Dans la liste déroulante **Actions d’étape**, sélectionnez **Définir la conversion des mots publicitaires**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Définissez une conversion **AdWords**.

   >[!NOTE]
   >
   >Une conversion AdWords différente peut être sélectionnée pour chaque compte enfant.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Conseil : Si vous n’avez aucune conversion AdWords, créez-en une en cliquant sur **+Nouvelle conversion**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ** ![](assets/image2015-3-27-17-3a23-3a13.png)

   **

1. Saisissez un **nom de conversion**. Cliquez sur **Enregistrer**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Excellent ! Cette nouvelle conversion apparaîtra dans votre compte AdWords.

## Utiliser le mappage AdWords {#use-adwords-mapping}

Vous pouvez associer toutes les étapes de votre modèle à votre conversion AdWords en un seul endroit à l’aide des mappages AdWords.

1. Sélectionnez **Modifier les mappages AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Sélectionnez un **compte AdWords** et une **conversion AdWords** pour chaque étape dont vous souhaitez effectuer le suivi.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Une fois que vous avez mappé vos étapes, cliquez sur **Enregistrer**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Une fois que vous avez terminé de mapper toutes vos conversions AdWords aux étapes des recettes, revenez à la page de résumé. Sélectionnez **Actions du modèle** et choisissez **Approuver les étapes**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Pour vue des données de conversion hors ligne, vous devez vous connecter à votre compte AdWords. Nous vous recommandons d&#39;utiliser la fonction [Colonnes personnalisées](https://support.google.com/adwords/answer/3073556) pour créer des colonnes de nombre de conversions pour chaque conversion hors ligne importée à partir de Marketing.
