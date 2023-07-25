---
description: Étape 3 sur 3 - Connexion de Marketo Engage et de Veeva CRM - Documents Marketo - Documentation du produit
title: Étape 3 sur 3 - Connexion de Marketo Engage et de Veeva CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Étape 3 sur 3 : Connexion à Marketo Engage et Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

Dans cet article, vous allez configurer Marketo Engage pour qu’il se synchronise avec votre instance CRM Veeva configurée. **Salesforce apparaît dans certaines fenêtres contextuelles.** car Veeva CRM est basé sur la plateforme Salesforce.

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : Ajout de champs Marketo à Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Étape 2 sur 3 : Création d’un utilisateur Veeva pour Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>Une seule instance Marketo peut être connectée à une instance CRM Veeva à la fois.

## Connexion à Veeva CRM à l’aide d’OAuth {#connect-to-veeva-crm-using-oauth}

1. Dans Marketo, cliquez sur **Administration**. Sélectionner **CRM** et cliquez sur **Synchronisation avec Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Veillez à [masquer tous les champs dont vous n’avez pas besoin ;](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} dans Marketo à partir de l’utilisateur de synchronisation avant de cliquer sur Champs de synchronisation. Une fois que vous avez cliqué sur Synchroniser les champs, tous les champs visibles par l’utilisateur sont créés dans Marketo de manière permanente et ne peuvent pas être supprimés.

1. Cliquez sur **Connexion avec Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Cochez Sandbox si vous synchronisez un sandbox Marketo avec un sandbox CRM Veeva.

1. Cliquez sur **Confirmation des informations d’identification**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Une fenêtre contextuelle contenant la page de connexion Salesforce s’affiche. Saisissez vos informations d’identification &quot;Utilisateur de synchronisation Marketo&quot;, puis cliquez sur **Connexion**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Saisissez le code de vérification que vous avez reçu par courrier électronique (envoyé par Salesforce) et cliquez sur **Vérifier**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Une fois la vérification effectuée, la page d’accès s’affiche pour demander l’accès. Cliquez sur **Autoriser**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. Dans quelques minutes, une fenêtre contextuelle s’affiche dans la page Marketo. Cliquez sur **Confirmation des informations d’identification**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Démarrer la synchronisation des veeva {#start-veeva-sync}

1. Cliquez sur **Démarrer la synchronisation des veeva** pour commencer la synchronisation CRM Marketo-Veeva persistante.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo ne procède pas automatiquement à la déduplication par rapport à une synchronisation CRM Veeva, ni lorsque vous saisissez manuellement des pistes.

1. Cliquez sur **Démarrer la synchronisation**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>Le temps d’exécution de la synchronisation initiale varie en fonction de la taille et de la complexité de votre base de données.

## Vérifier la synchronisation {#verify-sync}

Marketo fournit des messages d’état pour la synchronisation CRM Veeva dans la zone Admin. Vous pouvez vérifier que la synchronisation fonctionne correctement en procédant comme suit.

1. Dans Marketo, cliquez sur **Administration**, puis **Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. L’état de synchronisation est visible dans le coin supérieur droit. Il affiche l’un des trois messages suivants : Dernière synchronisation, synchronisation en cours ou échec.

>[!MORELIKETHIS]
>
>[Configuration d’objets personnalisés](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
