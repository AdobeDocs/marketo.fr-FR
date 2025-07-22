---
unique-page-id: 10098379
description: Utilisation de la synchronisation rapide avec Microsoft Dynamics pour un nouveau champ personnalisé - Documents Marketo - Documentation du produit
title: Utilisation de la synchronisation rapide avec Microsoft Dynamics pour un nouveau champ personnalisé
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 1%

---

# Utilisation de la synchronisation rapide avec [!DNL Microsoft Dynamics] pour un nouveau champ personnalisé {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing ou Ventes souhaite un nouveau champ. Ou peut-être en avez-vous oublié un lors de la sélection initiale du champ. Ou vos besoins ont changé. Dans tous les cas, vous pouvez utiliser la synchronisation rapide pour resynchroniser des champs spécifiques.

En règle générale, vous utiliserez la synchronisation rapide pour ajouter un nouveau champ et actualiser les valeurs. Cependant, il existe des cas où vous souhaiteriez synchroniser un champ existant. Vous pouvez restreindre la synchronisation des champs en fonction d’une période mise à jour ou créée. Consultez [Options de synchronisation avancées](#Advanced_Sync_Options) ci-dessous pour plus d’informations.

La synchronisation rapide peut synchroniser les valeurs nulles. Par exemple, si vous utilisez les valeurs A et B et modifiez une valeur B dans [!DNL Dynamics] sur null, la valeur null sera synchronisée sur Marketo.

## Synchronisation rapide pour tous les enregistrements {#quick-sync-for-all-records}

Voici comment utiliser la synchronisation rapide pour resynchroniser de nouveaux champs.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Cliquez sur **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. Dans [!UICONTROL Détails de synchronisation du champ], cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Sélectionnez les champs à synchroniser rapidement et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >Vous pouvez sélectionner des champs à partir de plusieurs entités.

1. Vous recevrez une notification une fois la synchronisation terminée.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >La synchronisation s’exécute côte à côte avec d’autres synchronisations. Selon la taille de la base de données, son exécution peut prendre un certain temps. Lorsqu’un champ est dans la file d’attente pour la synchronisation, vous ne pouvez pas le désélectionner.

## Options de synchronisation avancées {#advanced-sync-options}

Que se passe-t-il si vous souhaitez synchroniser un champ existant, mais uniquement pour un ensemble limité de données ? Voici comment procéder.

1. Décochez la case d’un champ existant. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Ouvrez à nouveau le pop-up et sélectionnez à nouveau le champ.

   ![](assets/select-field-reselect-hand.png)

1. Cliquez sur **[!UICONTROL Synchronisation avancée]**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Choisissez **[!UICONTROL Mise à jour]** et sélectionnez une période à l’aide des sélecteurs de date. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Seuls les enregistrements mis à jour entre le 8/19/16 et le 9/19/16 seront synchronisés rapidement pour ce champ.

## Correction des champs non synchronisés {#fixing-out-of-sync-fields}

Dans les rares cas où un champ [!DNL Dynamics] et Marketo ne sont pas synchronisés, il existe un moyen rapide et facile de les resynchroniser.

1. Désélectionnez le champ et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Sélectionnez à nouveau le champ et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Ça devrait arranger les choses !
