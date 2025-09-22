---
unique-page-id: 1147324
description: Effacer les valeurs de champ - Documents Marketo - Documentation du produit
title: Effacer les valeurs des champs
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '95'
ht-degree: 6%

---

# Effacer les valeurs des champs {#clear-field-values}

[Modifier la valeur des données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) est une bonne chose, mais comment _supprimer_ la valeur complètement ? Bonne question !

1. Dans l’étape de flux, choisissez le champ à effacer et saisissez **[!UICONTROL NULL]** (toutes les majuscules) comme **[!UICONTROL Nouvelle valeur]**.

   ![](assets/clear-field-values-1.png)

1. Une fois l’étape de flux terminée, la valeur du champ que vous avez choisi est effacée.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Si vous laissez la nouvelle valeur vide ou si vous entrez simplement un ESPACE, le champ n’est pas vraiment vide. Vous devez saisir NULL. N’oubliez pas non plus que les étapes de flux ne peuvent pas être annulées après l’exécution.
