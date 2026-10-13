---
description: Découvrez comment configurer la synchronisation d’objets personnalisés de Veeva CRM vers Marketo Engage. Activez les objets personnalisés dans Admin et utilisez-les dans les listes dynamiques et les triggers.
title: Synchronisation d’un objet personnalisé
hide: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
TQID: 'https://experienceleague.adobe.com/RmyCIMm3TKbcO3nPcqyZqbWZl1dnJ6Au4HsuURJjcKU'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
    internal-label: Implementation
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
  - id: f141b8e0-5812-4581-b47d-7322a93e7f28
    internal-label: Veeva CRM
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 2%
---
# Synchronisation d’un objet personnalisé {#custom-object-sync}

Les objets personnalisés créés dans votre instance CRM [!DNL Veeva] peuvent également faire partie de Marketo Engage. Voici comment le configurer.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>Pour utiliser un objet personnalisé, il doit être associé à un objet contact ou compte dans [!DNL Veeva] CRM.

## Activer l’objet personnalisé {#enable-custom-object}

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**, puis **[!UICONTROL Synchronisation des objets Veeva]**.

   ![](assets/custom-object-sync-1.png)

1. S&#39;il s&#39;agit de votre premier objet personnalisé, cliquez sur **[!UICONTROL Schéma de synchronisation]**.

   ![](assets/custom-object-sync-2.png)

1. Cliquez sur **[!UICONTROL Désactiver la synchronisation globale]**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >La synchronisation initiale du schéma d’objet personnalisé [!DNL Veeva] peut prendre quelques minutes.

1. Faites glisser l’objet personnalisé que vous souhaitez synchroniser dans la zone de travail.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Les objets personnalisés doivent avoir des noms uniques. Marketo ne prend pas en charge deux objets personnalisés différents portant le même nom.

1. Cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/custom-object-sync-5.png)

1. Cliquez de nouveau sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/custom-object-sync-6.png)

1. Revenez à l’onglet **[!UICONTROL Veeva]**.

   ![](assets/custom-object-sync-7.png)

1. Cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/custom-object-sync-8.png)

1. Pour afficher tous vos [!DNL Veeva] objets personnalisés, cliquez sur **[!UICONTROL Admin]** et **[!UICONTROL Synchronisation des objets Veeva]**.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo ne prend en charge que les entités personnalisées qui sont liées à des entités standard à un ou deux niveaux de profondeur.

Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans les campagnes et listes dynamiques.

>[!MORELIKETHIS]
>
>* [Synchronisation des messages d’appel et de clé d’appel](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [Ajouter/supprimer un champ d’objet personnalisé en tant que liste dynamique/contraintes de déclencheur](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
