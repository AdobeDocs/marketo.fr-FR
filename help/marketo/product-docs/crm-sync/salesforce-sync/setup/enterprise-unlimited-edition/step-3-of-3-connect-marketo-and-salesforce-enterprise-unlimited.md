---
unique-page-id: 2360366
description: Étape 3 sur 3 - Connecter Marketo et Salesforce (Entreprise/Illimité) - Documents Marketo - Documentation du produit
title: Étape 3 sur 3 - Connecter Marketo et Salesforce (Entreprise/Illimité)
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: f27e0d42161161347cc4c774853fb04e7ccecb5c
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Étape 3 sur 3 : connecter Marketo et [!DNL Salesforce] (Entreprise/Illimité) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

Dans cet article, vous allez configurer Marketo pour qu’il se synchronise avec l’instance [!DNL Salesforce] configurée.

>[!PREREQUISITES]
>
>* [Étape 1 de 3 : ajouter des champs Marketo à  [!DNL Salesforce] (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Étape 2 sur 3 : création d’un utilisateur  [!DNL Salesforce]  Marketo (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)

## Récupérer le jeton de sécurité de l’utilisateur de synchronisation {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si vous disposez déjà du jeton de sécurité, passez directement à Définition des informations d’identification de l’utilisateur de synchronisation et félicitations pour la préparation !

1. Connectez-vous à [!DNL Salesforce] avec l’utilisateur de synchronisation Marketo, cliquez sur le nom de l’utilisateur de synchronisation, puis sur **[!UICONTROL Mes paramètres]**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Dans la recherche rapide, saisissez « reset » et cliquez sur **[!UICONTROL Réinitialiser mon jeton de sécurité]**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Cliquez sur **[!UICONTROL Réinitialiser le jeton de sécurité]**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   Le jeton de sécurité vous sera envoyé par e-mail.

## Définir les informations d’identification de l’utilisateur de synchronisation {#set-sync-user-credentials}

1. Dans Marketo, accédez à **[!UICONTROL Admin]**, sélectionnez **CRM**, puis cliquez sur **[!UICONTROL Synchroniser avec Salesforce.com]**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Veillez à [masquer tous les champs dont vous n’avez pas besoin](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) dans Marketo à l’utilisateur de synchronisation avant de cliquer sur **[!UICONTROL Synchroniser les champs]**. Une fois que vous avez cliqué sur [!UICONTROL Synchroniser les champs] tous les champs visibles par l’utilisateur sont créés en permanence dans Marketo et ne peuvent pas être supprimés.

1. Saisissez les informations d’identification de l’utilisateur de synchronisation [!DNL Salesforce] créées dans la partie 2 de la configuration [!DNL Salesforce] ([Professionnel](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) ou [Entreprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) et cliquez sur **[!UICONTROL Champs de synchronisation]** (cochez la case **[!UICONTROL Sandbox]** [!DNL Salesforce] uniquement si vous synchronisez un sandbox Marketo avec un autre sandbox).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Si un bouton « Se connecter à [!DNL Salesforce] » s’affiche à la place des champs Nom d’utilisateur/Mot de passe/Jeton, votre abonnement Marketo est activé pour OAuth. Reportez-vous [&#x200B; cet article](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md). Dès que la synchronisation commence à utiliser un ensemble d’informations d’identification, **les informations d’identification [!DNL Salesforce] ou l’abonnement ne changent pas**. Si vous souhaitez utiliser l’authentification de base, contactez votre gestionnaire de compte.

1. Lisez l’avertissement, puis cliquez sur **[!UICONTROL Confirmer les informations d’identification]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si vous souhaitez parcourir les [mappages et les personnaliser](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), c’est votre seule chance de le faire ! Une fois que vous avez cliqué sur [!UICONTROL Démarrer la synchronisation de Salesforce], tout est terminé.

## Démarrer [!DNL Salesforce] synchronisation {#start-salesforce-sync}

1. Cliquez sur **[!UICONTROL Démarrer la synchronisation Salesforce]** pour lancer la synchronisation persistante Marketo-[!DNL Salesforce].

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

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**, puis sur **[!UICONTROL Salesforce]**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Le statut de synchronisation est visible dans le coin supérieur droit. L’un des trois messages suivants s’affiche : **[!UICONTROL Dernière synchronisation]**, **[!UICONTROL Synchronisation en cours]** ou **[!UICONTROL Échec]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Vous venez de terminer la configuration de l’une des fonctionnalités les plus puissantes de Marketo, allez-y !

>[!MORELIKETHIS]
>
>* [Étape 1 de 3 : ajouter des champs Marketo à  [!DNL Salesforce] (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Étape 2 sur 3 : création d’un utilisateur  [!DNL Salesforce]  Marketo (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installer le package Marketo Sales Insight dans [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configuration de Marketo Sales Insight in [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
