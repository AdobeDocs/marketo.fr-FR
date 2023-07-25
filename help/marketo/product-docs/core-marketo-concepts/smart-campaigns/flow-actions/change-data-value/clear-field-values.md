---
unique-page-id: 1147324
description: Effacer les valeurs de champ - Documents Marketo - Documentation du produit
title: Effacer les valeurs de champ
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Effacer les valeurs de champ {#clear-field-values}

[Modifier la valeur des données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) est génial, mais comment faire _remove_ la valeur complètement ? Bonne question !

1. À l’étape du flux, sélectionnez le champ à effacer et saisissez **NULL** (toutes les majuscules) en tant que **Nouvelle valeur**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boum ! Je parie que tu ne savais pas ça ! Une fois l’étape de flux terminée, la valeur du champ que vous choisissez est effacée.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Si vous laissez la nouvelle valeur vide ou entrez simplement un espace, le champ ne sera pas réellement vide. Vous devez saisir NULL. En outre, n’oubliez pas que les étapes de flux ne peuvent pas être annulées après exécution.
