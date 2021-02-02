---
unique-page-id: 2360366
description: Étape 3 sur 3 - Connecter Marketo et Salesforce (Enterprise/Unlimited) - Marketo Docs - Documentation du produit
title: Étape 3 sur 3 - Connecter Marketo et Salesforce (Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---


# Étape 3 sur 3 : Connectez Marketo et Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

Dans cet article, vous allez configurer Marketo pour qu’il se synchronise avec votre instance Salesforce configurée.

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : Ajouter les champs du marketing à Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Étape 2 sur 3 : Créer un utilisateur Salesforce pour Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)


## Récupérer le jeton de sécurité utilisateur de synchronisation {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si vous disposez déjà du jeton de sécurité, passez directement à la section Définition des informations d’identification de l’utilisateur et des félicitations pour la préparation !

1. Connectez-vous à Salesforce avec l’utilisateur synchronisé de Marketo, cliquez sur le nom de l’utilisateur synchronisé, puis **Mes paramètres**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Dans la recherche rapide, tapez &quot;reset&quot; et cliquez sur **Réinitialiser mon jeton de sécurité**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Cliquez sur **Réinitialiser le jeton de sécurité**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   Le jeton de sécurité vous sera envoyé par courrier électronique.

## Configurer les informations d&#39;identification utilisateur de synchronisation {#set-sync-user-credentials}

1. Dans Marketo, accédez à **Admin**, sélectionnez **CRM**, puis cliquez sur **Synchroniser avec [Salesforce.com](http://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Veillez à [masquer tous les champs dont vous n’avez pas besoin](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) dans Marketo de l’utilisateur de synchronisation avant de cliquer sur **Synchroniser les champs**. Une fois que vous avez cliqué sur Synchroniser les champs, tous les champs visibles par l’utilisateur sont créés de manière permanente dans Marketing Cloud et ne peuvent pas être supprimés.

1. Saisissez les informations d’identification de l’utilisateur de synchronisation Salesforce créées dans la partie 2 de la configuration Salesforce ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) et cliquez sur **Synchroniser les champs**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Cochez **Sandbox** si vous synchronisez un sandbox Marketo vers un sandbox Salesforce.

1. Lisez l’avertissement, puis cliquez sur **Confirmer les informations d’identification**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si vous souhaitez examiner les [mappages et les personnaliser](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), c&#39;est votre seule chance de le faire ! Une fois que vous avez cliqué sur Début Salesforce Sync, c&#39;est terminé.

## Début de la synchronisation Salesforce {#start-salesforce-sync}

1. Cliquez sur **Début Salesforce Sync** pour commencer la synchronisation persistante Marketo-Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo ne dédupliquera pas automatiquement la synchronisation Salesforce ou lorsque vous saisissez manuellement des pistes.

1. Cliquez sur **Début Sync**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Le temps nécessaire pour terminer la synchronisation initiale varie en fonction de la taille et de la complexité de votre base de données.

## Vérifier la synchronisation {#verify-sync}

Marketo fournit des messages d’état pour la synchronisation Salesforce dans la zone Admin. Vous pouvez vérifier que la synchronisation fonctionne correctement en procédant comme suit.

1. Dans Marketo, cliquez sur **Admin**, puis sur **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. L’état de synchronisation est visible dans le coin supérieur droit. Il affiche l&#39;un des trois messages suivants : **Dernière synchronisation**, **Synchronisation en cours** ou **Échec**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Ouah, vous venez de finir de configurer l&#39;une des fonctionnalités les plus puissantes de Marketo, allez-y !

>[!MORELIKETHIS]
>
>* [Étape 1 sur 3 : Ajouter les champs du marketing à Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Étape 2 sur 3 : Créer un utilisateur Salesforce pour Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installation du package Marketing Cloud Sales Insight dans l’AppExchange Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

