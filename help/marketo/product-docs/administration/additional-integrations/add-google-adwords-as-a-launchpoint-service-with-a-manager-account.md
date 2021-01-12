---
unique-page-id: 7504893
description: Ajouter Google AdWords en tant que service de point de lancement avec un compte de gestionnaire - Docs marketing - Documentation du produit
title: Ajouter Google AdWords en tant que service de point de lancement avec un compte de gestionnaire
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---


# Ajouter Google AdWords en tant que service de point de lancement avec un compte de gestionnaire {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Liez votre compte Google AdWords à Marketo pour télécharger automatiquement les données de conversion hors ligne de Marketo vers Google AdWords. Ensuite, à partir de l’interface utilisateur d’AdWords, vous pourrez identifier facilement les clics qui ont généré des pistes qualifiées, des opportunités et de nouveaux clients (ou les étapes de recettes dont vous souhaitez effectuer le suivi) après avoir [ajouté des colonnes personnalisées](https://support.google.com/adwords/answer/3073556) dans AdWords. Ces informations n’apparaissent pas dans l’interface utilisateur de Marketing Cloud.

Si vous disposez de plusieurs comptes Google Adwords, vous pouvez utiliser un [compte Google AdWords Manager](https://www.google.com/adwords/manager-accounts/) (anciennement appelé My Client Center) pour les intégrer à Marketo.

En savoir plus sur [la fonction d&#39;importation de conversion hors ligne de Google](https://support.google.com/adwords/answer/2998031?hl=en).

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Vous pouvez également intégrer un [compte Google AdWords autonome en tant que service Launchpoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md).

1. Accédez à la section **Admin**.

   ![](assets/login-admin-1.png)

1. Sélectionnez **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Sélectionnez **New** et **New Service**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Saisissez un nom d’affichage et sélectionnez **Google AdWords**.

   ![](assets/new-service-google-1.png)

1. Sélectionnez **Autoriser le marketing**.

   >[!NOTE]
   >
   >Veillez à vous déconnecter de votre compte Gmail personnel et à activer les fenêtres contextuelles.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Sélectionnez votre compte associé à **Google AdWords**.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Sélectionnez **Accepter**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. L’état s’affiche sous la forme **Succès**. Sélectionnez **Suivant**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Transférez vos conversions hors ligne de Marketo vers Google AdWords **Hebdomadairement** ou **Quotidien**.

   ![](assets/image2015-3-27-14-3a7-3a45.png)

1. Conversion d’attribut en **Premier clic** ou **Dernier clic**.

   | Type | Définition |
   |---|---|
   | Premier clic | Les conversions hors ligne sont attribuées aux premiers mots publicitaires et qu’une personne a cliqué au cours des 90 derniers jours |
   | Dernier clic | Les conversions hors ligne sont attribuées aux derniers mots publicitaires et qu’une personne a cliqué sur eux. |

   ![](assets/image2015-3-27-14-3a10-3a46.png)

   >[!NOTE]
   >
   >[Le ](https://support.google.com/adwords/answer/1752125?hl=en) balisage automatique doit être sélectionné pour que cette fonction fonctionne. Elle doit être activée dans AdWords.

1. Cliquez sur **Suivant**.

   ![](assets/image2015-3-27-14-3a11-3a31.png)

1. Désélectionnez les comptes que vous ne souhaitez pas mettre à jour. Cliquez sur **Créer**.

   ![](assets/image2015-3-27-14-3a12-3a51.png)

   Consultez maintenant l’article associé ci-dessous pour savoir comment mapper les conversions hors ligne d’AdWords dans votre modèle de recettes.

   >[!MORELIKETHIS]
   >
   >[Définir les conversions Google AdWords dans le modèle Recettes avec un compte de gestionnaire](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md)
