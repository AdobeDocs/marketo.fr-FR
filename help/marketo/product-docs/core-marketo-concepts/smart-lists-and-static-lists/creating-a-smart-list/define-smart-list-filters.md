---
unique-page-id: 557316
description: Découvrez comment définir des filtres de liste dynamique. Définissez des contraintes et des valeurs de filtre pour déterminer qui apparaît dans la liste.
title: Définir des filtres pour une liste intelligente
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/gCJT14FtnJaPAMhDUWI7XpoST1lc9yvzZbVKq-oTx-w'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 6%
---
# Définir des filtres pour une liste intelligente {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Rechercher et ajouter des filtres aux listes dynamiques](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Maintenant que vous avez [créé une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} et [ajouté des filtres](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}, définissez les filtres comme suit.

En poursuivant cet exemple, définissez ces filtres pour trouver toutes les personnes en Californie avec un score supérieur à 50.

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/define-smart-list-filters-1.png)

1. Sélectionnez la liste dynamique souhaitée et cliquez sur l’onglet **[!UICONTROL Liste dynamique]**.

   ![](assets/define-smart-list-filters-2.png)

1. Recherchez et sélectionnez « CA » pour le filtre **[!UICONTROL État]**.

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >Il se peut que vous stockiez à la fois « California » et « CA ». Pour filtrer les deux valeurs et inclure _toutes_ les personnes de Californie, apprenez à [ajouter plusieurs valeurs à un filtre de liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Sélectionnez l’opérateur **[!UICONTROL supérieur à]** et saisissez « 50 ».

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>Si vous pensez que certains enregistrements de votre base de données contiennent des adresses e-mail incomplètes (par exemple, « @adobe.com »), utilisez deux filtres d’adresse e-mail lorsque vous utilisez l’opérateur « contains ». Un filtre avec « contient @adobe.com » et un autre avec « contient adobe.com » (sans le symbole @).

Vous savez maintenant comment créer une liste dynamique et ajouter/définir des filtres.
