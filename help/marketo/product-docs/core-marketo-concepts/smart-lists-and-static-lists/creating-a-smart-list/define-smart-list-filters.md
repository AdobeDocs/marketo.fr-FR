---
unique-page-id: 557316
description: Définition De Filtres De Liste Dynamique - Documents Marketo - Documentation Du Produit
title: Définir des filtres pour une liste intelligente
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 5%

---

# Définir des filtres pour une liste intelligente {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Rechercher et ajouter des filtres aux listes dynamiques](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Maintenant que vous avez [créé une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} et [ajouté des filtres](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}, définissons les filtres. Voici comment faire.

En poursuivant notre exemple, définissons ces filtres pour trouver toutes les personnes en Californie avec un score supérieur à 50.

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
