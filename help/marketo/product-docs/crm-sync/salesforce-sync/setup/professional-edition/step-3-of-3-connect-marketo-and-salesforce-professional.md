---
unique-page-id: 3571800
description: Étape 3 sur 3 - Connecter Marketo et Salesforce (Professionnel) - Documentation de Marketo - Documentation du produit
title: Étape 3 sur 3 - Connecter Marketo et Salesforce (Professionnel)
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Étape 3 sur 3 : connecter Marketo et [!DNL Salesforce] (Professionnel) {#step-of-connect-marketo-and-salesforce-professional}

Dans cet article, vous allez configurer Marketo Engage pour qu’il se synchronise avec l’instance Salesforce configurée.

>[!PREREQUISITES]
>
>* [Étape 1 de 3 : ajouter des champs Marketo à Salesforce (professionnel)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}
>* [Étape 2 sur 3 : création d’un utilisateur Salesforce pour Marketo (professionnel)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}

## Récupérer le jeton de sécurité de l’utilisateur de synchronisation {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si vous disposez déjà du jeton de sécurité, passez directement à Définition des informations d’identification de l’utilisateur de synchronisation et félicitations pour la préparation !

1. Connectez-vous à Salesforce avec l’utilisateur de synchronisation Marketo, cliquez sur le nom de l’utilisateur de synchronisation, puis sur **[!UICONTROL Mes paramètres]**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Dans la barre de recherche de navigation, saisissez « reset », puis cliquez sur **[!UICONTROL Réinitialiser mon jeton de sécurité]**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Cliquez sur **[!UICONTROL Réinitialiser le jeton de sécurité]**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Le jeton de sécurité vous sera envoyé par e-mail.

## Définir les informations d’identification de l’utilisateur de synchronisation {#set-sync-user-credentials}

1. Dans Marketo, accédez à **[!UICONTROL Admin]**, sélectionnez **[!UICONTROL CRM]**, puis cliquez sur **[!UICONTROL Synchroniser avec Salesforce.com]**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Veillez à [masquer tous les champs dont vous n’avez pas besoin](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} dans Marketo à l’utilisateur de synchronisation avant de cliquer sur **[!UICONTROL Synchroniser les champs]**. Une fois que vous avez cliqué sur Synchroniser les champs, tous les champs que l’utilisateur peut voir seront créés définitivement dans Marketo et ne peuvent pas être supprimés.

1. Saisissez les informations d’identification de l’utilisateur de synchronisation Salesforce créées dans la partie 2 de la configuration de Salesforce ([Professionnel](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Entreprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) et cliquez sur **[!UICONTROL Champs de synchronisation]**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Cochez la case **[!UICONTROL Sandbox]** si vous synchronisez un sandbox Marketo avec un sandbox Salesforce.

1. Lisez l’avertissement, puis cliquez sur **[!UICONTROL Confirmer les informations d’identification]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si vous souhaitez parcourir les [mappages et les personnaliser](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"}, c’est votre seule chance de le faire ! Une fois que vous avez cliqué sur Démarrer la synchronisation Salesforce, tout est terminé.

## Démarrer [!DNL Salesforce] synchronisation {#start-salesforce-sync}

1. Cliquez sur **[!UICONTROL Démarrer la synchronisation Salesforce]** pour lancer la synchronisation persistante Marketo-Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo ne déduplique pas automatiquement les données par rapport à une synchronisation [!DNL Salesforce] ou lorsque vous saisissez manuellement des prospects.

1. Cliquez sur **[!UICONTROL Démarrer la synchronisation]**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Le temps nécessaire pour terminer la synchronisation initiale varie en fonction de la taille et de la complexité de votre base de données.

## Vérifier la synchronisation {#verify-sync}

Marketo fournit des messages de statut pour la synchronisation [!DNL Salesforce] dans la zone Admin. Pour vérifier que la synchronisation fonctionne correctement, procédez comme suit.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**, puis sur **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Le statut de synchronisation est visible dans le coin supérieur droit. L’un des trois messages suivants s’affiche : **[!UICONTROL Dernière synchronisation]**, **[!UICONTROL Synchronisation en cours]** ou **[!UICONTROL Échec]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Vous venez de terminer la configuration de l’une des fonctionnalités les plus puissantes de Marketo, allez-y !

>[!MORELIKETHIS]
>
>* [Installer le package Marketo Sales Insight dans Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Configuration de Marketo Sales Insight dans Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md){target="_blank"}
