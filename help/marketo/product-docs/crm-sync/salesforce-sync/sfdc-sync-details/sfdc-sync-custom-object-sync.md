---
unique-page-id: 2953471
description: Synchronisation SFDC - Synchronisation d’objets personnalisés - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation d’objet personnalisé
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Synchronisation SFDC : synchronisation d’objet personnalisé {#sfdc-sync-custom-object-sync}

Les objets personnalisés créés dans votre instance Salesforce peuvent également faire partie de Marketo Engage. Voici comment le mettre en place.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>Pour utiliser un objet personnalisé, il doit être associé à un objet [prospect](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"} ou [compte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"} dans Salesforce.

>[!IMPORTANT]
>
>L’utilisateur de synchronisation Marketo doit disposer d’un accès en lecture à l’objet personnalisé pour le répertorier et y effectuer une synchronisation.

## Activer l’objet personnalisé  {#enable-custom-object}

1. Cliquez sur **[!UICONTROL Admin]** et sur le lien **[!UICONTROL Synchronisation des objets Salesforce]** .

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. S’il s’agit de votre premier objet personnalisé, cliquez sur **[!UICONTROL Schéma de synchronisation]**.

   ![](assets/rtaimage-2.png)

1. Cliquez sur **[!UICONTROL Désactiver la synchronisation globale]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Une synchronisation initiale du schéma d’objet personnalisé Salesforce peut prendre quelques minutes.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Faites glisser l’objet personnalisé à synchroniser dans la zone de travail.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Les objets personnalisés doivent avoir des noms uniques. Marketo ne prend pas en charge deux objets personnalisés différents portant le même nom.

1. Cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Cliquez à nouveau sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >N’oubliez pas de réactiver votre synchronisation globale !

1. Revenez à l’onglet **Salesforce** .

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Pour afficher tous vos objets personnalisés Salesforce, cliquez sur **[!UICONTROL Admin]** et sur le lien **[!UICONTROL Synchronisation des objets Salesforce]** (comme à l’étape 1 ci-dessus).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo ne prend en charge que les entités personnalisées liées à des entités standard profondes d’un ou deux niveaux.

### What&#39;s Next : {#whats-next}

[Ajouter/Supprimer un champ d’objet personnalisé en tant que liste dynamique/contraintes de déclenchement](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans les campagnes intelligentes et les listes dynamiques.
