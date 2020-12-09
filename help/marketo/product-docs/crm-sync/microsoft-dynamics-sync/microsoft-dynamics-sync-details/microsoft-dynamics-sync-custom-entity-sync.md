---
unique-page-id: 3571846
description: Microsoft Dynamics Sync - Synchronisation des entités personnalisées - Documents marketing - Documentation du produit
title: Microsoft Dynamics Sync -Synchronisation d'entité personnalisée
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---


# Microsoft Dynamics Sync : Synchronisation des entités personnalisées {#microsoft-dynamics-sync-custom-entity-sync}

Si vous devez activer la synchronisation d&#39;entité personnalisée initiale pour rendre les données de Dynamics disponibles dans Marketing, voici comment procéder.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>Pour utiliser un objet personnalisé, il doit être associé à un objet [prospect](microsoft-dynamics-sync-lead-sync.md), [contact](microsoft-dynamics-sync-contact-sync.md)ou [](microsoft-dynamics-sync-account-sync.md)compte dans Dynamics.

>[!CAUTION]
>
>Assurez-vous que la synchronisation initiale est terminée (vous en serez averti par courrier électronique) avant de commencer la synchronisation pour les entités personnalisées.

1. Accédez à la section Admin.

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Cliquez sur **Désactiver la synchronisation** pour désactiver temporairement la synchronisation globale standard.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. Installez une version de Microsoft Dynamics qui prend en charge la synchronisation d&#39;entité personnalisée (après 2_0_0_2). Voir [Versions du module externe Marketo pour Microsoft Dynamics](../../../../product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).
1. Donnez à l’utilisateur de synchronisation marketing l’accès en lecture à toutes les entités que vous prévoyez de synchroniser.
1. Sous Gestion de la base de données, cliquez sur le lien** Dynamics Entities Sync**.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Cliquez sur le lien schéma **de** synchronisation pour rétablir la liste des entités personnalisées disponibles.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Une fois la liste synchronisée, sélectionnez les champs à synchroniser et ceux à utiliser comme [contraintes](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) et/ou déclencheurs dans les listes dynamiques. Lorsque vous avez terminé, cliquez sur **Activer la synchronisation**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. Réactivez la synchronisation globale.

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >Marketo ne prend en charge que les entités personnalisées liées à des entités standard d’un ou deux niveaux.

   >[!NOTE]
   >
   >Les noms d&#39;entité peuvent comporter au maximum** 33 caractères**.

Tu es bon !