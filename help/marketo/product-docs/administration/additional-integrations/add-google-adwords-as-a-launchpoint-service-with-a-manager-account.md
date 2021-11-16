---
unique-page-id: 7504893
description: Ajout de Google AdWords en tant que service Launch avec un compte de gestionnaire - Documents Marketo - Documentation du produit
title: Ajout de Google AdWords en tant que service Launch avec un compte de gestionnaire
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: ab8eb044b89c925accc3b6a4ac4def53e3927321
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 2%

---

# Ajout de Google AdWords en tant que service Launch avec un compte de gestionnaire {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Liez votre compte Google AdWords à Marketo pour charger automatiquement les données de conversion hors ligne de Marketo vers Google AdWords. Ensuite, à partir de l’interface utilisateur d’AdWords, vous pourrez facilement identifier les clics qui ont généré des prospects qualifiés, des opportunités et de nouveaux clients (ou toute étape de recettes dont vous souhaitez effectuer le suivi) après avoir effectué vos recherches.  [ajout de colonnes personnalisées](https://support.google.com/adwords/answer/3073556) dans AdWords. Ces informations n’apparaissent pas dans l’interface utilisateur de Marketo.

Si vous disposez de plusieurs comptes Google AdWords, vous pouvez utiliser une variable [Compte Google AdWords Manager](https://www.google.com/adwords/manager-accounts/) (anciennement appelé My Client Center) pour les intégrer à Marketo.

En savoir plus sur [Fonction d’importation de conversion hors ligne de Google](https://support.google.com/adwords/answer/2998031?hl=en).

>[!AVAILABILITY]
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Pour plus d’informations, contactez votre responsable du succès client.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Vous pouvez également intégrer une [compte Google AdWords autonome en tant que service LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md).

1. Accédez au **Administration** .

   ![](assets/login-admin-1.png)

1. Sélectionner **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Sélectionner **Nouveau** et **Nouveau service**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Saisissez un nom d’affichage et sélectionnez **Google AdWords**.

   ![](assets/new-service-google-1.png)

1. Sélectionner **Autoriser Marketo**.

   >[!NOTE]
   >
   >Veillez à vous déconnecter de votre compte Gmail personnel et à activer les fenêtres contextuelles.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Sélectionnez votre compte associé à **Google AdWords**.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Sélectionner **Accepter**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. L’état s’affiche comme **Succès**. Sélectionner **Suivant**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Chargement des conversions hors ligne de Marketo vers Google AdWords **Hebdomadaire** ou **Quotidien**.

   ![](assets/image2015-3-27-14-3a7-3a45.png)

1. Conversion des attributs en **Premier clic** ou **Dernier clic**.

   | Type | Définition |
   |---|---|
   | Premier clic | Les conversions hors ligne seront attribuées à la première publicité AdWords sur laquelle une personne a cliqué au cours des 90 derniers jours. |
   | Dernier clic | Les conversions hors ligne sont attribuées à la dernière publicité AdWords sur laquelle une personne a cliqué. |

   ![](assets/image2015-3-27-14-3a10-3a46.png)

   >[!NOTE]
   >
   >[Balisage automatique](https://support.google.com/adwords/answer/1752125?hl=en) doit être sélectionné pour que cette fonction fonctionne. Elle doit être activée dans AdWords.

1. Cliquez sur **Suivant**.

   ![](assets/image2015-3-27-14-3a11-3a31.png)

1. Désélectionnez les comptes que vous ne souhaitez pas mettre à jour. Cliquez sur **Créer**.

   ![](assets/image2015-3-27-14-3a12-3a51.png)

   Consultez maintenant l’article connexe ci-dessous pour savoir comment mapper les conversions hors ligne AdWords dans votre modèle de revenu.

   >[!MORELIKETHIS]
   >
   >[Définir des conversions Google AdWords dans le modèle de revenu avec un compte de gestionnaire](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md)
