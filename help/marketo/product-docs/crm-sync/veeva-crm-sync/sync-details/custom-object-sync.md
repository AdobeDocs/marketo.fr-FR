---
description: Synchronisation d’objets personnalisés - Documents Marketo - Documentation du produit
title: Synchronisation des objets personnalisés
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Synchronisation des objets personnalisés {#custom-object-sync}

Les objets personnalisés créés dans votre instance CRM Veeva peuvent également faire partie de Marketo Engage. Voici comment le configurer.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>Pour utiliser un objet personnalisé, il doit être associé à un objet de contact ou de compte dans le CRM Veeva.

## Activer l’objet personnalisé {#enable-custom-object}

1. Dans Marketo, cliquez sur **Administration**, puis **Synchronisation des objets Veeva**.

   ![](assets/custom-object-sync-1.png)

1. S’il s’agit de votre premier objet personnalisé, cliquez sur **Schéma de synchronisation**.

   ![](assets/custom-object-sync-2.png)

1. Cliquez sur **Désactiver la synchronisation globale**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >La synchronisation initiale du schéma d’objet personnalisé de Veeva peut prendre quelques minutes.

1. Faites glisser l’objet personnalisé que vous souhaitez synchroniser dans la zone de travail.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Les objets personnalisés doivent avoir des noms uniques. Marketo ne prend pas en charge deux objets personnalisés différents portant le même nom.

1. Cliquez sur **Activer la synchronisation**.

   ![](assets/custom-object-sync-5.png)

1. Cliquez sur **Activer la synchronisation** encore une fois.

   ![](assets/custom-object-sync-6.png)

1. Revenez au **Veeva** .

   ![](assets/custom-object-sync-7.png)

1. Cliquez sur **Activer la synchronisation**.

   ![](assets/custom-object-sync-8.png)

1. Pour afficher tous vos objets personnalisés Veeva, cliquez sur Synchronisation des objets Admin et Veeva.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo ne prend en charge que les entités personnalisées liées à des entités standard profondes d’un à deux niveaux.

Excellent ! Vous pouvez désormais utiliser les données de cet objet personnalisé dans les campagnes dynamiques et les listes dynamiques.

>[!MORELIKETHIS]
>
>* [Synchronisation des messages clés d’appel et d’appel](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
>* [Ajouter/Supprimer un champ d’objet personnalisé en tant que contraintes de liste/déclenchement intelligent](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}

