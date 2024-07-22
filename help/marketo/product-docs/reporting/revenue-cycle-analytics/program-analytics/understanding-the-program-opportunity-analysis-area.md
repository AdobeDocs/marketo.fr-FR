---
unique-page-id: 2951877
description: Présentation de la zone d’analyse des opportunités du programme - Documents Marketo - Documentation du produit
title: Présentation de la zone d’analyse des opportunités de programme
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 20%

---

# Présentation de la zone d’analyse des opportunités de programme {#understanding-the-program-opportunity-analysis-area}

## Vue d’ensemble {#overview}

La zone Analyse des opportunités de programme vous permet d’analyser l’efficacité de programmes individuels ou de voir les résultats résumés par canal de programme.

**Voici des exemples de questions professionnelles auxquelles vous pouvez répondre à l’aide de cette zone d’analyse :** :

Combien d’opportunités ont été associées à un programme donné et combien d’entre elles ont-elles gagné ?

![](assets/one-1.png)

Combien de recettes un programme ou canal donné a-t-il contribué à générer ?

![](assets/two-1.png)

Quels sont mes recettes en investissements pour un programme ou un canal donné ?

![](assets/three-1.png)

Quelles possibilités le programme a-t-il eu?

![](assets/four-1.png)

## Mesures d’attribution de l’analyse des opportunités du programme (points bleus) {#program-opportunity-analysis-attribution-measures-blue-dots}

Les mesures disponibles dans l’analyse sont généralement des nombres et sont représentées par des points bleus. Les Dimensions sont des attributs qui donnent différentes vues des mesures et sont représentés par des points jaunes.

Toutes les mesures (points bleus) se rapportent à l’attribution : le &quot;crédit&quot; pour l’acquisition d’une piste ou pour le succès de ventes associé à une piste.

![](assets/six.five.png) ![](assets/seven-1.png)

Il existe trois types de mesures :

* Les mesures liées à l’acquisition, qui obtiennent l’attribution Première touche (FT).
* Les mesures liées au succès, qui reçoivent une attribution multipoint (MT).
* Diverses mesures liées aux programmes, y compris le nombre moyen de touches marketing avant la création ou la fermeture d’opportunités.

## Mesures liées à l’acquisition et au succès {#acquisition-and-success-related-measures}

Les mesures liées à l’acquisition donnent du crédit au programme par lequel les coordonnées d’un prospect sont obtenues pour la première fois. Un prospect n’a pas à réussir dans un programme pour que le crédit d’acquisition soit accordé.

La valeur de l’acquisition d’une piste donnée change au fil du temps. Il est nul jusqu’à ce qu’un achat soit effectué par le prospect. Il peut ensuite augmenter avec des achats supplémentaires.

Les mesures de succès accordent du crédit à tous les programmes qui contribuent à la progression d’un prospect vers un achat.

Comme pour l’acquisition, la valeur de la contribution aux ventes réalisées pour un prospect change au fil du temps et est égale à zéro jusqu’à ce qu’un achat soit effectué par le prospect.

<table> 
 <tbody> 
  <tr> 
   <th>Mesure d’attribution - Liée aux opportunités (FT ou MT)*</th> 
   <th>Description</th> 
  </tr> 
  <tr> 
   <td>Coût des opportunités</td> 
   <td>La part du coût du programme qui a influencé l'opportunité. Le coût peut être fractionné si plusieurs pistes sont impliquées.</td> 
  </tr> 
  <tr> 
   <td>Opportunités créées</td> 
   <td>La part du crédit que le programme a reçu pour avoir influencé la création de l'opportunité. Il peut s’agir d’une fraction si plusieurs leads étaient impliqués.</td> 
  </tr> 
  <tr> 
   <td>Opportunités confirmées</td> 
   <td>La part du crédit que le programme a reçu pour avoir influé sur l'opportunité gagnée. Il peut s’agir d’une fraction si plusieurs leads étaient impliqués.</td> 
  </tr> 
  <tr> 
   <td>Pipeline créé</td> 
   <td>La part de crédit (en valeur monétaire) reçu par le programme pour avoir influencé la création de l’opportunité. Il peut s’agir d’une fraction si plusieurs leads étaient impliqués.</td> 
  </tr> 
  <tr> 
   <td>Pipeline créé - Toujours ouvert</td> 
   <td>La part de crédit (en valeur monétaire) reçu par le programme pour avoir influencé la création de l’opportunité ouverte actuellement. Il peut s’agir d’une fraction si plusieurs leads étaient impliqués.</td> 
  </tr> 
  <tr> 
   <td>Recettes attendues</td> 
   <td>La part de crédit (en valeur monétaire) reçu par le programme pour avoir influencé la création de l’opportunité. Le chiffre d’affaires attendu correspond à la probabilité d’opportunité multipliée par la valeur de l’opportunité. Il peut s’agir d’une fraction si plusieurs leads étaient impliqués.</td> 
  </tr> 
  <tr> 
   <td>Recettes pour l'investissement</td> 
   <td>Il s’agit du rapport entre la part de crédit (en valeur monétaire) reçu par le programme pour avoir influencé les opportunités confirmées et le coût du programme.</td> 
  </tr> 
  <tr> 
   <td>Chiffre d’affaires confirmé</td> 
   <td>La part de crédit (en valeur monétaire) reçu par le programme pour avoir influencé l’opportunité confirmée. Il peut s’agir d’une fraction si plusieurs leads étaient impliqués.</td> 
  </tr> 
 </tbody> 
