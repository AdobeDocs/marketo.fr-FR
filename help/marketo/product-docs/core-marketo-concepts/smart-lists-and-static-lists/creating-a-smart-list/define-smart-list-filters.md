---
unique-page-id: 557316
description: Définition de filtres de liste dynamique - Documents Marketo - Documentation du produit
title: Définition des filtres de liste dynamique
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Définition des filtres de liste dynamique {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Recherche et ajout de filtres aux listes dynamiques](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Maintenant que vous avez [création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} and [added filters](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} définissez les filtres. Voici comment.

Dans notre exemple, définissez ces filtres pour trouver toutes les personnes en Californie ayant un score supérieur à 50.

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Sélectionnez la liste dynamique, puis cliquez sur le bouton **[!UICONTROL Liste dynamique]** .

   ![](assets/smarlist-choosefilters.png)

1. Recherchez et sélectionnez &quot;CA&quot; pour le **[!UICONTROL État]** filtre.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Vous pouvez stocker &quot;Californie&quot; et &quot;CA&quot;. Pour filtrer les deux valeurs et inclure _all_ des gens de Californie, apprenez à  [ajout de plusieurs valeurs à un filtre Liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Sélectionnez la variable **[!UICONTROL supérieur à]** et saisissez &quot;50&quot;.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Si vous pensez que votre base de données contient des enregistrements qui contiennent des adresses électroniques incomplètes (par exemple, simplement &quot;@adobe.com&quot;), utilisez deux filtres d’adresses électroniques lorsque vous utilisez l’opérateur &quot;contient&quot;. Un filtre avec &quot;contient @adobe.com&quot; et un autre avec &quot;contient adobe.com&quot; (sans le symbole @).

Vous savez maintenant comment créer une liste dynamique et ajouter/définir des filtres.
