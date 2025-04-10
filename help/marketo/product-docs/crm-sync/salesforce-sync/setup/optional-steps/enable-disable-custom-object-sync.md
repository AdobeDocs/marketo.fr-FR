---
unique-page-id: 4719297
description: Activer/Désactiver La Synchronisation Des Objets Personnalisés - Documents Marketo - Documentation Du Produit
title: Activer/Désactiver La Synchronisation Des Objets Personnalisés
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 6293a11b9d48a20da4cb2448c8374c469679abdb
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Activer/Désactiver La Synchronisation Des Objets Personnalisés {#enable-disable-custom-object-sync}

Les objets personnalisés créés dans votre instance Salesforce peuvent également faire partie de Marketo Engage. Voici comment le configurer.

## Activer/Désactiver La Synchronisation Des Objets Personnalisés {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Dans le menu Gestion de la base de données, cliquez sur **[!UICONTROL Synchronisation des objets Salesforce]**.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. S&#39;il s&#39;agit de votre premier objet personnalisé, cliquez sur **[!UICONTROL Schéma de synchronisation]**. Sinon, cliquez sur **[!UICONTROL Actualiser le schéma]** pour vous assurer que vous disposez de la dernière version.

   ![](assets/enable-disable-custom-object-sync-3.png)

1. Si votre synchronisation globale est en cours d’exécution, vous devez la désactiver en cliquant sur **[!UICONTROL Désactiver la synchronisation globale]**.

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >La synchronisation du schéma d’objet personnalisé Salesforce peut prendre quelques minutes.

1. Cliquez sur **[!UICONTROL Actualiser le schéma]**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Sélectionnez l’objet à synchroniser et cliquez sur **[!UICONTROL Activer la synchronisation]**.

   >[!TIP]
   >
   >Marketo ne peut synchroniser un objet personnalisé que s’il a une relation directe avec l’objet de lead, de contact ou de compte dans Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Cliquez de nouveau sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Revenez à l’onglet **[!DNL Salesforce]** et cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Utilisation d’objets personnalisés {#using-your-custom-objects}

>[!NOTE]
>
>Vous ne pouvez pas utiliser d’objets personnalisés dans des campagnes intelligentes avec des déclencheurs.

1. Dans votre liste dynamique, faites glisser sur le filtre **[!UICONTROL A une opportunité]** et définissez sur **[!UICONTROL true]**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Ensuite, utilisez des contraintes de filtre pour limiter le focus.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans les campagnes et listes dynamiques.

>[!MORELIKETHIS]
>
>[Ajouter/supprimer un champ d’objet personnalisé en tant que liste dynamique/contraintes de déclencheur](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
