---
solution: Marketo Engage
product: marketo
title: Contenu conditionnel
description: Utilisez du contenu conditionnel dans vos e-mails pour afficher le contenu de manière dynamique en fonction du destinataire.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 6f2d3256f3422f1c5054dfd87db3e31c862724a5
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Contenu conditionnel {#conditional-content}

Le contenu conditionnel vous permet de contrôler dynamiquement le contenu vu par chaque audience. Utilisez les Segmentations existantes pour déterminer ce qu’un destinataire voit en fonction de critères prédéfinis.

>[!PREREQUISITES]
>
>Ayez au moins une segmentation [créée](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md) et [approuvée](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md).

## Ajouter du contenu conditionnel {#add-conditional-content}

1. Ouvrez l’e-mail souhaité, puis cliquez sur **Modifier le contenu de l’e-mail**.

   ![](assets/conditional-content-1.png)

1. Sélectionnez le contenu que vous souhaitez rendre conditionnel (dans cet exemple, nous choisissons l’image d’en-tête ). Cliquez sur l’icône _Activer le contenu conditionnel_.

   ![](assets/conditional-content-2.png)

1. La boîte devient orange. Sur la gauche, cliquez sur l’icône _Sélectionner une condition_ pour définir votre variante.

   ![](assets/conditional-content-3.png){width="700" zoomable="yes"}

1. Sélectionnez le segment souhaité, puis cliquez sur **Sélectionner**.

   ![](assets/conditional-content-4.png)

1. Cliquez sur l’icône _Modifier l’image_ pour remplacer l’image existante pour la variante. Choisissez la source de votre nouvelle image. Dans cet exemple, nous choisissons la bibliothèque _Images et fichiers_ dans notre abonnement Marketo Engage.

   ![](assets/conditional-content-5.png)

1. Sélectionnez l’image appropriée et cliquez sur **Sélectionner**.

   ![](assets/conditional-content-6.png){width="600" zoomable="yes"}

1. La nouvelle image s’affiche. Il est préférable de renommer votre variante pour la rendre plus facile à identifier.

   ![](assets/conditional-content-7.png){width="600" zoomable="yes"}

1. Pour ajouter des variantes supplémentaires (facultatif), cliquez sur **Ajouter une variante** et procédez de la même manière.

   ![](assets/conditional-content-8.png)

1. Lorsque vous avez terminé, chaque variante affiche le contenu que vous avez sélectionné.

   ![](assets/conditional-content-9.gif)

1. Les destinataires voient le contenu en fonction des règles définies dans chaque segment. Dans l’exemple ci-dessus, toute personne dont le « football » est répertorié dans votre champ Marketo Engage _Sport favori_ verra l’image de football.

>[!MORELIKETHIS]
>
>* [Définir des règles de segment](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
>* [Créer un champ personnalisé dans Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
