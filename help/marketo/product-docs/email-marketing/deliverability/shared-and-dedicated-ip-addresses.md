---
unique-page-id: 10912085
description: Adresses IP partagées et dédiées - Documents Marketo - Documentation du produit
title: Adresses IP partagées et dédiées
exl-id: 3d7a78f4-531a-4ad7-a20b-1385bd62d1d9
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Adresses IP partagées et dédiées {#shared-and-dedicated-ip-addresses}

## Qu’est-ce qu’une adresse IP ? {#what-is-an-ip-address}

Libellé numérique désignant l’adresse d’un ordinateur connecté à Internet.

## Que sont les adresses IP partagées ? {#what-are-shared-ip-addresses}

Cela fait référence lorsque plusieurs expéditeurs utilisent les mêmes adresses IP pour lancer des campagnes par courrier électronique. Ils partagent tous les mêmes adresses IP d’envoi.

## Qu’est-ce qu’une adresse IP dédiée ? {#what-is-a-dedicated-ip-address}

Adresse IP spécifique à l’utilisateur à partir de laquelle un seul expéditeur envoie.

## Quelle est la meilleure : partagée ou dédiée ? {#which-is-better-shared-or-dedicated}

Comme d’habitude, il existe des avantages et des inconvénients pour les deux options.

**Avantages et inconvénients d’une adresse IP dédiée**

_Pros_

**Réputation** - Vous détenez entièrement votre réputation et votre délivrabilité.\
**Surveillance** - Suivre les rapports de délivrabilité vous permet de réagir rapidement aux changements de vos mesures de diffusion.\
**Résolution de problème** - Il est plus facile de rechercher, de comprendre et de résoudre les problèmes de diffusion.

_Inconvénients_

**Changements de volume** - Les pics de volume peuvent nuire à votre réputation et doivent être gérés.\
**Processus de nettoyage d’IP** - La réputation est créée au fil du temps. Certains fournisseurs de services Internet (FAI) réduisent les adresses IP sans historique des volumes. Vous devrez donc établir une réputation au cours des premières semaines (Marketo peut vous aider à vous guider).\
**Coût** : l’envoi à partir d’une adresse IP dédiée à n’importe quel fournisseur entraîne généralement des frais supplémentaires.

**Avantages et inconvénients d’une adresse IP partagée**

_Pros_

**Bons colocataires** - Si les personnes que vous partagez votre adresse IP suivent les bonnes pratiques d’envoi, vous en tirerez avantage.\
**Fréquence de messagerie** - Aucune fréquence de messagerie minimale n’est nécessaire pour être admissible pour une adresse IP partagée, contrairement aux adresses IP dédiées.\
**Coût** : il n’y a jamais de frais supplémentaires à envoyer à partir d’une adresse IP partagée.

_Inconvénients_

**Mauvais(s) compagnons de chambrée** - Si les personnes que vous partagez votre adresse IP et qui s’engagent dans de mauvaises pratiques d’envoi, vos campagnes par e-mail risquent d’être affectées.\
**Contrôle** - Vous avez beaucoup moins de contrôle sur la réputation de votre expéditeur.\
**Résolution de problème** : il peut souvent être plus difficile de résoudre un problème lors de l’envoi à partir d’adresses IP partagées.

>[!NOTE]
>
>Lorsque vous prenez une décision, il y a un autre facteur important à prendre en compte : le volume d&#39;envoi. Si vous prévoyez d’envoyer moins de 100 000 emails par mois, ou moins de deux envois par mois, vous ne bénéficierez probablement pas d’une adresse IP dédiée. Les envois de ce type sont considérés comme peu nombreux et il serait difficile de garder votre adresse IP dédiée suffisamment &quot;chaude&quot; pour être considérée comme sûre par les principaux FAI. En gros, si vous ne publiez pas assez souvent, les FAI verront un publipostage comme une &quot;augmentation&quot; soudaine de l&#39;activité et pourraient finir par le bloquer comme un spam suspecté.

Si vous avez des questions ou si vous souhaitez configurer une adresse IP dédiée, contactez votre représentant commercial Marketo.
