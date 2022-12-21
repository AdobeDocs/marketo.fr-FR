---
unique-page-id: 2949413
description: Ajout d’une contrainte à un filtre de liste dynamique - Documents Marketo - Documentation du produit
title: Ajout d’une contrainte à un filtre de liste dynamique
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Ajout d’une contrainte à un filtre de liste dynamique {#add-a-constraint-to-a-smart-list-filter}

Lors de la création de listes dynamiques, certains filtres disposent d’options avancées appelées &quot;contraintes&quot;. Il s’agit de conditions supplémentaires que vous pouvez ajouter aux filtres et aux triggers pour affiner encore davantage votre recherche.

Dans cet exemple, ajoutons quelques contraintes à un **[Valeur de données modifiée](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** pour rechercher les personnes qui ont eu un changement d’état de MQL à SQL.

>[!PREREQUISITES]
>
>* [Création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Utilisation du filtre &quot;Valeur de données modifiée&quot; dans une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)
>


1. Accédez à **Activités marketing**.

   ![](assets/ma-1.png)

1. Sélectionnez la liste dynamique avec un filtre auquel vous allez ajouter une contrainte, puis cliquez sur le bouton **Liste dynamique** .

   ![](assets/two-3.png)

1. Sous **Ajouter une contrainte**, sélectionnez **Valeur précédente**.

   ![](assets/three-3.png)

1. Saisissez le **Valeur précédente**. Dans cet exemple, nous utilisons MQL.

   ![](assets/four-2.png)

1. Sous **Ajouter une contrainte**, sélectionnez **Nouvelle valeur**.

   ![](assets/five.png)

1. Saisissez le **Nouvelle valeur**. Dans cet exemple, nous utilisons SQL.

   ![](assets/six.png)

1. C&#39;est joli ! Cliquez sur le bouton **Personnes** pour afficher toutes les personnes qui ont eu une **État** changer à partir de **MQL** to **SQL** au cours des 30 derniers jours.
