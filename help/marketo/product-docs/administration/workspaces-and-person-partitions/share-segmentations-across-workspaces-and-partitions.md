---
unique-page-id: 7515767
description: Partage de segments entre espaces de travail et partitions - Documents Marketo - Documentation du produit
title: Partage de segments entre espaces de travail et partitions
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
feature: Partitions, Workspaces
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Partage de segments entre espaces de travail et partitions {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Cet article s’adresse uniquement aux clients qui disposent d’espaces de travail et de partitions.

## Qu’est-ce qu’une segmentation ? {#whats-a-segmentation}

Marketo est doué pour choisir les personnes appropriées pour un programme ou une campagne intelligente. Toutefois, pour des personnages plus permanents, vous devez utiliser des segments. Ils sont nécessaires pour utiliser du contenu dynamique avancé dans Marketo.

>[!NOTE]
>
>Découvrez [comment créer des segments](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Une fois ces personnages configurés (_et_ que vous utilisez des espaces de travail), vous souhaiterez les partager dans vos espaces de travail. Voici quelques bonnes choses à savoir :

## Règles et conseils {#rules-tips}

* Chaque abonnement Marketo peut contenir jusqu’à 20 segments &quot;totaux&quot; sur plusieurs espaces de travail (**et non 20 par espace de travail**).
* Vous pouvez uniquement partager une segmentation avec les espaces de travail auxquels vous avez accès.
* Veillez à créer et à utiliser un **espace de travail par défaut ayant une visibilité sur toutes les partitions**.

* Le traitement de la segmentation s’exécute uniquement sur les personnes de l’espace de travail dans lequel la segmentation est créée.

   * Créez la segmentation que vous souhaitez partager dans le Workspace par défaut.
      * Approuver la segmentation
      * L’espace de travail partagé voit un dossier verrouillé et la segmentation est en lecture seule.
      * La version partagée ne peut pas être modifiée. Vous ne pouvez modifier que la segmentation d’origine dans laquelle elle a été créée.

   * Lorsque vous cliquez sur un segment (par exemple, Health Care) dans une segmentation partagée, les personnes que vous voyez ne seront que des personnes dans la partition associée à l’espace de travail que vous visualisez.
      * Si vous créez une Segmentation dans Workspace 1 (WS1) et la partagez avec WS2 et WS1 n’a pas accès à la partition pour WS2, la segmentation NE SERA PAS recalculée.
      * Si vous créez une Segmentation dans un espace de travail qui comporte des partitions limitées, puis que vous la partagez avec un autre espace de travail, cet espace de travail qui a reçu la Segmentation partagée ne voit les personnes que si elles se chevauchent.

>[!NOTE]
>
>Certaines de ces règles sont un peu complexes. Le moyen le plus simple de commencer est de tester avec des personnes spécifiques. Vous pouvez toujours créer de nouvelles segments et vous débarrasser des anciens.

## Exemples de scénarios {#example-scenarios}

![](assets/share-segmentations-across-workspaces-and-partitions-1.png)

![](assets/share-segmentations-across-workspaces-and-partitions-2.png)

## Partager une segmentation {#share-a-segmentation}

1. Accédez à la **[!UICONTROL base de données]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-3.png)

1. Cliquez avec le bouton droit de la souris sur **[!UICONTROL Segmentations]** et sélectionnez **[!UICONTROL Nouveau dossier]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-4.png)

1. Nommez le dossier que vous allez partager dans les espaces de travail (par exemple : Partager les segments) et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-5.png)

1. Déplacez la ou les segmentation que vous souhaitez partager dans le dossier .

   ![](assets/share-segmentations-across-workspaces-and-partitions-6.png)

1. Cliquez avec le bouton droit sur le dossier et sélectionnez **[!UICONTROL Partager le dossier]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-7.png)

1. Sélectionnez le ou les espaces de travail avec lesquels vous souhaitez partager le dossier. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-8.png)

   >[!NOTE]
   >
   >La boîte de dialogue affiche les espaces de travail que vous êtes autorisé à afficher. C’est pourquoi Marketo recommande de créer et de partager des segments à partir de l’espace de travail par défaut, qui ont une visibilité sur tous les espaces de travail et partitions.

Le dossier d’origine s’affiche dans l’arborescence de la base de données avec une flèche indiquant qu’il est partagé avec d’autres espaces de travail. Depuis l’espace de travail partagé, le dossier s’affiche avec un cadenas pour indiquer que le contenu du dossier a été partagé depuis un autre espace de travail et qu’il est en lecture seule.
