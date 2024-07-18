---
unique-page-id: 557316
description: Définition de filtres de liste dynamique - Documents Marketo - Documentation du produit
title: Définition des filtres de liste dynamique
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Définition des filtres de liste dynamique {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Rechercher et ajouter des filtres aux listes dynamiques](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Maintenant que vous avez [ créé une liste dynamique ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} et [ ajouté des filtres](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}, définissons les filtres. Voici comment.

Dans notre exemple, définissez ces filtres pour trouver toutes les personnes en Californie ayant un score supérieur à 50.

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/define-smart-list-filters-1.png)

1. Sélectionnez la liste dynamique souhaitée et cliquez sur l’onglet **[!UICONTROL Liste dynamique]** .

   ![](assets/define-smart-list-filters-2.png)

1. Recherchez et sélectionnez &quot;CA&quot; pour le filtre **[!UICONTROL State]**.

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >Vous pouvez stocker &quot;Californie&quot; et &quot;CA&quot;. Pour filtrer les deux valeurs et inclure _tous_ les habitants de Californie, apprenez à [ajouter plusieurs valeurs à un filtre de liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Sélectionnez l’opérateur **[!UICONTROL supérieur à]** et saisissez &quot;50&quot;.

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>Si vous pensez que votre base de données contient des enregistrements qui contiennent des adresses électroniques incomplètes (par exemple, simplement &quot;@adobe.com&quot;), utilisez deux filtres d’adresses électroniques lorsque vous utilisez l’opérateur &quot;contient&quot;. Un filtre avec &quot;contient @adobe.com&quot; et un autre avec &quot;contient adobe.com&quot; (sans le symbole @).

Vous savez maintenant comment créer une liste dynamique et ajouter/définir des filtres.
