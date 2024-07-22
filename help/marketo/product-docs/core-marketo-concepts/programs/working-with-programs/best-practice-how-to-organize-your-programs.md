---
unique-page-id: 6848705
description: Bonne pratique - Comment organiser vos programmes - Documents Marketo - Documentation du produit
title: Bonne pratique - Comment organiser vos programmes
exl-id: 018a3fbd-b741-4005-9695-56958063d71a
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 4%

---

# Bonne pratique : comment organiser vos programmes {#best-practice-how-to-organize-your-programs}

Il existe de nombreuses façons d’organiser l’arborescence dans les activités marketing ainsi que le contenu d’un seul programme. Cependant, certaines solutions sont meilleures et aideront les personnes de votre service marketing.

>[!TIP]
>
>Un jour (quand vous serez promu !), quelqu&#39;un d&#39;autre essaiera de donner du sens à vos programmes. Une bonne organisation les aidera à être productifs rapidement.

## Dossiers {#folders}

Dans Activités marketing, vous devez utiliser des dossiers pour organiser vos programmes. La structure que nous recommandons est dans l&#39;exemple suivant :

>[!NOTE]
>
>**Exemple**
>
>* Programmes marketing actifs
>   * E-mails
>   * Événements
>      * Événements en direct / Fiches d’affichage
>      * Salons professionnels
>      * Webinaires
>   * Bulletins d’information
>   * Nurture
>   * Contenu Web
>   * Formulaires Web
>* Learning
>* Opérationnel
>   * Cycle de vie
>   * Évaluation
>   * Gestion des données
>* Sales Insight
>   * Moments significatifs
>   * E-mails de vente
>   * Campagnes demandées par les ventes
>* **Archive**
>   * Événements d’archivage
>      * Archive 2012
>      * Archive 2013

Chacun des éléments mentionnés dans l’exemple est un dossier. Remarquez comment ils portent tous un nom unique. Vous pouvez avoir des noms en double (plus simples) de dossiers dans les programmes INSIDE, mais pas à la racine de l’arborescence.

>[!TIP]
>
>Le dossier &quot;Archive&quot; est un type spécial de dossier conçu pour supprimer des éléments des listes sélectionnées ainsi que des rapports. Cela permettra à votre système de s’exécuter plus rapidement. En savoir plus [sur les dossiers](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md){target="_blank"}.

Vous pouvez certainement ajouter d’autres dossiers à votre gré. Gardez simplement à l’esprit que les futures générations de spécialistes du marketing de votre entreprise accompagneront vos décisions sur la manière de nommer/organiser des choses.

## Modèles de dénomination {#naming-schemes}

Le nommage est essentiel, car les fonctions de Marketo utilisent toutes une langue commune pour communiquer. Pour les programmes, vous devez leur attribuer un nom unique. **Aucun programme ne peut porter le même nom**. Il est recommandé d’utiliser le format suivant :

[Abréviation du type de programme] [AAAA]-[MM]-[JJ facultatif] [Brève description]

>[!NOTE]
>
>**Exemple**
>
>Exemples de noms de programme :
>
>1. Intro du widget ES 2015-09-21
>1. Newsletter NL 2015-06
>1. Le webinaire WBN 2015-12-01 ici

Les noms de programme doivent être uniques dans votre abonnement, même dans différents [espaces de travail](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md){target="_blank"}.  Pour les ressources locales dans les programmes, la règle est de **conserver le nom simple**. Il suffit de nommer une invitation &quot;Invitation&quot;, par opposition à &quot;Invitation du webinaire de juin 2015&quot;. Puisqu’il s’agit d’un programme, le programme parent fait automatiquement partie du nom lorsqu’il est sélectionné ailleurs. En d’autres termes, les ressources locales ne doivent être uniques que dans le programme. Vous pouvez avoir des centaines de ressources nommées &quot;Invitation&quot;, chacune dans un programme différent et ça ne vous fera pas de mal.

## Jetons {#tokens}

Les jetons utilisent des dossiers et des programmes comme véhicule pour définir les variables à utiliser par les landing pages, les emails et d’autres ressources.

L’organisation mentionnée ci-dessus vous permet de placer des jetons dans le dossier Événement afin qu’il soit ventilé en tous les événements.

>[!NOTE]
>
>**Exemple**
>
>**Votre adresse d’entreprise**. Utilisez un jeton plutôt que de l’écrire à chaque fois. Vous pouvez ainsi le mettre à jour à un seul emplacement sans avoir à créer de nombreux brouillons. Remplacez ensuite le jeton selon les besoins dans un dossier de niveau inférieur.

## Événements {#events}

Un événement comporte généralement de nombreuses parties mobiles, notamment : invitations, landing pages, formulaires, widgets sociaux et campagnes intelligentes. La bonne pratique pour les organiser pour en faciliter l’utilisation est d’abord la phase de l’événement. Voici un exemple de la manière dont votre arborescence de dossiers doit rechercher un événement.

![](assets/capture.png)

## Programmes d&#39;engagement {#engagement-programs}

Découvrez [tous les programmes d’engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md){target="_blank"}. La meilleure façon d’organiser votre programme d’engagement est d’utiliser les dossiers. Créez un dossier pour chaque flux, puis placez les emails ou les programmes dans ce dossier. Incluez un dossier d’archive dans chaque flux lorsque le contenu devient obsolète et que vous souhaitez le supprimer.

## Programmes opérationnels {#operational-programs}

Ils sont utilisés à des fins de nettoyage des données. Disposer de dossiers pour les dates d’exécution des programmes, puis archiver les dossiers. En rendant le programme opérationnel, vous l&#39;omettez des rapports, ce qui est bon pour ce genre d&#39;activité.

## Imbrication de programmes de messagerie {#nesting-email-programs}

Les programmes de messagerie électronique sont conçus pour être votre outil de diffusion différée du courrier. Vous pouvez les placer dans des Événements ou d’autres programmes pour des promotions, des invitations et des rappels. Ils sont fournis avec un tableau de bord attrayant et d’autres fonctions de test A/B. En outre, ils sont facilement manipulés dans la vue de planification du programme.

Vous pouvez également créer un programme de messagerie en tant que programme autonome. Les programmes de messagerie électronique ne sont pas autorisés dans d’autres programmes de messagerie. Ce serait fou !

## Clonage {#cloning}

L’une des fonctionnalités les plus cool de Marketo est la capacité à cloner des programmes. Cela signifie que vous pouvez configurer un &quot;modèle&quot; de programme qui contient toutes les campagnes intelligentes et tous les emails que vous souhaitez. Configurez-le à l’avance, puis clonez-le pour votre prochaine initiative marketing.

>[!TIP]
>
>Notez les modèles d’événement dans l’exemple ci-dessus. Placez vos différents types d&#39;événements là-dedans pour faciliter le clonage.

Certaines personnes abstraient même la plupart du texte des emails et des landing pages dans des jetons. Vous pouvez ainsi cloner puis modifier les jetons. Enfin, accédez à la vue du planning du programme et ajustez les dates et vous avez terminé. Voila !

## Résumé {#summary}

Comme vous pouvez le voir, Marketo a beaucoup de pouvoir. Nous avons abordé les principes de base ici, mais nous vous invitons à vous aider des [experts Marketo Engage](https://business.adobe.com/products/marketo/services-support.html){target="_blank"} pour vous perfectionner et vous préparer au succès.
