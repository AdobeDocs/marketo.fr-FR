---
unique-page-id: 1147324
description: Découvrez comment effacer les valeurs de champ dans une étape de flux de campagne intelligente. Supprimez les valeurs des champs de personne ou d’entreprise.
title: Effacer les valeurs des champs
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/57QZb7T-y2JVdNeP4nhTl9PDjIX1S9GcQmRAMJ-53E0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 106
ht-degree: 5%

---

# Effacer les valeurs des champs {#clear-field-values}

[Modifier la valeur des données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) est une bonne chose, mais comment _supprimer_ la valeur complètement ? Bonne question !

1. Dans l’étape de flux, choisissez le champ à effacer et saisissez **[!UICONTROL NULL]** (toutes les majuscules) comme **[!UICONTROL Nouvelle valeur]**.

   ![](assets/clear-field-values-1.png)

1. Une fois l’étape de flux terminée, la valeur du champ que vous avez choisi est effacée.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Si vous laissez la nouvelle valeur vide ou saisissez un ESPACE, le champ n’est pas vraiment vide. Vous devez saisir NULL. N’oubliez pas non plus que les étapes de flux ne peuvent pas être annulées après l’exécution.
