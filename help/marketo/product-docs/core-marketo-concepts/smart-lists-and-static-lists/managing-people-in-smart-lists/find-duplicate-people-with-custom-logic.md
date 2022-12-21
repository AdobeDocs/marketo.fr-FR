---
unique-page-id: 2952636
description: Recherche de personnes en double avec une logique personnalisée - Documents Marketo - Documentation du produit
title: Recherche de personnes en double avec une logique personnalisée
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 6%

---

# Recherche de personnes en double avec une logique personnalisée {#find-duplicate-people-with-custom-logic}

Marketo dispose d’une liste dynamique système qui détecte les doublons en faisant correspondre leurs adresses électroniques. Si vous souhaitez utiliser un autre champ pour rechercher des doublons avec, voici comment.

>[!PREREQUISITES]
>
>[Création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Accédez au **Activités marketing** zone.

![](assets/ma-2.png)

1. Sélectionnez votre liste dynamique, puis cliquez sur le bouton **Liste dynamique** .

   ![](assets/two-4.png)

1. Recherchez et faites glisser le **Dupliquer les champs** filtre sur la zone de travail.

   ![](assets/three-4.png)

1. Sélectionnez l’une des quatre options disponibles :

   * Adresse e-mail
   * Nom complet
   * Nom
   * Mis à jour à

   >[!NOTE]
   >
   >Tous les champs, à l’exception de l’adresse électronique, sont sensibles à la casse. Ainsi, l’utilisation de &quot;john doe&quot; dans le champ Nom complet _not_ renvoie les résultats pour John Doe.

   ![](assets/four-2.png)

   Fait! Exécutez la liste dynamique pour rechercher les personnes ayant la même valeur dans le champ précédemment sélectionné.
