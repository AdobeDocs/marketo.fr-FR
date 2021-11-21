---
unique-page-id: 2359449
description: Définition de règles de segment - Documents Marketo - Documentation du produit
title: Définition de règles de segment
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
source-git-commit: 4699b17a670655820946cd277adf28f2233f04d3
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Définition de règles de segment {#define-segment-rules}

La définition de règles de segment vous permet de classer vos personnes en différents groupes mutuellement exclusifs.

>[!PREREQUISITES]
>
>[Création d’une segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. Accédez au **Base de données.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Sélectionner **Segmentation** dans l’arborescence, puis cliquez sur un **Segment**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Cliquez sur **Liste dynamique** et ajoutez des filtres.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Les segments ne sont actuellement pas pris en charge _Dans le passé_ et _Dans la période_  sur les filtres. En effet, les segments recherchent uniquement les mises à jour lorsqu’une valeur de données de modification est enregistrée. Ces valeurs sont les suivantes : _not_ consignés pour les éléments qui changent automatiquement, tels que les champs de formule et les dates. En outre, les opérateurs de dates avec des plages de dates relatives ne sont pas pris en charge, car ils sont calculés au moment de la validation de la segmentation, et non au moment d’une activité de modification de la valeur des données .

   >[!NOTE]
   >
   >Les filtres &quot;Type SFDC&quot; et &quot;Type Microsoft&quot; ne sont actuellement pas pris en charge dans les listes dynamiques de segmentation.

1. Renseignez les valeurs appropriées pour les filtres.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >Nous vous conseillons _against_ l’utilisation des champs Compte lors de la définition de règles de segment, car cela peut entraîner des problèmes de journalisation des activités.

1. Cliquez sur le bouton **Personnes (version préliminaire)** pour afficher les personnes qui peuvent être incluses dans ce segment.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Accédez à **Actions de segmentation**. Cliquez sur **Approuver**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >Le nombre total de segments que vous pouvez créer dans une segmentation dépend du nombre et du type de filtres utilisés, ainsi que de la complexité de la logique de vos segments. Bien que vous puissiez créer jusqu’à 100 segments à l’aide de champs standard, l’utilisation d’autres types de filtres peut accroître la complexité et votre segmentation peut ne pas être approuvée. Voici quelques exemples : les champs personnalisés, le membre de la liste, les champs du propriétaire de prospect et les étapes de recettes.
   >
   >Si vous recevez un message d’erreur lors de l’approbation et si vous avez besoin d’aide pour réduire la complexité de votre segmentation, contactez [Prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Consultez le tableau de bord pour un aperçu rapide de vos segments dans un graphique circulaire, ainsi que les règles appliquées.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Bon travail ! Ces segments s’avèrent utiles dans de nombreux endroits de Marketo.

>[!NOTE]
>
>Une personne peut être admissible pour différents segments, mais appartient à une seule personne qui dépend de la variable [ordre de priorité des segments](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>L’écran Personnes (Brouillon) affiche toutes les personnes qui remplissent les critères d’appartenance et qui ne sont pas toujours la liste finale des personnes. Approuvez votre segment pour afficher la liste finale.

>[!MORELIKETHIS]
>
>[Approbation d’une segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
