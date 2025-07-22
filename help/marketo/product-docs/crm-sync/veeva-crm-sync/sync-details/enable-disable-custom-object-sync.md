---
description: Activer/Désactiver La Synchronisation Des Objets Personnalisés - Documents Marketo - Documentation Du Produit
title: Activer/Désactiver La Synchronisation Des Objets Personnalisés
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Activer/Désactiver La Synchronisation Des Objets Personnalisés {#enable-disable-custom-object-sync}

Les objets personnalisés créés dans votre instance CRM [!DNL Veeva] peuvent également faire partie de Marketo Engage. Voici comment le configurer.

## Activer ou désactiver la synchronisation d’objet personnalisé {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**, puis **[!UICONTROL Synchronisation des objets Veeva]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. S&#39;il s&#39;agit de votre premier objet personnalisé, cliquez sur **[!UICONTROL Schéma de synchronisation]**. Si ce n’est pas le cas, cliquez sur **[!UICONTROL Actualiser le schéma]** pour vous assurer que vous disposez de la dernière version.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Si la synchronisation globale est en cours d’exécution, désactivez-la en cliquant sur **[!UICONTROL Désactiver la synchronisation globale]**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >La synchronisation du schéma d’objet personnalisé [!DNL Veeva] peut prendre quelques minutes.

1. Cliquez sur **[!UICONTROL Actualiser le schéma]**.

   ![](assets/enable-disable-custom-object-sync-4.png)

Sélectionnez l’objet à synchroniser et cliquez sur **[!UICONTROL Activer la synchronisation]**.

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo ne peut synchroniser un objet personnalisé que s’il a une relation directe avec l’objet Contact ou Compte dans [!DNL Veeva] CRM.

1. Cliquez de nouveau sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Revenez à l’onglet [!UICONTROL &#x200B; Veeva &#x200B;] et cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Utilisation d’objets personnalisés {#using-your-custom-objects}

>[!NOTE]
>
>Vous ne pouvez pas utiliser d’objets personnalisés dans des campagnes intelligentes avec des déclencheurs.

1. Dans votre [!UICONTROL Liste dynamique], faites glisser sur le filtre « **[!UICONTROL A une opportunité]** » et définissez sur **[!UICONTROL Vrai]**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. Vous pouvez éventuellement utiliser des contraintes de filtre pour limiter le focus.

   ![](assets/enable-disable-custom-object-sync-9.png)

Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans [!UICONTROL Campagnes intelligentes] et [!UICONTROL Listes intelligentes].

>[!MORELIKETHIS]
>
>[Ajouter/supprimer un champ d’objet personnalisé en tant que liste dynamique/contraintes de déclencheur](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
