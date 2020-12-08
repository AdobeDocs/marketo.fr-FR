---
unique-page-id: 1146901
description: Utilisation de la logique avancée des règles de Liste intelligente - Documents marketing - Documentation du produit
title: Utilisation de la logique avancée des règles de Liste intelligente
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---


# Utilisation de la logique avancée des règles de Liste intelligente {#using-advanced-smart-list-rule-logic}

Vous pouvez trouver les personnes exactes dont vous avez besoin en appliquant une logique de règle de liste intelligente à plusieurs filtres dans une liste intelligente. Voici comment.

>[!NOTE]
>
>**Conditions préalables**
>
>* [Rechercher et Ajouter des Filtres à une Liste intelligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Définir des Filtres de Liste intelligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)

>



>[!NOTE]
>
>La logique de filtre avancée n’est disponible que si votre liste dynamique comporte au moins trois filtres.

## Ajouter la logique à une Liste intelligente {#add-logic-to-a-smart-list}

Par défaut, votre liste intelligente trouvera les personnes qui correspondent à **TOUS les** filtres (filtres 1 *et* 2 *et* 3). Vous pouvez modifier la logique de règle pour rechercher des personnes qui correspondent à **N&#39;IMPORTE QUEL** des filtres définis (filtres 1 *ou* 2 *ou 3), ou utiliser des filtres avancés (filtres 1* *et 2 *ou *3).*

Dans cet exemple, supposons que vous souhaitiez trouver des personnes en Californie *et* avec un score d&#39;au moins 50 points *ou* avec un statut &quot;Sales Qualified&quot; (Ventes qualifiées).

1. Sélectionnez **Utiliser** des **filtres** **avancés** dans la liste déroulante.

   ![](assets/one.png)

   >[!NOTE]
   >
   >L’utilisation de filtres **avancés** réduit la nécessité de créer des listes intelligentes avec le filtre Membre de la Liste intelligente. Cela permet d’optimiser les performances.

1. La zone de texte **filtres** **avancés** affiche &quot;et&quot; comme valeur par défaut entre tous vos filtres.

   ![](assets/two-2.png)

1. Tapez une paire de parenthèses autour de &quot;2 et 3&quot;.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >Lorsque vous entrez une logique de règle, vous devez utiliser &quot;et&quot; avant &quot;ou&quot;.

1. Remplacez &quot;et&quot; entre &quot;2 et 3&quot; par &quot;ou&quot;.

   ![](assets/four-1.png)

## Utiliser des parenthèses lors du mélange de &quot;Et&quot; et &quot;Ou&quot; {#use-parentheses-when-mixing-and-and-or}

Le mélange des logiques &quot;et&quot; et &quot;ou&quot; requiert des parenthèses pour clarifier votre intention.

![](assets/advancedfilters-parent.png)

## Utiliser des parenthèses imbriquées pour quatre Filtres ou plus si nécessaire {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Selon votre intention, vous devrez peut-être ajouter des parenthèses imbriquées lors de l’utilisation de quatre filtres ou plus.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Si vous entrez une règle non valide, une ligne rouge s&#39;affichera sous la règle. Faites défiler le texte pour afficher le message d’erreur associé.

