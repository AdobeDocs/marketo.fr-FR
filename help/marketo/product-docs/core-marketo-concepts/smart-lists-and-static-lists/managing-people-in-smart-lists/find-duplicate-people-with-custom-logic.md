---
unique-page-id: 2952636
description: Recherche de personnes en double avec une logique personnalisée - Documents Marketo - Documentation du produit
title: Recherche de personnes en double avec une logique personnalisée
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 6%

---

# Recherche de personnes en double avec une logique personnalisée {#find-duplicate-people-with-custom-logic}

Marketo Engage dispose d’une liste dynamique système qui détecte les personnes en double en correspondant à leurs adresses électroniques. Si vous souhaitez utiliser un autre champ pour rechercher des doublons avec, voici comment.

>[!PREREQUISITES]
>
>[Création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Accédez au **[!UICONTROL Activités marketing]** zone.

![](assets/ma-2.png)

1. Sélectionnez votre liste dynamique, puis cliquez sur **[!UICONTROL Liste dynamique]** .

   ![](assets/two-4.png)

1. Recherchez et faites glisser le **[!UICONTROL Dupliquer les champs]** filtre sur la zone de travail.

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
