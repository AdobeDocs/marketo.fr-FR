---
unique-page-id: 2949413
description: Ajouter une contrainte à un filtre de liste dynamique - Documents Marketo - Documentation du produit
title: Ajout d’une contrainte à un filtre de liste dynamique
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: aeefe7a5c265e3a7ddd50920820742a463ab178a
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Ajout d’une contrainte à un filtre de liste dynamique {#add-a-constraint-to-a-smart-list-filter}

Lors de la création d’une liste dynamique, certains filtres disposent d’options avancées appelées &quot;contraintes&quot;. Il s’agit de conditions supplémentaires que vous pouvez ajouter aux filtres et aux triggers pour affiner encore davantage votre recherche.

Dans cet exemple, ajoutons quelques contraintes à un **[Valeur de données modifiée](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** pour rechercher les personnes qui ont eu un changement d’état de MQL à SQL.

>[!PREREQUISITES]
>
>* [Création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Utilisation du filtre &quot;Valeur de données modifiée&quot; dans une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/ma-1.png)

1. Sélectionnez la liste dynamique avec un filtre auquel vous allez ajouter une contrainte et cliquez sur le bouton **[!UICONTROL Liste dynamique]** .

   ![](assets/two-3.png)

1. Sous **[!UICONTROL Ajouter une contrainte]**, sélectionnez **[!UICONTROL Valeur précédente]**.

   ![](assets/three-3.png)

1. Saisissez le **[!UICONTROL Valeur précédente]**. Dans cet exemple, nous utilisons MQL.

   ![](assets/four-2.png)

1. Sous **[!UICONTROL Ajouter une contrainte]**, sélectionnez **[!UICONTROL Nouvelle valeur]**.

   ![](assets/five.png)

1. Saisissez la nouvelle valeur. Dans cet exemple, nous utilisons SQL.

   ![](assets/six.png)

1. C&#39;est joli ! Cliquez sur le bouton **[!UICONTROL Personnes]** pour voir toutes les personnes qui ont eu un changement d’état de &quot;MQL&quot; à &quot;SQL&quot; au cours des 30 derniers jours.
