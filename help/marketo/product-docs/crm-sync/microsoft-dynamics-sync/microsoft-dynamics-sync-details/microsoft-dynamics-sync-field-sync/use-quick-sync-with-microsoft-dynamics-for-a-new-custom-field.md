---
unique-page-id: 10098379
description: Utilisation de la synchronisation rapide avec Microsoft Dynamics pour un nouveau champ personnalisé - Documents marketing - Documentation du produit
title: Utiliser la synchronisation rapide avec Microsoft Dynamics pour un nouveau champ personnalisé
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Utiliser la synchronisation rapide avec Microsoft Dynamics pour un nouveau champ personnalisé {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing ou ventes souhaite un nouveau champ. Ou peut-être en avez-vous oublié une dans votre sélection de champ initiale. Ou vos besoins ont changé. Dans tous les cas, vous pouvez utiliser la synchronisation rapide pour resynchroniser des champs spécifiques.

Normalement, vous utiliserez la synchronisation rapide pour ajouter un nouveau champ et actualiser les valeurs. Cependant, il peut arriver que vous souhaitiez synchroniser un champ existant. Vous pouvez limiter la synchronisation des champs en fonction d’une plage de dates mise à jour ou créée. Voir Options [de synchronisation](#Advanced_Sync_Options) avancéesci-dessous pour plus d’informations.

Quick Sync peut synchroniser des valeurs nulles. Par exemple, si vous utilisez les valeurs A et B et que vous modifiez une valeur B dans Dynamics en la définissant sur null, la valeur null sera synchronisée avec Marketo.

## Synchronisation rapide pour tous les enregistrements {#quick-sync-for-all-records}

Voici comment utiliser la synchronisation rapide pour resynchroniser de nouveaux champs.

1. Dans Marketing, cliquez sur **Admin**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Cliquez sur** Microsoft Dynamics**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. Dans Détails de synchronisation des champs, cliquez sur **Modifier**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Sélectionnez les champs à synchroniser rapidement, puis cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >Vous pouvez sélectionner des champs à partir de plusieurs entités.

1. Vous recevrez une notification lorsque la synchronisation sera terminée.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >La synchronisation s’exécute côte à côte avec d’autres synchronisations et, en fonction de la taille de la base de données, il peut s’écouler un certain temps avant qu’elle ne se termine. Lorsqu’un champ se trouve dans une file d’attente pour synchronisation, vous ne pouvez pas le désélectionner.

## Options de synchronisation avancées {#advanced-sync-options}

Que se passe-t-il si vous souhaitez synchroniser un champ existant, mais uniquement pour un ensemble limité de données ? Voici comment.

1. Décochez la case d’un champ existant. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Ouvrez à nouveau la fenêtre contextuelle et sélectionnez à nouveau le champ.

   ![](assets/select-field-reselect-hand.png)

1. Cliquez sur Synchronisation **** avancée.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Sélectionnez **Mise à jour **et sélectionnez une plage de dates à l’aide des sélecteurs de dates. Cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Seuls les enregistrements mis à jour entre le 19/8/16 et le 19/9/16 seront synchronisés rapidement pour le champ.

## Correction des champs non synchronisés {#fixing-out-of-sync-fields}

Dans les rares cas où un champ Dynamics et Marketo ne sont pas synchronisés, il existe un moyen rapide et facile de les resynchroniser.

1. Désélectionnez le champ et cliquez sur **Enregistrer**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Sélectionnez à nouveau le champ, puis cliquez sur **Enregistrer**. C&#39;est tout !

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Ça devrait arranger ça !

