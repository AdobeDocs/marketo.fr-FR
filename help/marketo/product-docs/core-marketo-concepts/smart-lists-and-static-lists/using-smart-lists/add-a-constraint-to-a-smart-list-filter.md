---
unique-page-id: 2949413
description: Ajouter une contrainte à un filtre de liste dynamique - Documents Marketo - Documentation du produit
title: Ajouter une contrainte à un filtre de liste intelligente
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 9%

---

# Ajouter une contrainte à un filtre de liste intelligente {#add-a-constraint-to-a-smart-list-filter}

Lors de la création d’une liste dynamique, certains filtres disposent d’options avancées appelées « contraintes ». Ce sont des conditions supplémentaires que vous pouvez ajouter aux filtres et aux déclencheurs pour vous aider à affiner davantage votre recherche.

Dans cet exemple, ajoutons des contraintes à un filtre **[Valeur des données modifiées](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** pour rechercher les personnes dont le statut a été modifié de MQL à SQL.

>[!PREREQUISITES]
>
>* [Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Utilisation du filtre « Valeur des données modifiée » dans une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. Sélectionnez la liste dynamique avec un filtre auquel vous allez ajouter une contrainte, puis cliquez sur l&#39;onglet **[!UICONTROL Liste dynamique]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. Sous **[!UICONTROL Ajouter une contrainte]**, sélectionnez **[!UICONTROL Valeur précédente]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. Saisissez la **[!UICONTROL Valeur précédente]**. Dans cet exemple, nous utilisons MQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. Sous **[!UICONTROL Ajouter une contrainte]**, sélectionnez **[!UICONTROL Nouvelle valeur]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. Saisissez la nouvelle valeur. Dans cet exemple, nous utilisons SQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. Bien joué ! Cliquez sur l’onglet **[!UICONTROL Personnes]** pour afficher toutes les personnes dont le statut est passé de « MQL » à « SQL » au cours des 30 derniers jours.
