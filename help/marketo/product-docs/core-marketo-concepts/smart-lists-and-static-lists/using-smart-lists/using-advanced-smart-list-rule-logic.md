---
unique-page-id: 1146901
description: Utilisation de la logique avancée des règles de Liste intelligente - Documents marketing - Documentation du produit
title: Utilisation de la logique avancée des règles de Liste intelligente
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Utilisation de la logique de règle de Liste intelligente avancée {#using-advanced-smart-list-rule-logic}

Vous pouvez trouver les personnes exactes dont vous avez besoin en appliquant une logique de règle de liste intelligente à plusieurs filtres dans une liste intelligente. Voici comment.

>[!PREREQUISITES]
>
>* [Rechercher et Ajouter des Filtres à une Liste intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Définir des Filtres de Liste intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)


>[!NOTE]
>
>La logique de filtre avancée n’est disponible que si votre liste dynamique comporte au moins trois filtres.

## Ajouter la logique à une Liste dynamique {#add-logic-to-a-smart-list}

Par défaut, votre liste intelligente trouvera les personnes qui correspondent aux filtres **ALL** (filtres 1 _et_ 2 _et_ 3). Vous pouvez modifier la logique de règle pour rechercher des personnes qui correspondent à **ANY** des filtres définis (filtres 1 _ou_ 2 _ou_ 3), ou utiliser des filtres avancés (filtres 1 _et_ 2 _ou_ 3).

Dans cet exemple, supposons que vous souhaitiez trouver des personnes en Californie _et_ avec un score d&#39;au moins 50 points _ou_ avec le statut &quot;Sales Qualified&quot;.

1. Sélectionnez **Utiliser des filtres avancés** dans la liste déroulante.

   ![](assets/one.png)

   >[!NOTE]
   >
   >L&#39;utilisation de filtres **avancés** réduit la nécessité de créer des listes intelligentes avec le filtre Membre de la Liste intelligente. Cela permet d’optimiser les performances.

1. La zone de texte **filtres avancés** affiche &quot;et&quot; comme valeur par défaut entre tous vos filtres.

   ![](assets/two-2.png)

1. Tapez une paire de parenthèses autour de &quot;2 et 3&quot;.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >Lorsque vous entrez une logique de règle, vous devez utiliser &quot;et&quot; avant &quot;ou&quot;.

1. Remplacez &quot;et&quot; entre &quot;2 et 3&quot; par &quot;ou&quot;.

   ![](assets/four-1.png)

## Utiliser des parenthèses lors du mélange de &quot;Et&quot; et &quot;Ou {#use-parentheses-when-mixing-and-and-or}

Le mélange des logiques &quot;et&quot; et &quot;ou&quot; requiert des parenthèses pour clarifier votre intention.

![](assets/advancedfilters-parent.png)

## Utiliser des parenthèses imbriquées pour quatre Filtres ou plus si nécessaire {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Selon votre intention, vous devrez peut-être ajouter des parenthèses imbriquées lors de l’utilisation de quatre filtres ou plus.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Si vous entrez une règle non valide, une ligne rouge s&#39;affichera sous la règle. Faites défiler le texte pour afficher le message d’erreur associé.
