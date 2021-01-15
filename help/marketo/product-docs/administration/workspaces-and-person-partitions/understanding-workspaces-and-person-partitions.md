---
unique-page-id: 2360309
description: Présentation des espaces de travail et des partitions de personne - Documents marketing - Documentation du produit
title: Présentation des espaces de travail et des partitions de personne
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---


# Présentation des espaces de travail et des partitions de personne {#understanding-workspaces-and-person-partitions}

## Espaces de travail {#workspaces}

>[!CAUTION]
>
>Les espaces de travail peuvent être complexes à configurer. Contactez le [Support marketing](https://nation.marketo.com/t5/Support/ct-p/Support) pour savoir s&#39;ils vous conviennent.

Les espaces de travail sont des zones distinctes du marché qui contiennent des actifs marketing tels que des programmes, des landings page, des courriers électroniques, etc. Ils peuvent être utilisés par plusieurs personnes. Chaque utilisateur a accès à un ou plusieurs espaces de travail.

>[!NOTE]
>
>**Exemple**
>
>Voici quelques raisons pour lesquelles vous pouvez utiliser un espace de travail :
>
>* Géographie : Les départements marketing d&#39;Europe, d&#39;Asie et d&#39;Amérique du Nord ont chacun un espace de travail
>* Unité opérationnelle : Rapide, Quickbooks et TurboTax ont chacun un espace de travail

>
>
Dans chaque cas, la séparation est due au fait que les actifs marketing sont complètement différents. S’ils partagent des ressources marketing, les espaces de travail peuvent ne pas être l’outil approprié pour vous.

>[!NOTE]
>
>Découvrez comment créer [un nouvel espace de travail](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Partage entre espaces de travail {#sharing-across-workspaces}

Voici comment partager des ressources entre différents espaces de travail. Il fonctionne de la même manière pour tout ce que vous souhaitez partager ; cet exemple montre les segmentations.

>[!NOTE]
>
>Le dossier parent contenant vos ressources est le seul dossier qui peut être partagé, pas les dossiers enfants.

1. Créez un dossier.

   ![](assets/one.png)

1. Nommez le dossier que vous allez partager.

   ![](assets/two.png)

1. Déplacez le ou les fichiers que vous souhaitez partager dans le dossier.

   ![](assets/three.png)

1. Cliquez avec le bouton droit sur le dossier et sélectionnez **Partager le dossier**.

   ![](assets/four.png)

1. Sélectionnez le ou les espaces de travail avec lesquels partager le dossier, puis cliquez sur **Enregistrer**. La boîte de dialogue Partager le dossier affiche uniquement les espaces de travail autorisés à la vue.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >Le dossier d’origine comporte désormais une petite flèche verte indiquant qu’il a été partagé. Dans l’espace de travail partagé, le dossier comporte un cadenas indiquant qu’il est en lecture seule.

Vous pouvez partager ces éléments dans les espaces de travail.

* Modèles de courrier électronique
* Modèles de landing page
* Modèles
* Campagnes dynamiques
* [Listes intelligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segments](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Extraits de code

## Clonage entre les espaces de travail {#cloning-across-workspaces}

Pour les ressources qui ne sont pas des modèles, il est préférable de les cloner en tant que ressources locales au sein d’un programme.  Avec le niveau d’accès approprié, vous pouvez faire glisser ces ressources vers un autre espace de travail :

* Programmes
* Courriers électroniques
* landings page
* Forms

>[!NOTE]
>
>Lors du clonage de fichiers qui comportent des modèles, ces modèles doivent être partagés avec l’espace de travail de destination.

## Déplacement de ressources vers d’autres espaces de travail {#moving-assets-to-other-workspaces}

Pour déplacer des fichiers vers un nouvel espace de travail, placez-les dans un dossier et faites glisser le dossier vers l’autre espace de travail.

>[!NOTE]
>
>Vous ne pouvez pas déplacer un programme qui contient des membres d&#39;un espace de travail à un autre.

## Partitions de personne {#person-partitions}

Les partitions de personne agissent comme des bases de données distinctes. Chaque partition a ses propres personnes qui ne dédupliquent pas ou ne se mélangent pas avec d&#39;autres partitions. Si vous estimez que vous avez un cas d&#39;utilisation commerciale qui peut nécessiter l&#39;utilisation d&#39;enregistrements de duplicata avec la même adresse électronique, veuillez contacter le [Support marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

Vous pouvez affecter des partitions de personne à [espaces de travail](create-a-new-workspace.md) dans les configurations suivantes :

* un espace de travail à une partition individuelle (1:1)
* un espace de travail pour plusieurs partitions (1:x)
* plusieurs espaces de travail sur une partition individuelle (x:1)

>[!NOTE]
>
>Raisons pour lesquelles vous utiliseriez une partition de personne :
>
>* Vos espaces de travail ont non seulement des ressources différentes, mais ils ne partagent pas non plus de personnes.
>* Vous voulez des duplicata pour d&#39;autres raisons commerciales


>[!CAUTION]
>
>Les partitions personnelles n&#39;interagissent pas les unes avec les autres, soyez donc prudent lors de leur configuration.

>[!NOTE]
>
>Découvrez comment [créer une partition de personne](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
