---
unique-page-id: 2953384
description: Activer la synchronisation pour une entité personnalisée - Documents Marketo - Documentation du produit
title: Activer la synchronisation pour une entité personnalisée
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 4f36194fb76fd8e26c2fd6fe49526d88d355a24a
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Activer la synchronisation pour une entité personnalisée {#enable-sync-for-a-custom-entity}

Si vous avez besoin que les données d’entité personnalisées de [!DNL Dynamics] soient disponibles dans Marketo Engage, voici comment activer la synchronisation de ces données.

>[!PREREQUISITES]
>
>Pour utiliser un objet personnalisé, il doit être associé à un objet [prospect](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md){target="_blank"} ou [compte](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md){target="_blank"} dans Microsoft Dynamics.

>[!NOTE]
>
>* Lorsque vous activez la synchronisation pour une entité personnalisée, Marketo effectue une synchronisation initiale pour importer toutes les données de l’objet personnalisé.
>* Les listes marketing et membres de listes marketing ne sont _pas pris en charge_ pour le moment.

>[!IMPORTANT]
>
>L’utilisateur de la synchronisation Marketo a besoin d’un accès en lecture à l’objet personnalisé pour le répertorier et effectuer une synchronisation sur celui-ci.

1. Accédez à la section **[!UICONTROL Admin]**.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Sélectionnez **[!UICONTROL Microsoft Dynamics]** puis cliquez sur **[!UICONTROL Désactiver la synchronisation]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Vous devez désactiver temporairement la synchronisation globale pour activer ou désactiver une entité personnalisée.

1. Sous [!UICONTROL Gestion de la base de données], cliquez sur le lien **[!UICONTROL Synchronisation des entités Dynamics]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Cliquez sur le lien **[!UICONTROL Schéma de synchronisation]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Sélectionnez l’entité à synchroniser, puis cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Sélectionnez les champs que vous souhaitez synchroniser ou utiliser comme [contraintes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) et/ou déclencheurs dans les listes dynamiques. Lorsque vous avez terminé, cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Pendant le processus de synchronisation, vous remarquerez peut-être que l’élément « [!UICONTROL Synchronisation des entités dynamiques] » disparaît de l’arborescence de navigation. Ce comportement est prévu et il réapparaîtra une fois la synchronisation terminée.

1. L’entité dispose désormais d’une coche verte.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. N’oubliez pas de réactiver la synchronisation globale.

   ![](assets/enable-sync-for-a-custom-entity-8.png)

   >[!NOTE]
   >
   >* Marketo ne prend en charge que les entités personnalisées qui sont liées à des entités standard à un ou deux niveaux de profondeur.
   >
   >* L’arborescence d’objets personnalisés peut afficher le même objet plusieurs fois, en raison de ses connexions directes avec l’un des objets principaux (par exemple, prospects, contacts, comptes ou connexions indirectes par le biais d’objets intermédiaires). Dans ce cas, choisissez l’objet le plus proche de l’objet principal et choisissez-en un seul. Le fait de sélectionner le même objet plusieurs fois peut gêner la synchronisation de cet objet personnalisé.
