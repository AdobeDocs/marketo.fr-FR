---
unique-page-id: 2952636
description: Rechercher des personnes en double avec une logique personnalisée - Documents Marketo - Documentation du produit
title: Rechercher des personnes en double avec la logique personnalisée
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Rechercher des personnes en double avec la logique personnalisée {#find-duplicate-people-with-custom-logic}

Marketo Engage dispose d’une liste dynamique système qui détecte les doublons en faisant correspondre leurs adresses e-mail. Si vous souhaitez utiliser un autre champ pour rechercher des doublons, procédez comme suit.

>[!PREREQUISITES]
>
>[Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Accédez à la zone **[!UICONTROL Activités marketing]**.

![](assets/ma-2.png)

1. Sélectionnez votre liste dynamique, puis cliquez sur l’onglet **[!UICONTROL Liste dynamique]**.

   ![](assets/two-4.png)

1. Recherchez et faites glisser le filtre **[!UICONTROL Champs en double]** sur la zone de travail.

   ![](assets/three-4.png)

1. Choisissez l’une des quatre options disponibles :

   * [!UICONTROL Adresse électronique]
   * [!UICONTROL Nom complet]
   * [!UICONTROL Nom]
   * [!UICONTROL Mise À Jour Le]

   >[!NOTE]
   >
   >Tous les champs, à l’exception de Adresse e-mail, sont sensibles à la casse. Ainsi, l’utilisation de « john doe » dans le champ Nom complet _renvoie pas_ résultats pour John Doe.

   ![](assets/four-2.png)

   Terminé ! Exécutez la liste dynamique pour rechercher des personnes ayant la même valeur dans le champ précédemment sélectionné.
