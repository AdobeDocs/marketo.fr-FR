---
unique-page-id: 1146901
description: Utilisation de la logique de règle de liste dynamique avancée - Documents Marketo - Documentation du produit
title: Utilisation de la logique de règle de liste dynamique avancée
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
feature: Smart Lists
source-git-commit: d087b22e84c23fea5e38fe7bf20349dc7eec09f7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Utilisation de la logique de règle de liste dynamique avancée {#using-advanced-smart-list-rule-logic}

Vous pouvez trouver les personnes exactes dont vous avez besoin en appliquant la logique de règle Liste dynamique à plusieurs filtres dans une liste dynamique. Voici comment.

>[!PREREQUISITES]
>
>* [Rechercher et ajouter des filtres à une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}
>* [Définir des filtres de liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md){target="_blank"}

>[!NOTE]
>
>La logique de filtre avancée n’est disponible que s’il existe trois filtres ou plus dans votre liste dynamique.

## Ajouter une logique à une liste dynamique {#add-logic-to-a-smart-list}

Par défaut, votre liste dynamique trouvera les personnes qui correspondent aux filtres **[!UICONTROL ALL]** (filtres 1 _et_ 2 _et_ 3). Vous pouvez modifier la logique de règle pour rechercher les personnes qui correspondent à **[!UICONTROL ANY]** des filtres définis (filtres 1 _ou_ 2 _ou_ 3), ou utiliser des filtres avancés (filtres 1 _et_ 2 _ou_ 3).

Dans cet exemple, supposons que vous souhaitiez trouver des personnes en Californie _et_ avec un score d’au moins 50 points _ou_ avec le statut &quot;Ventes qualifiées&quot;.

1. Sélectionnez **[!UICONTROL Utiliser des filtres avancés]** dans la liste déroulante.

   ![](assets/using-advanced-smart-list-rule-logic-1.png)

   >[!NOTE]
   >
   >L’utilisation de filtres **[!UICONTROL avancés]** réduit la nécessité de créer des listes dynamiques avec le filtre Membre de la liste dynamique. Cela permet d’optimiser les performances.

1. La zone de texte **[!UICONTROL Filtres avancés]** affichera &quot;et&quot; comme valeur par défaut entre tous vos filtres.

   ![](assets/using-advanced-smart-list-rule-logic-2.png)

1. Saisissez une paire de parenthèses autour de &quot;2 et 3&quot;.

   ![](assets/using-advanced-smart-list-rule-logic-3.png)

   >[!CAUTION]
   >
   >Vous devez utiliser &quot;et&quot; avant &quot;ou&quot; lors de la saisie d’une logique de règle.

1. Remplacez &quot;et&quot; entre &quot;2 et 3&quot; par &quot;ou&quot;.

   ![](assets/using-advanced-smart-list-rule-logic-4.png)

## Utiliser des parenthèses lors du mélange de &quot;Et&quot; et &quot;Ou&quot; {#use-parentheses-when-mixing-and-and-or}

Le mélange des logiques &quot;et&quot; et &quot;ou&quot; nécessite des parenthèses pour clarifier votre intention.

![](assets/using-advanced-smart-list-rule-logic-5.png)

## Utilisez des parenthèses imbriquées pour quatre filtres ou plus si nécessaire {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Selon votre intention, vous devrez peut-être ajouter des parenthèses imbriquées lors de l’utilisation de quatre filtres ou plus.

![](assets/using-advanced-smart-list-rule-logic-6.png)

>[!TIP]
>
>Si vous saisissez une règle non valide, une ligne rouge s’affichera sous la règle. Faites défiler le texte pour afficher le message d’erreur associé.
