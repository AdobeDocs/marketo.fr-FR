---
unique-page-id: 2360309
description: Découvrez comment les espaces de travail organisent les ressources marketing et comment les partitions de personne agissent comme des bases de données distinctes.
title: Présentation des espaces de travail et des répartitions de personnes
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 97%

---

# Présentation des espaces de travail et des répartitions de personnes {#understanding-workspaces-and-person-partitions}

## Espaces de travail {#workspaces}

>[!CAUTION]
>
>La configuration des espaces de travail peut être complexe. Contactez le [support technique de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) pour savoir s’ils vous conviendraient.

Les espaces de travail sont des zones distinctes de Marketo qui contiennent des ressources marketing telles que des programmes, des pages de destination, des e-mails, etc. Ils peuvent être utilisés par plusieurs personnes. Chaque personne a accès à un ou plusieurs espaces de travail.

>[!NOTE]
>
>**Exemple**
>
>Voici quelques raisons d’utiliser un espace de travail :
>
>* Géographie : les services marketing d’Europe, d’Asie et d’Amérique du Nord disposent chacun d’un espace de travail.
>* Unité opérationnelle : [!DNL Quicken], [!DNL Quickbooks] et [!DNL TurboTax] ont chacun un espace de travail.
>
>Dans chaque cas, la séparation est due au fait que les ressources marketing sont complètement différentes. Les espaces de travail peuvent ne pas vous convenir en cas de partage des ressources marketing.

>[!NOTE]
>
>Découvrez comment [créer un espace de travail](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Partage sur plusieurs espaces de travail {#sharing-across-workspaces}

Découvrez comment partager des ressources sur plusieurs espaces de travail. Cela fonctionne de la même manière pour tout ce que vous souhaitez partager ; cet exemple illustre les segmentations.

>[!NOTE]
>
>Le dossier parent contenant vos ressources est le seul dossier qui peut être partagé, et non les dossiers enfants.

1. Cliquez sur **[!UICONTROL Base de données]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Cliquez avec le bouton droit sur le dossier Segmentation et cliquez sur **[!UICONTROL Nouveau dossier]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Nommez le dossier, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Déplacez la ou les ressources à partager dans le dossier.

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Cliquez avec le bouton droit sur le dossier et sélectionnez **[!UICONTROL Partager le dossier]**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Sélectionnez le ou les espaces de travail avec lesquels vous souhaitez partager le dossier et cliquez sur **[!UICONTROL Enregistrer]**. La boîte de dialogue Partager le dossier affiche uniquement les espaces pour lesquels vous disposez de l’autorisation d’affichage.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >Le dossier d’origine comporte désormais une petite flèche verte, indiquant qu’il a été partagé. Dans l’espace de travail partagé, le dossier comporte un cadenas, indiquant la lecture seule.

Vous pouvez partager ces éléments sur plusieurs espaces de travail.

* Modèles d’e-mail
* Modèles de page de destination
* Modèles
* Campagnes intelligentes
* [Listes intelligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentations](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Extraits

## Clonage sur plusieurs espaces de travail {#cloning-across-workspaces}

Pour les ressources qui ne sont pas des modèles, il est préférable de les cloner en tant que ressources locales dans un programme. Avec le niveau d’accès approprié, vous pouvez faire glisser ces ressources et les déposer dans un autre espace de travail :

* Programmes
* E-mails
* Pages de destination
* Formulaires

>[!IMPORTANT]
>
>Bien que tous les éléments répertoriés ci-dessus puissent être clonés dans les espaces de travail, les e-mails, les formulaires et les pages de destination _doivent se trouver dans un programme_ au moment du clonage.

>[!NOTE]
>
>Lors du clonage de ressources comportant des modèles, ces modèles doivent être partagés avec l’espace de travail de destination.

## Déplacement de ressources vers d’autres espaces de travail {#moving-assets-to-other-workspaces}

Pour déplacer des ressources vers un nouvel espace de travail, placez-les dans un dossier et faites-le glisser vers l’autre espace de travail.

>[!NOTE]
>
>Vous ne pouvez pas déplacer un programme qui contient des personnes membres d’un espace de travail à un autre.

## Répartitions de personnes {#person-partitions}

Les répartitions de personnes se comportent comme des bases de données distinctes. Chaque répartition a ses propres personnes qui ne sont pas dédupliquées ni mélangées avec d’autres répartitions. Si vous pensez avoir un cas d’utilisation professionnel qui peut nécessiter d’avoir des enregistrements en double avec la même adresse e-mail, contactez l’[assistance de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

Vous pouvez affecter des répartitions de personne aux [espaces de travail](create-a-new-workspace.md) dans les configurations suivantes :

* Un espace de travail pour une répartition de personnes (1:1)
* Un espace de travail pour plusieurs répartitions de personnes (1:x)
* Plusieurs espaces de travail pour une répartition de personnes (x:1)

>[!NOTE]
>
>Motifs d’utilisation d’une répartition de personnes :
>
>* Vos espaces de travail ne disposent pas seulement de ressources différentes, mais ils ne partagent pas les personnes non plus.
>* Vous voulez des doublons pour d’autres raisons commerciales.

>[!CAUTION]
>
>Les répartitions des personnes n’interagissent pas les unes avec les autres. Faites donc preuve de prudence lors de leur configuration.

>[!NOTE]
>
>Découvrez comment [créer une répartition de personnes](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
