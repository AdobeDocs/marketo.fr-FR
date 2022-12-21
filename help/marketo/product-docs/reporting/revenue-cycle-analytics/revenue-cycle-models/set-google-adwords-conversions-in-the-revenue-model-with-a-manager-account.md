---
unique-page-id: 7504923
description: Définir les conversions Google AdWords dans le modèle de revenu avec un compte de gestionnaire - Documents Marketo - Documentation du produit
title: Définir des conversions Google AdWords dans le modèle de revenu avec un compte de gestionnaire
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Définir des conversions Google AdWords dans le modèle de revenu avec un compte de gestionnaire {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Liez votre compte Google AdWords à Marketo pour charger automatiquement les données de conversion hors ligne de Marketo vers Google AdWords. Ensuite, à partir de l’interface utilisateur d’AdWords, vous pourrez facilement identifier les clics qui ont généré des prospects qualifiés, des opportunités et de nouveaux clients (ou toute étape de recettes dont vous souhaitez effectuer le suivi) après avoir effectué vos recherches. [ajout de colonnes personnalisées](https://support.google.com/adwords/answer/3073556) dans AdWords.

Si vous disposez de plusieurs comptes Google AdWords, vous pouvez utiliser une variable [Compte Google AdWords Manager](https://www.google.com/adwords/manager-accounts/) (anciennement appelé My Client Center) pour les intégrer à Marketo.

Vous pouvez mapper des conversions hors ligne AdWords à une ou plusieurs scènes dans un modèle Recettes. Il existe deux façons :

* Action d’évaluation
* Mappage AdWords

>[!PREREQUISITES]
>
>[Ajout de Google AdWords en tant que service Launch avec un compte de gestionnaire](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Utilisation d’une action d’étape {#use-stage-action}

Mappage d’une conversion AdWords sous Actions intermédiaires.

1. Sélectionnez l’étape à mapper à une conversion AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Sous , **Actions de l’étape** menu déroulant, sélectionnez **Définir la conversion d’AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Définissez un **Conversion d’AdWords**.

   >[!NOTE]
   >
   >Une conversion AdWords différente peut être sélectionnée pour chaque compte enfant.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Conseil : Si vous ne disposez d’aucune conversion AdWords, créez-en une en cliquant sur **+Nouvelle conversion**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. Une fois le mappage de toutes vos conversions AdWords aux phases de recettes terminé, revenez à la page de résumé. Sélectionner **Actions de modèle** et choisissez **Approuver les étapes**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Conseil : Ajout d’une nouvelle conversion {#pro-tip-add-a-new-conversion}

Conseil professionnel ! Une nouvelle conversion hors ligne AdWords peut être créée à partir de Marketo.

>[!CAUTION]
>
>Le paramètre &quot;optimisation&quot; est activé pour les nouvelles conversions créées à partir de Marketo. Cela signifie que les stratégies d’offres AdWords sont autorisées à optimiser vos offres pour ces conversions. Vous pouvez modifier ce paramètre à partir de votre compte AdWords.

1. Sous , **Actions de l’étape** menu déroulant, sélectionnez **Définir la conversion d’AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Sélectionner **Nouvelle conversion**.

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Saisissez un **Nom de la conversion**. Cliquez sur **Enregistrer**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Excellent ! Cette nouvelle conversion apparaîtra dans votre compte AdWords.

## Utilisation du mappage AdWords {#use-adwords-mapping}

Vous pouvez associer toutes vos scènes de modèle à votre conversion AdWords à un seul emplacement à l’aide des mappages AdWords.

1. Sélectionner **Modifier les mappages AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Sélectionnez la **Compte AdWords** et désiré **Conversion d’AdWords** pour chaque étape dont vous souhaitez effectuer le suivi.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Une fois que vous avez mappé vos scènes, cliquez sur **Enregistrer**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Une fois le mappage de toutes vos conversions AdWords aux phases de recettes terminé, revenez à la page de résumé. Sélectionner **Actions de modèle** et choisissez **Approuver les étapes**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Pour afficher les données de conversion hors ligne, vous devez vous connecter à votre compte AdWords. Nous vous recommandons d’utiliser les [Fonctionnalité Colonnes personnalisées](https://support.google.com/adwords/answer/3073556) pour créer des colonnes de comptage de conversion pour chaque conversion hors ligne que vous importez à partir de Marketo.
