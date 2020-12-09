---
unique-page-id: 3571800
description: Étape 3 sur 3 - Connecter Marketo et Salesforce (Professional) - Marketo Docs - Documentation sur les produits
title: Étape 3 sur 3 - Connecter Marketo et Salesforce (Professional)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---


# Étape 3 sur 3 : Connect Marketo and Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

Dans cet article, vous allez configurer Marketo pour qu’il se synchronise avec votre instance Salesforce configurée.

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : Ajouter les champs du marketing à Salesforce (Professional)](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [Étape 2 sur 3 : Créer un utilisateur Salesforce pour Marketo (Professional)](step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)

>



## Récupérer le jeton de sécurité utilisateur de synchronisation {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si vous disposez déjà du jeton de sécurité, passez directement à la section Définition des informations d’identification de l’utilisateur et des félicitations pour la préparation !

1. Connectez-vous à Salesforce avec l’utilisateur synchronisé de Marketo, cliquez sur le nom de l’utilisateur synchronisé, puis sur **Mes paramètres**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Dans la barre de recherche Nav, tapez &quot;reset&quot; et cliquez sur **Réinitialiser mon jeton** de sécurité.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Cliquez sur **Réinitialiser le jeton** de sécurité.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Le jeton de sécurité vous sera envoyé par courrier électronique.

## Définir les informations d’identification utilisateur de synchronisation {#set-sync-user-credentials}

1. Dans Marketo, accédez à **Admin**, sélectionnez **CRM**, puis cliquez sur **Synchroniser avec [Salesforce.com.](http://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >Veillez à [masquer tous les champs dont vous n’avez pas besoin](../../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) dans Marketo de l’utilisateur de synchronisation avant de cliquer sur **Synchroniser les champs**. Une fois que vous avez cliqué sur Synchroniser les champs, tous les champs visibles par l’utilisateur sont créés de manière permanente dans Marketing Cloud et ne peuvent pas être supprimés.

1. Saisissez les informations d’identification de l’utilisateur de synchronisation Salesforce créées dans la partie 2 de la configuration de Salesforce ([Professional](https://community.marketo.com/MarketoArticle?id=kA050000000LJ3QCAW), [Enterprise](https://community.marketo.com/MarketoArticle?id=kA050000000LIwKCAW)) et cliquez sur **Synchroniser les champs**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Cochez **Sandbox** si vous synchronisez un sandbox Marketo avec un sandbox Salesforce.

1. Lisez l’avertissement, puis cliquez sur **Confirmer les informations d’identification**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Si vous souhaitez examiner les [mappages et les](../../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)personnaliser, c&#39;est votre seule chance de le faire ! Une fois que vous avez cliqué sur Début Salesforce Sync, c&#39;est terminé.

## Début Salesforce Sync {#start-salesforce-sync}

1. Cliquez sur **Début Salesforce Sync** pour commencer la synchronisation persistante Marketo-Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo ne dédupliquera pas automatiquement la synchronisation Salesforce ou lorsque vous saisissez manuellement des pistes.

1. Cliquez sur **DÉBUT SYNC**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Le temps nécessaire pour terminer la synchronisation initiale varie en fonction de la taille et de la complexité de votre base de données.

## Vérifier la synchronisation {#verify-sync}

Marketo fournit des messages d’état pour la synchronisation Salesforce dans la zone Admin. Vous pouvez vérifier que la synchronisation fonctionne correctement en procédant comme suit.

1. Dans Marketing, cliquez sur **Admin**, puis sur **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. L’état de synchronisation est visible dans le coin supérieur droit. Il affiche l&#39;un des trois messages suivants : **Dernière synchronisation**, **synchronisation en cours** ou **échec**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Ouah, vous venez de finir de configurer l&#39;une des fonctionnalités les plus puissantes de Marketo, allez-y !

>[!NOTE]
>
>**Articles connexes**
>
>* [Installation du package Marketing Cloud Sales Insight dans l’AppExchange Salesforce](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configuration de Marketo Sales Insight dans Salesforce Professional Edition](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>* [Étapes facultatives](http://docs.marketo.com/display/docs/optional+steps)

>



