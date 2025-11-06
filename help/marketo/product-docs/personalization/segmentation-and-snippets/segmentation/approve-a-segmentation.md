---
unique-page-id: 2359457
description: Approuver une segmentation - Documents Marketo - Documentation du produit
title: Approuver une segmentation
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: b29186ba84ec88be42432e56d1ad0e77c5b43900
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 2%

---

# Approuver une segmentation {#approve-a-segmentation}

Une segmentation doit être approuvée avant de pouvoir être utilisée.

>[!PREREQUISITES]
>
>* [Créer une segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [Définir des règles de segment](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Un maximum de 20 segmentations peut être approuvé à la fois.

1. Accédez à la **[!UICONTROL Base de données]**.

   ![](assets/approve-a-segmentation-1.png)

1. Dans la Segmentation, cliquez sur **[!UICONTROL Actions de segmentation]**, puis sur **[!UICONTROL Approuver]**.

   ![](assets/approve-a-segmentation-2.png)

   >[!NOTE]
   >
   >Le statut passe à _Approbation_ pendant que l’approbation est en cours.

   >[!CAUTION]
   >
   >L&#39;approbation peut prendre de quelques minutes à un jour ou deux, selon la taille de la base de données.

1. Une fois approuvé, le [!UICONTROL Statut] passe de [!UICONTROL Approbation] à [!UICONTROL Approuvé].

   ![](assets/approve-a-segmentation-3.png)

   >[!TIP]
   >
   >Le nombre de personnes dans chaque segment est indiqué entre parenthèses en regard du nom du segment.

1. L’onglet **[!UICONTROL Personnes]** dans le **[!UICONTROL Segment]** affiche désormais la liste finale des personnes du segment.

   ![](assets/approve-a-segmentation-4.png)

>[!CAUTION]
>
>Le nombre total de segments que vous pouvez créer dans une segmentation dépend du nombre et du type de filtres utilisés, ainsi que de la complexité de la logique de vos segments. Bien que vous puissiez créer jusqu’à 100 segments à l’aide de champs standard, l’utilisation d’autres types de filtres peut augmenter la complexité et votre segmentation peut échouer à approuver. Voici quelques exemples : champs personnalisés, membre de la liste, champs du propriétaire du prospect et étapes de chiffre d’affaires.
>
>Si un message d’erreur s’affiche lors de la validation et que vous avez besoin d’aide pour réduire la complexité de votre segmentation, contactez l’assistance de [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Utilisation de filtres de segments dans une liste dynamique](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
