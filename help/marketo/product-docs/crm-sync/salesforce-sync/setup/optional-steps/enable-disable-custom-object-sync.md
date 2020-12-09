---
unique-page-id: 4719297
description: Activer/désactiver la synchronisation d'objets personnalisés - Documents marketing - Documentation du produit
title: Activer/désactiver la synchronisation d’objets personnalisés
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Activer/désactiver la synchronisation d’objets personnalisés {#enable-disable-custom-object-sync}

Les objets personnalisés créés dans votre instance Salesforce peuvent également faire partie de Marketing Cloud. Voici comment le configurer.

## Activer/désactiver la synchronisation d’objets personnalisés {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Droits d’administration requis.

1. Cliquez sur **Admin**.

   ** ![](assets/one.png)

   **

1. Dans le menu Gestion de la base de données, cliquez sur **Salesforce** **Objets synchronisés**.

   ![](assets/two-2.png)

1. S’il s’agit de votre premier objet personnalisé, cliquez sur **Synchroniser le schéma.** Sinon, cliquez sur **Actualiser le Schéma** pour vous assurer que vous disposez de la dernière version.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Si votre synchronisation globale est en cours d’exécution, vous devrez la désactiver en cliquant sur **Désactiver la synchronisation globale.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Une synchronisation du schéma d&#39;objets personnalisés Salesforce peut prendre quelques minutes.

1. Cliquez sur **Actualiser le Schéma**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Sélectionnez l’objet à synchroniser, puis cliquez sur **Activer la synchronisation**.

   >[!TIP]
   >
   >Marketo ne peut synchroniser un objet personnalisé que s&#39;il a une relation directe avec l&#39;objet prospect, contact ou compte dans Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Cliquez à nouveau sur **Activer la synchronisation** .

   ** ![](assets/image2014-12-10-10-3a15-3a40.png)

   **

1. Revenez à l’onglet **Salesforce** et cliquez sur **Activer la synchronisation**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Utilisation des objets personnalisés {#using-your-custom-objects}

>[!NOTE]
>
>Vous ne pouvez pas utiliser d’objets personnalisés dans des campagnes dynamiques avec des déclencheurs.

1. Dans votre liste intelligente, faites glisser le pointeur de la souris sur le **filtre** Avec opportunité et définissez cette option sur **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Utilisez ensuite les contraintes de filtre pour restreindre la cible d’action.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans des campagnes et des listes intelligentes.

>[!MORELIKETHIS]
>
>* [Ajouter/supprimer un champ d&#39;objet personnalisé en tant que contraintes de Liste/déclenchement intelligent](add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

>



