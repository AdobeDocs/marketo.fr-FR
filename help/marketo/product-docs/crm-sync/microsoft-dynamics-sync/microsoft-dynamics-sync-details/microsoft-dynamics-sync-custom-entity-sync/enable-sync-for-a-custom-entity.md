---
unique-page-id: 2953384
description: Activer la synchronisation pour une entité personnalisée - Documents Marketo - Documentation du produit
title: Activer la synchronisation pour une entité personnalisée
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Activer la synchronisation pour une entité personnalisée {#enable-sync-for-a-custom-entity}

Si vous avez besoin que les données d&#39;entité personnalisées de Dynamics soient disponibles dans Marketo, voici comment activer la synchronisation pour elle :

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Lorsque vous activez la synchronisation pour une entité personnalisée, Marketo effectue une synchronisation initiale pour importer toutes les données de l’objet personnalisé.

1. Accédez à la section **Admin**.

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Sélectionnez **Microsoft Dynamics** et cliquez sur **Désactiver la synchronisation**.

   Vous devez désactiver temporairement la synchronisation globale pour activer ou désactiver une entité personnalisée.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. Sous Gestion de la base de données, cliquez sur le lien **Dynamics Entities Sync**.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Cliquez sur le lien **schéma de synchronisation**.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Sélectionnez l&#39;entité à synchroniser, puis cliquez sur **Activer la synchronisation**.

   ![](assets/image2015-11-10-9-3a44-3a35.png)

1. Sélectionnez les champs que vous souhaitez synchroniser ou utiliser en tant que [contraintes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) et/ou déclencheurs dans les listes dynamiques. Lorsque vous avez terminé, cliquez sur **Activer la synchronisation**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

   >[!NOTE]
   >
   >Au cours du processus de synchronisation, vous remarquerez peut-être que l’élément &quot;Dynamic Entities Sync&quot; disparaît de l’arborescence de navigation. Ce comportement est attendu et réapparaîtra une fois la synchronisation terminée.

1. L&#39;entité comporte désormais une coche verte.

   ![](assets/image2014-10-20-14-3a33-3a4.png)

1. N&#39;oubliez pas de réactiver la synchronisation globale !

   ![](assets/image2015-11-10-9-3a48-3a35.png)

Oh oui ! Des trucs puissants.
