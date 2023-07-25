---
unique-page-id: 4719297
description: Activer/Désactiver la synchronisation d’objets personnalisés - Documents Marketo - Documentation du produit
title: Activer/Désactiver la synchronisation d’objets personnalisés
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Activer/Désactiver la synchronisation d’objets personnalisés {#enable-disable-custom-object-sync}

Les objets personnalisés créés dans votre instance Salesforce peuvent également faire partie de Marketo. Voici comment le mettre en place.

## Activer/Désactiver la synchronisation d’objets personnalisés {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Droits d’administrateur requis.

1. Cliquez sur **Administration**.

   ![](assets/one.png)

1. Dans le menu Gestion de la base de données, cliquez sur **Synchronisation des objets Salesforce**.

   ![](assets/two-2.png)

1. S’il s’agit de votre premier objet personnalisé, cliquez sur **Schéma de synchronisation.** Sinon, cliquez sur **Actualiser le schéma** pour vous assurer que vous disposez des dernières fonctionnalités.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Si votre synchronisation globale est en cours d’exécution, vous devrez la désactiver en cliquant sur **Désactivez la synchronisation globale.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Une synchronisation du schéma d’objet personnalisé Salesforce peut prendre quelques minutes.

1. Cliquez sur **Actualiser le schéma**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Sélectionnez l’objet que vous souhaitez synchroniser, puis cliquez sur **Activer la synchronisation**.

   >[!TIP]
   >
   >Marketo ne peut synchroniser un objet personnalisé que s’il entretient une relation directe avec l’objet Lead, Contact ou Account de Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Cliquez sur **Activer la synchronisation** encore une fois.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Revenez au **Salesforce** et cliquez sur **Activer la synchronisation**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Utilisation des objets personnalisés {#using-your-custom-objects}

>[!NOTE]
>
>Vous ne pouvez pas utiliser d’objets personnalisés dans des campagnes dynamiques avec des déclencheurs.

1. Dans votre liste dynamique, faites glisser le pointeur de la souris sur l’objet **A une opportunité** filtrer et définir sur **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Ensuite, utilisez les contraintes de filtre pour limiter la cible d’action.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans les campagnes intelligentes et les listes dynamiques.

>[!MORELIKETHIS]
>
>[Ajouter/Supprimer un champ d’objet personnalisé en tant que contraintes de liste/déclenchement intelligent](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
