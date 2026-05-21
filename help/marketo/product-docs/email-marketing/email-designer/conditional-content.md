---
solution: Marketo Engage
product: marketo
title: Contenu conditionnel
description: Découvrez le contenu conditionnel afin d’afficher un contenu différent par destinataire. Utilisez des règles dans la Designer d’e-mail pour personnaliser les e-mails.
level: Beginner, Intermediate
feature: Email Designer
exl-id: 979ef9db-920f-466f-8c7d-e9de1ee4cf00
TQID: https://experienceleague.adobe.com/MKNaSOXiUYlnS2KNvH2rUQXqeNxvjiIr-OlbJQvtnaA
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: df8eb12b-4f82-491f-acbb-d74012ca5654
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 2%

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

1. La zone de surbrillance devient orange. Sur la gauche, cliquez sur l’icône _Sélectionner la condition_ (![](assets/icon-select-condition.png)) pour définir votre variante.

   ![](assets/conditional-content-3.png){width="700" zoomable="yes"}

1. Sélectionnez le segment souhaité, puis cliquez sur **Sélectionner**.

   ![](assets/conditional-content-4.png)

1. Cliquez sur l’icône _Modifier l’image_ pour remplacer l’image existante pour la variante. Choisissez la source de votre nouvelle image. Dans cet exemple, nous choisissons la bibliothèque _Images et fichiers_ dans notre abonnement Marketo Engage.

   ![](assets/conditional-content-5.png)

1. Sélectionnez l’image appropriée et cliquez sur **Sélectionner**.

   ![](assets/conditional-content-6.png){width="600" zoomable="yes"}

1. La nouvelle image s’affiche. Il est préférable de renommer votre variante pour la rendre plus facile à identifier. Cliquez sur les points de suspension et sélectionnez **Renommer**.

   >[!NOTE]
   >
   >Cliquer sur les points de suspension vous permet également d’afficher la condition définie de la variante, ainsi que de la dupliquer. Si vous disposez de plusieurs variantes, une option de suppression est disponible. Si vous n’avez qu’une seule variante, la manière de la supprimer est de simplement cliquer de nouveau sur l’icône _Activer le contenu conditionnel_ (elle se lira désormais _Désactiver le contenu conditionnel_ lorsque vous passerez la souris dessus).

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
