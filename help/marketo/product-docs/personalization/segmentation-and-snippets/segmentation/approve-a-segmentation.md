---
unique-page-id: 2359457
description: Approbation d’une segmentation - Documents Marketo - Documentation du produit
title: Approbation d’une segmentation
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Approbation d’une segmentation {#approve-a-segmentation}

Une segmentation doit être approuvée avant de pouvoir être utilisée.

>[!PREREQUISITES]
>
>* [Création d’une segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [Définition de règles de segment](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>20 segments au maximum peuvent être approuvés à la fois.

1. Accédez au **Base**.

   ![](assets/image2017-3-28-14-3a25-3a49.png)

1. Dans la section Segmentation, cliquez sur **Actions de segmentation**, puis **Approuver**.

   ![](assets/image2017-3-28-14-3a46-3a22.png)

   >[!NOTE]
   >
   >L’état passe à Valider avec une molette ( ![](assets/image2014-9-15-15-3a31-3a43.png)) pendant que l’approbation est en cours.

   >[!CAUTION]
   >
   >Selon la taille de la base de données, la validation peut prendre plusieurs minutes à plus d’une journée.

   Une fois approuvé, le statut passe de Valider à Approuvé.
   ![](assets/image2017-3-28-14-3a46-3a44.png)

   >[!TIP]
   >
   >Le nombre de personnes dans chaque segment est indiqué entre parenthèses en regard du nom du segment.

1. Le **Personnes** dans le **Segment** affiche maintenant la liste finale des personnes pour le segment.

   ![](assets/image2017-3-28-14-3a47-3a10.png)

>[!CAUTION]
>
>Le nombre total de segments que vous pouvez créer dans une segmentation dépend du nombre et du type de filtres utilisés, ainsi que de la complexité de la logique de vos segments. Bien que vous puissiez créer jusqu’à 100 segments à l’aide de champs standard, l’utilisation d’autres types de filtres peut accroître la complexité et votre segmentation peut ne pas être approuvée. Voici quelques exemples : les champs personnalisés, le membre de la liste, les champs du propriétaire de prospect et les étapes de recettes.
>
>Si vous recevez un message d’erreur lors de l’approbation et si vous avez besoin d’aide pour réduire la complexité de votre segmentation, contactez [Prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Utilisation des filtres de segments dans une liste dynamique](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
