---
unique-page-id: 557316
description: Définition de filtres de liste dynamique - Documents Marketo - Documentation du produit
title: Définition des filtres de liste dynamique
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Définition des filtres de liste dynamique {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Création d’une liste dynamique](create-a-smart-list.md)
>* [Recherche et ajout de filtres aux listes dynamiques](find-and-add-filters-to-a-smart-list.md)

Maintenant que vous avez [création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) et [filtres ajoutés](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) définissez les filtres. Voici comment.

Dans notre exemple, définissez ces filtres pour trouver toutes les personnes en Californie ayant un score supérieur à 50.

1. Accédez à **Activités marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Sélectionnez la liste dynamique, puis cliquez sur l’icône **Liste dynamique** .

   ![](assets/smarlist-choosefilters.png)

1. Rechercher et sélectionner **CA** pour le **État** filtre.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Vous pouvez stocker les deux **Californie** et **CA**. Pour filtrer les deux valeurs et inclure _all_ des gens de Californie, apprenez à  [ajout de plusieurs valeurs à un filtre de liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. Sélectionnez la variable **supérieur à** et saisissez **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Si vous pensez que votre base de données contient des enregistrements qui contiennent des adresses électroniques incomplètes (par exemple, simplement &quot;@adobe.com&quot;), utilisez **two** Filtres d’adresses électroniques lorsque vous utilisez l’opérateur &quot;contient&quot;. Un filtre avec &quot;contient @adobe.com&quot; et un autre avec &quot;contient adobe.com&quot; (sans le symbole @).

Vous savez maintenant comment créer une liste dynamique et ajouter/définir des filtres.