</table>

_&#42;(FT) = Attribution Première touche, utilisée pour les mesures de l’acquisition de pistes ; (MT) = Attribution multipoint, utilisée pour les mesures de succès de pistes_

Vous trouverez ci-dessous un scénario qui décrit le mode de calcul des unités d’opportunité lorsqu’il existe deux programmes qui ont généré des pistes, mais qu’elles ont conduit à une opportunité à partir du même compte.

**Programme 1**

* Génère une piste : piste 1
* La piste 1 provient du compte 1

**Programme 2**

* Génère une autre piste : Lead 2
* La piste 2 provient également du compte 1

**Compte 1**

* Génère une opportunité : opportunité 1

Marketo accorde le crédit de manière appropriée sans double comptage des opportunités dans tous les programmes. Ainsi, dans ce cas, chaque programme reçoit 0,5 unité d’opportunités. En d’autres termes, chaque programme reçoit la moitié du crédit pour l’opportunité générée. En outre, la moitié des recettes associées à l’opportunité est affectée à chaque programme.

## Diverses mesures liées au programme {#miscellaneous-program-related-measures}

Les autres mesures disponibles reflètent la performance globale du programme.

<table> 
 <tbody> 
  <tr> 
   <th>Mesure d’attribution - En lien avec le programme</th> 
   <th>Description</th> 
  </tr> 
  <tr> 
   <td>Nombre d’opportunités associées au programme</td> 
   <td><p>Nombre total d’opportunités qui ont accordé un crédit d’attribution quelconque à un programme. Les opportunités peuvent être influencées par une ou plusieurs pistes et par un ou plusieurs programmes.</p></td> 
  </tr> 
  <tr> 
   <td>Nombre moyen de succès par opportunité fermée</td> 
   <td>Nombre moyen de succès de programme avant la clôture de l’opportunité. <br></td> 
  </tr> 
  <tr> 
   <td>Nombre moyen de succès par opportunité créée</td> 
   <td>Nombre moyen de succès de programmes avant la création de l’opportunité.</td> 
  </tr> 
  <tr> 
   <td>Nouveaux noms</td> 
   <td>Nombre total de nouveaux noms, c’est-à-dire de nouvelles pistes, acquises par le programme.</td> 
  </tr> 
  <tr> 
   <td>Coût du programme</td> 
   <td>Coût total du programme.</td> 
  </tr> 
  <tr> 
   <td>Succès (total)</td> 
   <td>Nombre total de membres du programme ayant réussi.</td> 
  </tr> 
 </tbody> 
</table>

## Dimensions d’analyse des opportunités de programme (points jaunes) {#program-opportunity-analysis-dimensions-yellow-dots}

Alors que les mesures (points bleus) sont calculées et nécessitent quelques réflexions et explications, les dimensions (points jaunes) sont descriptives. Voici les dimensions disponibles.

<table> 
 <tbody> 
  <tr> 
   <th>Catégorie</th> 
   <th>Afficher l'intitulé</th> 
  </tr> 
  <tr> 
   <td>Attributs d'opportunité</td> 
   <td>Opportunité Fermée<br>Nom de l’opportunité*<br>Nom du propriétaire de l’opportunité<br>Étape de l’opportunité<br>Type d’opportunité</td> 
  </tr> 
  <tr> 
   <td>Période d’opportunité</td> 
   <td>Opportunité Fermée Année/Trimestre/Mois<br>Opportunité Créée Année/Trimestre/Mois</td> 
  </tr> 
  <tr> 
   <td>Attributs de programme</td> 
   <td>Program Channel<br>Program Name</td> 
  </tr> 
  <tr> 
   <td>Période de coût du programme</td> 
   <td>Année/Trimestre/Mois de coût</td> 
  </tr> 
 </tbody> 
</table>

*&#42;Toutes les opportunités qui ont attribué tout type de crédit d’attribution à un programme. Les opportunités peuvent être influencées par une ou plusieurs pistes et par un ou plusieurs programmes.*

>[!MORELIKETHIS]
>
>[Créer un rapport Explorateur de recettes](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
