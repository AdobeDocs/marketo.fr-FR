---
unique-page-id: 7504893
description: Intégrez plusieurs comptes  [!DNL Google AdWords]  Marketo à l’aide d’un compte Manager dans LaunchPoint.
title: Ajouter [!DNL Google AdWords] as a [!DNL Launchpoint] Service avec un compte Manager
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 3%

---

# Ajout d’[!DNL Google AdWords] as a [!DNL Launchpoint] Service à un compte Manager {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Liez votre compte [!DNL Google AdWords] à Marketo pour charger automatiquement les données de conversion hors ligne de Marketo vers [!DNL Google AdWords]. Ensuite, à partir de l’interface utilisateur de [!DNL AdWords], vous pourrez facilement voir quels clics ont généré des prospects qualifiés, des opportunités et de nouveaux clients (ou toutes les étapes de chiffre d’affaires que vous souhaitez suivre) après avoir [ajouté des colonnes personnalisées](https://support.google.com/adwords/answer/3073556){target="_blank"} dans [!DNL AdWords]. Ces informations n’apparaissent pas dans l’interface utilisateur de Marketo.

Si vous disposez de plusieurs comptes [!DNL Google Adwords], vous pouvez utiliser un [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (anciennement appelé [!DNL My Client Center]) pour les intégrer à Marketo.

En savoir plus sur la fonctionnalité d’importation de conversions hors ligne de [Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Tous les utilisateurs de Marketo Engage n’ont pas acheté cette fonctionnalité. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

>[!NOTE]
>
>**Autorisations d’administration requises**

>[!NOTE]
>
>Vous pouvez également intégrer un [compte autonome [!DNL Google AdWords] en tant que  [!DNL Launchpoint] service](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Sélectionnez **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouveau service]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Saisissez un **[!UICONTROL Nom d’affichage]** et sélectionnez **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Sélectionnez **[!UICONTROL Autoriser Marketo]**.

   >[!NOTE]
   >
   >Veillez à vous déconnecter de votre compte [!DNL Gmail] personnel et à activer les fenêtres pop-up.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Sélectionnez le compte associé à **[!DNL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Cliquez sur **[!UICONTROL Accepter]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. Le statut s’affiche sous la forme **[!UICONTROL Succès]**. Sélectionnez **[!UICONTROL Suivant]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Chargez vos conversions hors ligne de Marketo vers [!DNL Google AdWords] **[!UICONTROL Hebdomadaire]** ou **[!UICONTROL Quotidien]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Conversion des attributs en **[!UICONTROL Premier clic]** ou **[!UICONTROL Dernier clic]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Type | Définition |
   |---|---|
   | [!UICONTROL Premier clic] | Les conversions hors ligne seront attribuées à la première publicité [!DNL AdWords] sur laquelle une personne a cliqué au cours des 90 derniers jours |
   | [!UICONTROL Dernier clic] | Les conversions hors ligne seront attribuées à la dernière publicité [!DNL AdWords] sur laquelle une personne a cliqué |

   >[!NOTE]
   >
   >[Balisage automatique](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} doit être sélectionné pour que cette fonctionnalité fonctionne. Il doit être activé dans [!DNL AdWords].

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Désélectionnez les comptes à ne pas mettre à jour. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Consultez maintenant l’article connexe ci-dessous pour savoir comment mapper [!DNL AdWords] conversions hors ligne dans votre modèle de chiffre d’affaires.

   >[!MORELIKETHIS]
   >
   >[Set [!DNL Google AdWords] Conversions dans le modèle de chiffre d’affaires avec un compte Manager](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
