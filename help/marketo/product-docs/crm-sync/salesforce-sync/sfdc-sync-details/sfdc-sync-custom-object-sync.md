---
unique-page-id: 2953471
description: Synchronisation SFDC - Synchronisation d’objets personnalisés - Documents marketing - Documentation du produit
title: Synchronisation SFDC -Synchronisation d’objets personnalisés
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Synchronisation SFDC : Synchronisation d’objets personnalisés {#sfdc-sync-custom-object-sync}

Les objets personnalisés créés dans votre instance Salesforce peuvent également faire partie de Marketing Cloud.  Voici comment le configurer.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>Pour utiliser un objet personnalisé, il doit être associé à un objet [prospect](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md) ou [compte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) dans Salesforce.

## Activer l&#39;objet personnalisé {#enable-custom-object}

1. Cliquez sur **Admin** et sur le lien **Salesforce Objects Sync**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. S’il s’agit de votre premier objet personnalisé, cliquez sur **Schéma de synchronisation**.

   ![](assets/rtaimage-2.png)

1. Cliquez sur **Désactiver la synchronisation globale**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Une synchronisation initiale du schéma d&#39;objets personnalisés Salesforce peut prendre quelques minutes.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Faites glisser l’objet personnalisé à synchroniser dans la trame.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Les objets personnalisés doivent avoir des noms uniques. Marketo ne prend pas en charge deux objets personnalisés différents portant le même nom.

1. Cliquez sur **Activer la synchronisation**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Cliquez de nouveau sur **Activer la synchronisation**.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >N&#39;oubliez pas de réactiver votre synchronisation globale !

1. Retournez à l&#39;onglet **Salesforce**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Cliquez sur **Activer la synchronisation**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Pour vue à tous vos objets personnalisés Salesforce, cliquez sur **Admin** et sur le lien **Salesforce Objects Sync** (comme à l&#39;étape 1 ci-dessus).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo ne prend en charge que les entités personnalisées liées à des entités standard d’un ou deux niveaux.

### Eléments suivants : {#whats-next}

[Ajouter/supprimer un champ d&#39;objet personnalisé en tant que contraintes de Liste/déclenchement intelligent](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans des campagnes et des listes intelligentes.
