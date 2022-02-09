---
unique-page-id: 2953384
description: Activer la synchronisation pour une entité personnalisée - Documents Marketo - Documentation du produit
title: Activation de la synchronisation pour une entité personnalisée
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: dadaf5bd8e887309d0e9ee8fc25fc58d1c4fbe97
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---

# Activation de la synchronisation pour une entité personnalisée {#enable-sync-for-a-custom-entity}

Si vous avez besoin que les données d’entité personnalisées de Dynamics soient disponibles dans Marketo, voici comment activer la synchronisation pour celle-ci.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>* Lorsque vous activez la synchronisation pour une entité personnalisée, Marketo effectue une synchronisation initiale afin d’importer toutes les données de l’objet personnalisé.
>* Les membres de la liste marketing et de la liste marketing sont **non pris en charge** à ce moment-là.


1. Accédez au **Administration** .

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Sélectionner **Microsoft Dynamics** et cliquez sur **Désactiver la synchronisation**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Vous devez désactiver temporairement la synchronisation globale pour activer ou désactiver une entité personnalisée.

1. Sous Gestion de la base de données, cliquez sur le **Synchronisation des entités Dynamics** lien.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Cliquez sur le bouton **Schéma de synchronisation** lien.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Sélectionnez l’entité à synchroniser, puis cliquez sur **Activer la synchronisation**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Sélectionnez les champs que vous souhaitez synchroniser ou utiliser comme [contraintes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) et/ou se déclenchent dans les listes dynamiques. Lorsque vous avez terminé, cliquez sur **Activer la synchronisation**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Au cours du processus de synchronisation, vous pouvez constater que l’élément &quot;Synchronisation des entités dynamiques&quot; disparaît de l’arborescence de navigation. Ce comportement est attendu et réapparaîtra une fois la synchronisation terminée.

1. L’entité comporte désormais une coche verte.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. N’oubliez pas de réactiver la synchronisation globale !

   ![](assets/enable-sync-for-a-custom-entity-8.png)
