---
unique-page-id: 4719300
description: Ajouter/Supprimer un champ d’objet personnalisé en tant que liste dynamique/contraintes de déclenchement - Documents Marketo - Documentation du produit
title: Ajouter/Supprimer un champ d’objet personnalisé en tant que contraintes de liste/déclenchement intelligent
exl-id: 639e73eb-9a8c-4b10-8e97-892abf5c5db0
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Ajouter/Supprimer un champ d’objet personnalisé en tant que contraintes de liste/déclenchement intelligent {#add-remove-custom-object-field-as-smart-list-trigger-constraints}

Marketo fournit un contrôle de grain fin sur la synchronisation des objets personnalisés Salesforce. Vous pouvez ainsi sélectionner les champs disponibles en tant que contraintes dans les filtres d’objets personnalisés et les utiliser comme déclencheurs dans les campagnes intelligentes.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Cliquez sur **Administrateur.**

   ![](assets/image2014-12-10-13-3a9-3a47.png)

1. Cliquez sur **Administration** puis **Synchronisation des objets Salesforce.**

   ![](assets/image2015-12-11-15-3a11-3a41.png)

1. **Synchronisation des objets Salesforce** apparaît dans la colonne de gauche.

   ![](assets/image2015-12-11-15-3a15-3a15.png)

1. Sélectionnez l’objet que vous souhaitez modifier.

   ![](assets/image2014-12-10-13-3a10-3a11.png)

1. Cliquez sur **Modifier les champs visibles**.

   >[!TIP]
   >
   >Si la variable **Modifier les champs visibles** est grisé, l’objet est actuellement utilisé dans une liste dynamique ou une campagne dynamique. Supprimez toutes les associations pour continuer.

   ![](assets/image2014-12-10-13-3a10-3a25.png)

1. Si votre synchronisation globale est activée, cliquez sur **Désactiver la synchronisation globale**.

   ![](assets/image2014-12-10-13-3a10-3a36.png)

1. Cochez les cases en regard des contraintes de filtre/déclenchement nécessaires, puis cliquez sur **Enregistrer**.

   ![](assets/image2014-12-10-13-3a10-3a47.png)

   >[!NOTE]
   >
   >Tous les champs sont sélectionnés par défaut pour être des contraintes sur les filtres.

1. Cliquez sur le bouton **Champs** pour confirmer vos modifications.

   ![](assets/image2014-12-10-13-3a10-3a56.png)

   >[!NOTE]
   >
   >N’oubliez pas de réactiver votre synchronisation globale !

Waouh ! Maintenant vos listes intelligentes et vos campagnes intelligentes ont encore plus de pouvoir.

>[!MORELIKETHIS]
>
>[Activer/Désactiver la synchronisation d’objets personnalisés](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-custom-object-sync.md)
