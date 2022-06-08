---
unique-page-id: 2953471
description: Synchronisation SFDC - Synchronisation d’objets personnalisés - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation d’objet personnalisé
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Synchronisation SFDC : Synchronisation des objets personnalisés {#sfdc-sync-custom-object-sync}

Les objets personnalisés créés dans votre instance Salesforce peuvent également faire partie de Marketo.  Voici comment le mettre en place.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>Pour utiliser un objet personnalisé, il doit être associé à un objet [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)ou [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) dans Salesforce.

## Activer l’objet personnalisé  {#enable-custom-object}

1. Cliquez sur **Administration** et le **Synchronisation des objets Salesforce** lien.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. S’il s’agit de votre premier objet personnalisé, cliquez sur **Schéma de synchronisation**.

   ![](assets/rtaimage-2.png)

1. Cliquez sur **Désactiver la synchronisation globale**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Une synchronisation initiale du schéma d’objet personnalisé Salesforce peut prendre quelques minutes.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Faites glisser l’objet personnalisé que vous souhaitez synchroniser dans la zone de travail.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Les objets personnalisés doivent avoir des noms uniques. Marketo ne prend pas en charge deux objets personnalisés différents portant le même nom.

1. Cliquez sur **Activer la synchronisation**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Cliquez sur **Activer la synchronisation** encore une fois.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >N’oubliez pas de réactiver votre synchronisation globale !

1. Revenez au **Salesforce** .

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Cliquez sur **Activer la synchronisation**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Pour afficher tous vos objets personnalisés Salesforce, cliquez sur **Administration** et le **Synchronisation des objets Salesforce** lien (comme pour l’étape 1 ci-dessus).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo ne prend en charge que les entités personnalisées liées à des entités standard profondes d’un ou deux niveaux.

### What&#39;s Next : {#whats-next}

[Ajouter/Supprimer un champ d’objet personnalisé en tant que contraintes de liste/déclenchement intelligent](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans les campagnes intelligentes et les listes dynamiques.
