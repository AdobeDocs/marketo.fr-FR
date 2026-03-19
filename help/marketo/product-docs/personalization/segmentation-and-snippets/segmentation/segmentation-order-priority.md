---
unique-page-id: 2359500
description: Découvrez la priorité de l’ordre de segmentation et comment elle détermine le segment auquel appartient une personne. Modifier l’ordre des segments dans la base de données pour contrôler l’évaluation des segments
title: Ordre de priorité des segmentations
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
source-git-commit: 80b39eb99cdaacf4c9655aa175da3d22548dcca6
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 4%

---

# Ordre de priorité des segmentations {#segmentation-order-priority}

Il est important de comprendre comment **ordre** définit la priorité de l’évaluation de vos personnes dans une segmentation.

>[!PREREQUISITES]
>
>[Créer une segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>[Définissez Des Règles De Segment](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Vous pouvez uniquement modifier une segmentation en mode brouillon.

1. Accédez à la **Base de données**.

   ![](assets/segmentation-order-priority-1.png)

1. Sélectionnez votre **Segmentation**. Dans **[!UICONTROL Actions de segmentation]**, cliquez sur **[!UICONTROL Modifier les segments]**.

   ![](assets/segmentation-order-priority-2.png)

   Vous pouvez vérifier ou modifier l’ordre de vos segments à partir de cet écran.

   ![](assets/segmentation-order-priority-3.png)

>[!NOTE]
>
>* Les segments s’excluent mutuellement. Une personne ne peut être membre que d’un seul segment à la fois.
>* Lorsqu’une personne est admissible pour deux segments, elle n’appartiendra qu’au premier de la liste.
>* Si une personne n’est éligible à aucun segment, elle deviendra membre du segment par défaut.
