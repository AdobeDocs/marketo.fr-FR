---
unique-page-id: 2949413
description: Ajouter une contrainte à un filtre de Liste dynamique - Documents marketing - Documentation du produit
title: Ajouter une contrainte à un filtre de Liste dynamique
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---


# Ajouter une contrainte à un filtre de Liste dynamique {#add-a-constraint-to-a-smart-list-filter}

Lors de la création de listes intelligentes, certains filtres disposent d’options avancées appelées &quot;contraintes&quot;. Il s’agit de conditions supplémentaires que vous pouvez ajouter aux filtres et aux déclencheurs afin de mieux cibler votre recherche.

Dans cet exemple, ajoutons quelques contraintes à un filtre **[Valeur de données modifiée](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** pour trouver les personnes qui ont subi un changement d&#39;état de MQL à SQL.

>[!PREREQUISITES]
>
>* [Création d’une Liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Utiliser le filtre &quot;Valeur des données modifiée&quot; dans une Liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. Accédez à **Activités marketing**.

   ![](assets/ma-1.png)

1. Sélectionnez la liste intelligente avec un filtre auquel vous allez ajouter une contrainte, puis cliquez sur l&#39;onglet **Liste dynamique**.

   ![](assets/two-3.png)

1. Sous **Ajouter la contrainte**, sélectionnez **Valeur précédente**.

   ![](assets/three-3.png)

1. Saisissez la **Valeur précédente**. Dans cet exemple, nous utilisons MQL.

   ![](assets/four-2.png)

1. Sous **Ajouter la contrainte**, sélectionnez **Nouvelle valeur**.

   ![](assets/five.png)

1. Saisissez la **Nouvelle valeur**. Dans cet exemple, nous utilisons SQL.

   ![](assets/six.png)

1. Bien joué ! Cliquez sur l&#39;onglet **Personnes** pour afficher toutes les personnes qui ont subi une modification **Status** de **MQL** à **SQL** au cours des 30 derniers jours.
