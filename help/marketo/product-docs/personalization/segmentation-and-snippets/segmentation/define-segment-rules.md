---
unique-page-id: 2359449
description: Définition de règles de segment - Documents Marketo - Documentation du produit
title: Définition de règles de segment
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
feature: Segmentation
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Définition de règles de segment {#define-segment-rules}

La définition de règles de segment vous permet de classer vos personnes en différents groupes mutuellement exclusifs.

>[!PREREQUISITES]
>
>[Créer une segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. Accédez à la **base de données.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Sélectionnez **Segmentation** dans l’arborescence, puis cliquez sur un **segment** particulier.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Cliquez sur **Liste dynamique** et ajoutez des filtres.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Les segments ne prennent actuellement pas en charge les opérateurs _Dans le passé_ et _Dans la période_ sur les filtres. En effet, les segments recherchent uniquement les mises à jour lorsqu’une valeur de données de modification est enregistrée. Ces valeurs sont _et non_ consignées pour les éléments qui changent automatiquement, tels que les champs de formule et les dates. En outre, les opérateurs de dates avec des plages de dates relatives ne sont pas pris en charge, car ils sont calculés au moment de la validation de la segmentation, et non au moment d’une activité de modification de la valeur des données .

   >[!NOTE]
   >
   >Les filtres &quot;Type SFDC&quot; et &quot;Type Microsoft&quot; ne sont actuellement pas pris en charge dans les listes dynamiques de segmentation.

1. Renseignez les valeurs appropriées pour les filtres.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >Le comportement de journalisation des activités des champs Compte peut avoir une incidence sur la qualification. Par conséquent, nous vous déconseillons d’utiliser les champs Compte lors de la définition de règles de segment.

1. Cliquez sur l’onglet **Personnes (Brouillon)** pour afficher les personnes pouvant être incluses dans ce segment.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Accédez à **Actions de segmentation**. Cliquez sur **Approve**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >Le nombre total de segments que vous pouvez créer dans une segmentation dépend du nombre et du type de filtres utilisés, ainsi que de la complexité de la logique de vos segments. Bien que vous puissiez créer jusqu’à 100 segments à l’aide de champs standard, l’utilisation d’autres types de filtres peut accroître la complexité et votre segmentation peut ne pas être approuvée. Voici quelques exemples : champs personnalisés, membres de la liste, champs du propriétaire de piste et étapes des recettes.
   >
   >Si vous recevez un message d’erreur lors de l’approbation et si vous avez besoin d’aide pour réduire la complexité de votre segmentation, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Consultez le tableau de bord pour un aperçu rapide de vos segments dans un graphique circulaire, ainsi que les règles appliquées.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Bon travail ! Ces segments s’avèrent utiles dans de nombreux endroits de Marketo.

>[!NOTE]
>
>Une personne peut être admissible pour différents segments, mais appartient finalement à une seule personne qui dépend de l’ordre de priorité [ des segments](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>L’écran Personnes (Brouillon) affiche toutes les personnes qui remplissent les critères d’appartenance et qui ne sont pas toujours la liste finale des personnes. Approuvez votre segment pour afficher la liste finale.

>[!MORELIKETHIS]
>
>[Approuver une segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
