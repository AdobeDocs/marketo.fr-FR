---
unique-page-id: 6848705
description: Bonne pratique - Comment organiser vos programmes - Documents Marketo - Documentation du produit
title: Bonne pratique - Comment organiser vos programmes
exl-id: 018a3fbd-b741-4005-9695-56958063d71a
feature: Programs
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 4%

---

# Bonne pratique : organisation des programmes {#best-practice-how-to-organize-your-programs}

Il existe de nombreuses façons d’organiser l’arborescence dans les activités marketing, ainsi que le contenu d’un seul programme. Cependant, certaines méthodes sont plus efficaces et aideront les membres de votre service de marketing.

>[!TIP]
>
>Un jour (lorsque vous obtiendrez une promotion !), quelqu&#39;un d&#39;autre essaiera de donner un sens à vos programmes. Une bonne organisation les aidera à être rapidement productifs.

## Dossiers {#folders}

Dans Activités marketing, vous devez utiliser des dossiers pour organiser vos programmes. La structure que nous recommandons est la suivante :

>[!NOTE]
>
>**Exemple**
>
>* Programmes marketing actifs
>   * E-mails
>   * Événements
>      * Événements en direct/tournées d’exposition
>      * Salons professionnels
>      * Webinaires
>   * Bulletins d’information
>   * Nurture
>   * Contenu Web
>   * Formulaires Web
>* Formation
>* Opérationnel
>   * Cycle de vie
>   * Notation
>   * Data Management
>* Sales Insight
>   * Moments significatifs
>   * E-mails de vente
>   * Campagnes demandées par les ventes
>* **Archiver**
>   * Archiver les événements
>      * Archive 2012
>      * Archive 2013

Chacun de ces éléments mentionnés dans l’exemple est un dossier. Notez qu’ils portent tous un nom unique. Vous pouvez avoir des noms en double (plus simples) de dossiers INSIDE programmes, mais pas à la racine de l&#39;arborescence.

>[!TIP]
>
>Le dossier « Archive » est un type spécial de dossier conçu pour supprimer des éléments de listes sélectionnées ainsi que des rapports. Cela permet à votre système de fonctionner plus rapidement. En savoir [plus sur les dossiers](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md){target="_blank"}.

Vous pouvez certainement ajouter d’autres dossiers comme vous le souhaitez. Gardez simplement à l’esprit que les générations futures de professionnels du marketing au sein de votre entreprise suivront vos décisions concernant le nom et l’organisation des éléments.

## Schémas de dénomination {#naming-schemes}

Le nommage est essentiel, car les fonctionnalités de Marketo utilisent toutes un langage commun pour communiquer. Pour les programmes, vous devez leur donner un nom unique. **Deux programmes ne peuvent pas porter le même nom**. Il est recommandé d’utiliser le format suivant :

[Abréviation du type de programme ] [AAAA]-[MM]-[JJ] facultatif [brève description]

>[!NOTE]
>
>**Exemple**
>
>Exemples de noms de programme :
>
>1. ES 2015-09-21 Widget Introduction
>1. NL Newsletter 2015-06
>1. Webinaire WBN 2015-12-01

Les noms de programme doivent être uniques dans votre abonnement, même dans différents [espaces de travail](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md){target="_blank"}.  Pour les ressources locales dans les programmes, la règle est de **garder le nom simple**. Nommez simplement une invitation « Invitation », par opposition à « Invitation au webinaire de juin 2015 ». Comme ils se trouvent dans un programme, le programme parent fait automatiquement partie du nom lors de sa sélection à un autre emplacement. En d’autres termes, les ressources locales ne doivent être uniques qu’au sein du programme. Vous pouvez avoir des centaines de ressources appelées « Inviter », chacune dans un programme différent, ce qui ne vous perturbera pas.

## Jetons {#tokens}

Les jetons utilisent des dossiers et des programmes pour définir des variables à utiliser dans les pages de destination, les e-mails et d’autres ressources.

L’organisation mentionnée ci-dessus vous permet de placer des jetons dans le dossier Événement afin qu’il se répercute dans tous les événements.

>[!NOTE]
>
>**Exemple**
>
>**Adresse de votre société**. Utilisez un jeton plutôt que de l’écrire à chaque fois. Vous pouvez ainsi le mettre à jour en un seul endroit sans avoir à créer de nombreux brouillons. Remplacez ensuite le jeton selon les besoins dans un dossier de niveau inférieur.

## Événements {#events}

Un événement comporte généralement de nombreux éléments mobiles, notamment : invitations, pages de destination, formulaires, widgets sociaux et campagnes intelligentes. La bonne pratique pour les organiser afin d’en faciliter l’utilisation consiste à utiliser la phase de l’événement . Voici un exemple de la manière dont votre arborescence de dossiers doit rechercher un événement.

![](assets/capture.png)

## Programmes d’engagement {#engagement-programs}

En savoir [sur les programmes d’engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md){target="_blank"}. La meilleure façon d’organiser votre programme d’engagement est d’utiliser des dossiers. Créez un dossier pour chaque flux, puis placez les e-mails ou les programmes dans ce dossier. Incluez un dossier d’archive dans chaque flux lorsque le contenu devient obsolète et que vous souhaitez le supprimer.

## Programmes Opérationnels {#operational-programs}

Ils sont utilisés à des fins de nettoyage des données. Disposer de dossiers pour les dates d’exécution des programmes, puis archiver les dossiers. En rendant le programme opérationnel, vous l&#39;omettez des rapports, ce qui est bon pour ce genre d&#39;activité.

## Imbrication de programmes de messagerie {#nesting-email-programs}

Les programmes de messagerie sont conçus pour être votre outil de sablage de courrier. Vous pouvez les placer dans des événements ou d’autres programmes pour des promotions, des invitations et des rappels. Ils sont fournis avec un tableau de bord utile et d’autres fonctionnalités de test A/B. En outre, ils sont facilement manipulés dans la vue de planning du programme.

Vous pouvez également créer un programme d’e-mail en tant que programme autonome. Les programmes de messagerie ne sont pas autorisés dans d&#39;autres programmes de messagerie. Ce serait fou !

## Clonage {#cloning}

L’une des fonctionnalités les plus intéressantes de Marketo est la possibilité de cloner des programmes. Cela signifie que vous pouvez configurer un « modèle » de programme qui contient toutes les campagnes intelligentes et tous les e-mails que vous souhaitez. Configurez-le à l’avance, puis clonez-le pour votre prochaine initiative marketing.

>[!TIP]
>
>Remarquez les modèles d’événement dans l’exemple en haut. Insérez vos différents types d’événements pour un clonage facile.

Certaines personnes convertissent même la plupart du texte des e-mails et des landing pages en jetons. Vous pouvez ainsi cloner, puis modifier les jetons. Enfin, accédez à la vue du planning du programme et ajustez les dates. Vous avez terminé. Voila !

## Résumé {#summary}

Comme vous pouvez le voir, il y a beaucoup de pouvoir à Marketo. Nous avons abordé les bases ici, mais envisagez des services supplémentaires de [experts Marketo Engage](https://business.adobe.com/products/marketo/services-support.html){target="_blank"} pour affiner et configurer votre système pour réussir.
