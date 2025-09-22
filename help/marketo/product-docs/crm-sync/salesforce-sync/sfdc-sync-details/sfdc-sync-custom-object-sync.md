---
unique-page-id: 2953471
description: Synchronisation de SFDC - Synchronisation d’objet personnalisé - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - Synchronisation d’objet personnalisé
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 1%

---

# Synchronisation SFDC : synchronisation d’objet personnalisé {#sfdc-sync-custom-object-sync}

Les objets personnalisés créés dans votre instance [!DNL Salesforce] peuvent également faire partie de Marketo.  Voici comment le configurer.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>Pour utiliser un objet personnalisé, il doit être associé à un objet [prospect](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md) ou [compte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) dans [!DNL Salesforce].

>[!IMPORTANT]
>
>L’utilisateur de la synchronisation Marketo a besoin d’un accès en lecture à l’objet personnalisé pour le répertorier et effectuer une synchronisation sur celui-ci.

## Activer l’objet personnalisé  {#enable-custom-object}

1. Cliquez sur **[!UICONTROL Admin]** et sur le lien **[!UICONTROL Synchronisation des objets Salesforce]**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. S&#39;il s&#39;agit de votre premier objet personnalisé, cliquez sur **[!UICONTROL Schéma de synchronisation]**.

   ![](assets/rtaimage-2.png)

1. Cliquez sur **[!UICONTROL Désactiver la synchronisation globale]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Une synchronisation initiale du schéma d’objet personnalisé [!DNL Salesforce] peut prendre quelques minutes.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Faites glisser l’objet personnalisé que vous souhaitez synchroniser dans la zone de travail.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Les objets personnalisés doivent avoir des noms uniques. Marketo ne prend pas en charge deux objets personnalisés différents portant le même nom.

1. Cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Cliquez de nouveau sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >N’oubliez pas de réactiver votre synchronisation globale.

1. Revenez à l’onglet **[!UICONTROL Salesforce]**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Pour afficher tous vos [!DNL Salesforce] objets personnalisés, cliquez sur **[!UICONTROL Admin]** et sur le lien **[!UICONTROL Synchronisation des objets Salesforce]** (comme à l’étape 1 ci-dessus).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >* Marketo ne prend en charge que les entités personnalisées qui sont liées à des entités standard à un ou deux niveaux de profondeur.
   >
   >* L’arborescence d’objets personnalisés peut afficher le même objet plusieurs fois, en raison de ses connexions directes avec l’un des objets principaux (par exemple, prospects, contacts, comptes ou connexions indirectes par le biais d’objets intermédiaires). Dans ce cas, choisissez l’objet le plus proche de l’objet principal et choisissez-en un seul. Le fait de sélectionner le même objet plusieurs fois peut gêner la synchronisation de cet objet personnalisé.

### Et après ? {#whats-next}

[Ajouter/supprimer un champ d’objet personnalisé en tant que liste dynamique/contraintes de déclencheur](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans les campagnes et listes intelligentes.
