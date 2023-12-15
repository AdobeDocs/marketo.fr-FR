---
unique-page-id: 2360309
description: Présentation des espaces de travail et des partitions de personne - Documents Marketo - Documentation du produit
title: Présentation des espaces de travail et des partitions de personne
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: 91b6460bf0fa7fed85d48887ec38203f2ee7440f
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 3%

---

# Présentation des espaces de travail et des partitions de personne {#understanding-workspaces-and-person-partitions}

## Espaces de travail {#workspaces}

>[!CAUTION]
>
>La configuration des espaces de travail peut s’avérer complexe. Contact [Prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) pour savoir s&#39;ils ont raison pour vous.

Les espaces de travail sont des zones distinctes de Marketo qui contiennent des ressources marketing telles que des programmes, des landing pages, des emails, etc. Ils peuvent être utilisés par plusieurs personnes. Chaque utilisateur a accès à un ou plusieurs espaces de travail.

>[!NOTE]
>
>**Exemple**
>
>Pour certaines raisons, vous pouvez utiliser un espace de travail :
>
>* Géographie : les départements marketing d’Europe, d’Asie et d’Amérique du Nord ont chacun un espace de travail
>* Unité opérationnelle : [!DNL Quicken], [!DNL Quickbooks] et [!DNL TurboTax] obtenir un espace de travail
>
>Dans chaque cas, la séparation est due au fait que les ressources marketing sont complètement différentes. S’ils partagent des ressources marketing, les espaces de travail peuvent ne pas être l’outil idéal pour vous.

>[!NOTE]
>
>Découvrez comment créer [créer un espace de travail](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Partage entre espaces de travail {#sharing-across-workspaces}

Voici comment partager des ressources entre espaces de travail. Il fonctionne de la même manière pour tout ce que vous souhaitez partager ; cet exemple affiche des segments.

>[!NOTE]
>
>Le dossier parent contenant vos ressources est le seul dossier qui peut être partagé, et non les dossiers enfants.

1. Cliquez sur **[!UICONTROL Base]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Cliquez avec le bouton droit de la souris sur le dossier Segmentation, puis cliquez sur **[!UICONTROL Nouveau dossier]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Nommez votre dossier et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Déplacez la ou les ressources que vous souhaitez partager dans le dossier .

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Cliquez avec le bouton droit sur le dossier et sélectionnez **[!UICONTROL Share Folder]**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Sélectionnez le ou les espaces de travail avec lesquels vous souhaitez partager le dossier et cliquez sur **[!UICONTROL Enregistrer]**. La boîte de dialogue Partager le dossier affiche uniquement les espaces de travail que vous êtes autorisé à afficher.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >Le dossier d’origine comporte désormais une petite flèche verte, indiquant qu’il a été partagé. Dans l’espace de travail partagé, le dossier comporte un cadenas, indiquant la lecture seule.

Vous pouvez partager ces éléments dans plusieurs espaces de travail.

* Modèles d’e-mail
* Modèles de page de destination
* Modèles
* Campagnes intelligentes
* [Listes dynamiques](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentations](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Extraits

## Clonage dans les espaces de travail {#cloning-across-workspaces}

Pour les ressources qui ne sont pas des modèles, il est préférable de les cloner en tant que ressources locales au sein d’un programme. Avec le niveau d’accès approprié, vous pouvez faire glisser ces ressources dans un autre espace de travail :

* Programmes
* E-mails
* Pages de destination
* Formulaires

>[!IMPORTANT]
>
>Bien que tous les éléments répertoriés ci-dessus puissent être clonés dans des espaces de travail, des emails, des formulaires et des landing pages _doit figurer dans un programme_ au moment du clonage.

>[!NOTE]
>
>Lors du clonage de ressources qui comportent des modèles, ces modèles doivent être partagés avec l’espace de travail de destination.

## Déplacement de ressources vers d’autres espaces de travail {#moving-assets-to-other-workspaces}

Pour déplacer des ressources vers un nouvel espace de travail, placez-les dans un dossier et faites glisser le dossier vers l’autre espace de travail.

>[!NOTE]
>
>Vous ne pouvez pas déplacer un programme contenant des membres d’un espace de travail vers un autre.

## Répartitions de l&#39;individu {#person-partitions}

Les partitions de personne agissent comme des bases de données distinctes. Chaque partition a sa propre population qui ne déduplique pas ou ne mélange pas avec d&#39;autres partitions. Si vous pensez que vous avez un cas d’utilisation commerciale qui peut nécessiter la duplication d’enregistrements avec la même adresse email, veuillez contacter [Prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

Vous pouvez affecter des partitions à des personnes.  [espaces de travail](create-a-new-workspace.md) dans les configurations suivantes :

* un espace de travail à une partition par personne (1:1)
* un espace de travail pour plusieurs partitions (1:x)
* de nombreux espaces de travail à une seule partition (x:1) ;

>[!NOTE]
>
>Raisons pour lesquelles vous utiliseriez une partition de personne :
>
>* Vos espaces de travail ne contiennent pas seulement des ressources différentes, mais ne partagent pas non plus de personnes.
>* Vous souhaitez des doublons pour d’autres raisons commerciales.

>[!CAUTION]
>
>Les partitions personnelles n&#39;interagissent pas entre elles, soyez donc prudent lors de leur configuration.

>[!NOTE]
>
>Découvrez comment [créer une partition de personne](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
