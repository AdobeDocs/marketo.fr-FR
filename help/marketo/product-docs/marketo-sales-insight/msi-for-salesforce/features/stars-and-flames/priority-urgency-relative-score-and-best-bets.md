---
unique-page-id: 2950396
description: Priorité, urgence, note relative et meilleurs résultats - Documents Marketo - Documentation du produit
title: Priorité, urgence, note relative et meilleurs paris
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 1%

---

# Priorité, urgence, note relative et meilleurs paris {#priority-urgency-relative-score-and-best-bets}

Marketo Sales Insight sélectionne vos meilleurs prospects et contacts en fonction de leur priorité. La priorité d’un prospect ou d’un contact comporte deux composants : urgence et score relatif.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

Elles sont dérivées du score de piste — une mesure de l’intérêt de la personne pour vos produits. Plus le score est élevé, plus il est probable qu’ils répondent positivement à un appel de votre équipe commerciale.

>[!NOTE]
>
>Vous avez besoin de plusieurs campagnes de notation pour obtenir la valeur complète de la priorité, de l’urgence et du score relatif.  Avec trop peu ou pas de campagnes de notation, ces champs ne seront pas utiles.

## Urgence {#urgency}

Les flammes représentent l&#39;urgence — combien le score de cette personne a changé récemment. Une urgence élevée (plus de flammes) signifie que le score de cette piste a beaucoup augmenté ces derniers temps ; c&#39;est un bon signe que cette piste s&#39;intéresse à votre offre. Tu devrais suivre cette personne rapidement !

Par exemple, un prospect qui a demandé une démonstration et consulté plusieurs pages web aura probablement une urgence très élevée. Un prospect qui n’a pas consulté votre page web ou ouvert vos emails a une faible urgence. Utilisez l’urgence pour prioriser les personnes à contacter ensuite.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Évaluation relative {#relative-score}

Les étoiles représentent un score relatif — une mesure de la façon dont le score de cette personne se compare à celui de tout le monde. Un score relatif élevé signifie que cette personne est probablement plus intéressée et informée sur votre offre que les personnes ayant des scores relatifs plus faibles.

Si deux pistes ont la même urgence, vous pouvez utiliser un score relatif pour déterminer laquelle mérite un appel téléphonique en premier. Celle qui a le score relatif le plus élevé peut réagir plus favorablement à votre offre que la moins forte.

## Meilleurs paris {#best-bets}

Vos meilleurs paris sont vos pistes et vos contacts avec la plus grande urgence et le meilleur score relatif. Seules les pistes que vous détenez sont visibles dans cette liste et la liste est mise à jour à mesure que les scores changent.

>[!NOTE]
>
>Si vos paris ne correspondent pas aux meilleurs prospects et contacts que vous détenez, contactez un membre de votre société qui a accès à Marketo au sujet de la mise à jour de vos [règles de notation](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Méthode de calcul de l’urgence et de la note relative

Pour calculer le nombre d’étoiles et de flammes, vos pistes et contacts sont d’abord triés par note ou changement de score (respectivement pour Score relatif et Urgence). Ensuite ils sont divisés en niveaux — le niveau supérieur reçoit le plus d&#39;étoiles ou de flammes, le suivant reçoit moins, etc.

À mesure que les scores changent, l’urgence, la priorité et les valeurs de score relatif sont immédiatement recalculées. Les niveaux d’urgence et de score relatif sont automatiquement calculés chaque nuit sur les serveurs Marketo.

>[!NOTE]
>
>Les nombres d’urgence relative (flammes) et de score relatif (étoiles) sont des entiers dans Marketo. Les valeurs possibles pour chacune d’elles sont 0 à 3.
