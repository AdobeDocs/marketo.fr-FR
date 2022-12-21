---
unique-page-id: 7515767
description: Partage de segments entre espaces de travail et partitions - Documents Marketo - Documentation du produit
title: Partage de segments entre espaces de travail et partitions
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '469'
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
>En savoir plus [comment créer des segments](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Une fois ces personnages configurés (_et_ si vous utilisez des espaces de travail), vous souhaiterez les partager dans vos espaces de travail. Voici quelques bonnes choses à savoir :

## Règles et conseils {#rules-tips}

* Chaque abonnement Marketo peut contenir jusqu’à 20 segments &quot;totaux&quot; sur plusieurs espaces de travail (**pas 20 par espace de travail**).
* Vous pouvez uniquement partager une segmentation avec les espaces de travail auxquels vous avez accès.
* Veillez à créer et à utiliser une **Espace de travail par défaut ayant une visibilité sur toutes les partitions**.

* Le traitement de la segmentation s’exécute uniquement sur les personnes de l’espace de travail dans lequel la segmentation est créée.

   * Créez la segmentation que vous souhaitez partager dans l’espace de travail par défaut.
      * Approuver la segmentation
      * L’espace de travail partagé voit un dossier verrouillé et la segmentation est en lecture seule.
      * La version partagée ne peut pas être modifiée. Vous ne pouvez modifier que la segmentation d’origine dans laquelle elle a été créée.
   * Lorsque vous cliquez sur un segment (par exemple, Health Care) dans une segmentation partagée, les personnes que vous voyez ne seront que des personnes dans la partition associée à l’espace de travail que vous visualisez.
      * Si vous créez une segmentation dans Workspace 1 (WS1) et que vous la partagez avec WS2 et WS1 n’a pas accès à la partition pour WS2, la segmentation NE SERA PAS recalculée.
      * Si vous créez une Segmentation dans un espace de travail qui comporte des partitions limitées, puis que vous la partagez avec un autre espace de travail, cet espace de travail qui a reçu la Segmentation partagée ne verra les personnes que s’ils se chevauchent.


>[!NOTE]
>
>Certaines de ces règles sont un peu complexes. Le moyen le plus simple de commencer est de tester avec des personnes spécifiques. Vous pouvez toujours créer de nouvelles segments et vous débarrasser des anciens.

## Exemples de scénarios {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

![](assets/image2015-5-27-16-3a26-3a48.png)

## Partage d’une segmentation {#share-a-segmentation}

1. Accédez au **Base**.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Clic droit **Segments** et sélectionnez **Nouveaux dossiers**.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Nommez le dossier que vous allez partager dans les espaces de travail (par exemple : Partager des segments).

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Déplacez la ou les segmentation que vous souhaitez partager dans le dossier .

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Cliquez avec le bouton droit sur le dossier et sélectionnez **Partager le dossier**.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Sélectionnez le ou les espaces de travail avec lesquels vous souhaitez partager le dossier. Cliquez sur **Enregistrer**.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >La boîte de dialogue affiche les espaces de travail que vous êtes autorisé à afficher. C’est pourquoi Marketo recommande de créer et de partager des segments à partir de l’espace de travail par défaut, qui ont une visibilité sur tous les espaces de travail et partitions.

Le dossier d’origine s’affiche dans l’arborescence de la base de données avec une flèche indiquant qu’il est partagé avec d’autres espaces de travail. Depuis l’espace de travail partagé, le dossier s’affiche avec un cadenas pour indiquer que le contenu du dossier a été partagé depuis un autre espace de travail et qu’il est en lecture seule.
