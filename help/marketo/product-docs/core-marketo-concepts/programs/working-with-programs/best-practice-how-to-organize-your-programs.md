---
unique-page-id: 6848705
description: Meilleure pratique - Comment organiser vos Programmes - Docs marketing - Documentation sur les produits
title: Meilleure pratique - Comment organiser vos Programmes
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---


# Bonne pratique : Comment organiser vos Programmes {#best-practice-how-to-organize-your-programs}

Il existe de nombreuses façons d’organiser l’arborescence dans les Activités marketing ainsi que le contenu d’un seul programme. Cependant, certaines méthodes sont meilleures et aideront les personnes de votre service marketing.

>[!TIP]
>
>Un jour, (quand vous êtes promu !) quelqu&#39;un d&#39;autre essaiera de comprendre vos programmes. Une bonne organisation les aidera à être productifs rapidement.

## Dossiers {#folders}

Dans les Activités marketing, vous devez utiliser des dossiers pour organiser vos programmes. La structure que nous recommandons est présentée dans l’exemple suivant :

>[!NOTE]
>
>**Exemple**
>
>* Programmes marketing principaux
   >   * Courriers électroniques
   >   * Événements
      >      * Événements en direct / Journaux
      >      * Références commerciales
      >      * Webinaires
   >   * Bulletins
   >   * Infirmière
   >   * Contenu Web
   >   * formulaires web
>* Formation
>* Opérationnel
   >   * Cycle de vie
   >   * Scores
   >   * data Management
>* Insight commercial
   >   * Moments intéressants
   >   * Courriers électroniques des ventes
   >   * Campagnes demandées par les ventes
>* **Archiver**
   >   * Événements d&#39;archivage
      >      * Archive 2012
      >      * Archive 2013


Chacun de ces éléments mentionnés dans l&#39;exemple est un dossier. Notez comment ils portent un nom unique. Vous pouvez avoir des noms de duplicata (plus simples) de dossiers INSIDE programmes, mais pas à la racine de l&#39;arborescence.

>[!TIP]
>
>Le dossier &quot;Archiver&quot; est un type de dossier spécial conçu pour supprimer des éléments de certaines listes ainsi que du rapports. Cela permettra à votre système de s&#39;exécuter plus rapidement. En savoir plus [sur les dossiers](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md).

Vous pouvez certainement ajouter d&#39;autres dossiers à votre convenance. Gardez simplement à l’esprit que les générations futures de spécialistes du marketing dans votre société seront à l’écoute de vos décisions concernant la manière de nommer/d’organiser les éléments.

## Schémas d&#39;attribution de noms {#naming-schemes}

Le nommage est essentiel, car les fonctionnalités de Marketo utilisent toutes une langue commune pour communiquer. Pour les programmes, vous devez leur donner un nom unique. **Deux programmes ne peuvent pas avoir le même nom**. Il est recommandé d’utiliser le format suivant :

[Abréviation du Programme ] [TypeAAAA]-[MM]-Facultatif [ ] [DDBrief Description]

>[!NOTE]
>
>**Exemple**
>
>Exemples de noms de programme :
>
>1. Intro du widget ES 2015-09-21
>1. Newsletter NL 2015-06
>1. Webinaire WBN 2015-12-01


Les noms de programme doivent être uniques dans votre abonnement, même dans différents [espaces de travail](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md).  Pour les ressources locales à l’intérieur des programmes, la règle est de **conserver le nom simple**. Il vous suffit de nommer une invitation &quot;Invitation&quot;, par opposition à &quot;Invitation du webinaire de juin 2015&quot;. Dans la mesure où ils se trouvent dans un programme, le programme parent fait automatiquement partie du nom lorsqu’il le choisit ailleurs. En d’autres termes, les actifs locaux ne doivent être uniques qu’à l’intérieur du programme. Vous pouvez avoir des centaines de ressources appelées &quot;Inviter&quot;, chacune dans un programme différent et cela ne vous fera pas de mal.

## Jetons {#tokens}

Les jetons utilisent des dossiers et des programmes pour définir les variables à utiliser par les landings page, les courriels et d’autres ressources.

L’organisation mentionnée ci-dessus vous permet de placer des jetons dans le dossier de Événement afin qu’il se retrouve en cascade dans tous les événements.

>[!NOTE]
>
>**Exemple**
>
>**Votre adresse** professionnelle. Utilisez un jeton plutôt que de l’écrire à chaque fois. De cette façon, vous pouvez le mettre à jour en un seul endroit sans avoir à créer beaucoup de brouillons. Ensuite, remplacez le jeton si nécessaire dans un dossier de niveau inférieur.

## Événements {#events}

Un Événement comporte généralement de nombreuses pièces mobiles, notamment : invitations, landings page, formulaires, widgets sociaux et campagnes dynamiques. La meilleure façon de les organiser pour en faciliter l&#39;utilisation est de passer par la phase du Événement. Voici un exemple de la manière dont votre arborescence de dossiers doit rechercher un Événement.

![](assets/capture.png)

## Programmes d’engagement {#engagement-programs}

Découvrez [tout sur les programmes d&#39;engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md). Le meilleur moyen d’organiser votre programme d’engagement consiste à utiliser des dossiers. Créez un dossier pour chaque flux, puis placez les programmes ou courriers électroniques dans ce dossier. Insérez un dossier d’archives dans chaque flux lorsque le contenu devient obsolète et que vous souhaitez le supprimer.

## Programmes opérationnels {#operational-programs}

Elles sont utilisées à des fins de nettoyage des données. Disposez de dossiers pour les dates d&#39;exécution des programmes, puis archivez les dossiers. En rendant le programme opérationnel, vous l&#39;omettez du rapports, ce qui est bon pour ce genre d&#39;activité.

## Imbrication de Programmes électroniques {#nesting-email-programs}

Les Programmes électroniques sont conçus pour être votre outil de diffusion de messages. Vous pouvez les placer dans des Événements ou d&#39;autres programmes pour des promotions, des invitations et des rappels. Ils sont dotés d&#39;un tableau de bord sympa et d&#39;autres fonctions de test A/B. De plus, ils sont facilement manipulables dans la vue de Planning du programme.

Vous pouvez également créer un programme de messagerie en tant que programme autonome. Les programmes de messagerie ne sont pas autorisés dans les autres programmes de messagerie. Ce serait fou !

## Clonage {#cloning}

L&#39;une des fonctionnalités les plus cool de Marketo est la possibilité de cloner des programmes. Cela signifie que vous pouvez configurer un &quot;modèle&quot; de programme contenant toutes les campagnes et tous les courriers électroniques intelligents que vous souhaitez. Configurez-le à l’avance, puis clonez-le pour votre prochaine initiative marketing.

>[!TIP]
>
>Notez les modèles de Événement dans l&#39;exemple en haut. Mettez vos différents types de événements là-dedans pour faciliter le clonage.

Certaines personnes font même abstraction de la majeure partie du texte des courriels et landings page en jetons. Vous pouvez ainsi cloner puis modifier les jetons. Enfin, allez à la vue de Planning du programme et ajustez les dates et vous avez terminé. Voila !

## Résumé {#summary}

Comme vous pouvez le voir, il y a beaucoup de pouvoir dans Marketo. Nous avons traité des concepts de base ici, mais considérons certains [services supplémentaires de Marketo Experts](https://www.marketo.com/services/) pour affiner et vous préparer au succès.
