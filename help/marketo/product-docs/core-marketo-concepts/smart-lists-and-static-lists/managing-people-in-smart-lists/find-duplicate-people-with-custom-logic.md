---
unique-page-id: 2952636
description: Rechercher des personnes Duplicata avec une logique personnalisée - Docs Marketo - Documentation du produit
title: Rechercher des personnes Duplicata avec une logique personnalisée
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 6%

---

# Rechercher des Duplicata avec une logique personnalisée {#find-duplicate-people-with-custom-logic}

Marketo dispose d&#39;une liste intelligente système qui recherche les duplicata en faisant correspondre leurs adresses électroniques. Si vous voulez utiliser un autre champ pour trouver des duplicata, voici comment.

>[!PREREQUISITES]
>
>[Création d’une Liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Accédez à la zone **Activités marketing**.

![](assets/ma-2.png)

1. Sélectionnez votre liste intelligente, cliquez sur l&#39;onglet **Liste intelligente**.

   ![](assets/two-4.png)

1. Recherchez et faites glisser le filtre **Champs de Duplicata** sur la trame.

   ![](assets/three-4.png)

1. Choisissez l’une des quatre options disponibles :

   * Adresse e-mail
   * Nom complet
   * Nom
   * Mis à jour à

   >[!NOTE]
   >
   >Tous les champs, à l’exception de l’adresse électronique, sont sensibles à la casse. Ainsi, l’utilisation de &quot;john doe&quot; dans le champ Nom complet _ne renvoie pas_ les résultats pour John Doe.

   ![](assets/four-2.png)

   Fait! Exécutez la liste intelligente pour rechercher les personnes ayant la même valeur dans le champ précédemment sélectionné.
