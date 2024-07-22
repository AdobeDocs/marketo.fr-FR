---
description: Onglet Carte de l’engagement - Documents Marketo - Documentation du produit
title: Onglet Carte d’engagement
exl-id: 8c4d076a-d8aa-44ff-b538-ca6a6778697a
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# Onglet Carte d’engagement {#engagement-map-tab}

La carte de l’engagement est représentée par une série de déclencheurs, de filtres et de cartes de flux. Cliquez sur chaque carte pour afficher des informations supplémentaires.

Présentation du déclencheur : cette carte indique le nombre de déclencheurs dans votre campagne. Si vous cliquez dessus, une carte s’affiche pour chaque déclencheur, ainsi qu’un panneau déroulant contenant les informations suivantes :

* Campagne à laquelle le déclencheur appartient
* Liste des noms des déclencheurs
* Modifier le déclencheur

  ![](assets/engagement-map-tab-1.png)

Détails du déclencheur : cette carte affiche le nom du déclencheur. Si vous cliquez dessus, un panneau de visualisation s’affiche avec les informations suivantes :

* Campagne à laquelle le déclencheur appartient
* Liste des contraintes associées au déclencheur
* Modifier le déclencheur

Filtre : lorsque vous cliquez sur cette carte, un panneau de visualisation s’affiche avec les informations suivantes :

* Campagne à laquelle le filtre appartient
* Nombre estimé de personnes qui remplissent les critères du filtre
* Liste des filtres et leurs contraintes respectives
* Modifier le filtre

  ![](assets/engagement-map-tab-3.png)

Étapes du flux : si une étape de flux comprend des choix, cette carte indique le nom de l’étape de flux. Si vous cliquez dessus, un panneau de visualisation s’affiche avec les informations suivantes :

* Opération à laquelle appartient l’étape de flux
* Liste des conditions de choix associées à l’étape de flux
* Étape de flux de modification

Étapes de flux : si une étape de flux n’inclut _pas_ d’options, cette carte affiche les attributs associés à l’étape de flux. Si vous cliquez dessus, un panneau de visualisation s’affiche avec les informations suivantes :

* Opération à laquelle appartient l’étape de flux
* Liste des attributs associés à l’étape de flux
* Étape de flux de modification

  ![](assets/engagement-map-tab-5.png)

## Étape de flux pour exécuter et demander des campagnes {#flow-step-for-execute-and-request-campaigns}

* Si l’étape Exécuter ou Demander le flux de la campagne n’inclut aucun choix, la carte affichera le nom de la campagne. Un clic sur la carte affiche un panneau déroulant contenant les informations suivantes :

   * Opération à laquelle appartient l’étape de flux
   * Étape de flux de modification
   * Liste des attributs associés à l’étape de flux
   * Bouton &quot;Afficher la liste&quot; qui ouvre la liste des campagnes qui utilisent la requête/exécution de campagne spécifique

>[!NOTE]
>
>Vous pouvez modifier la ou les étapes du flux à partir d’une campagne principale. Pour modifier les campagnes imbriquées, vous devez accéder à la campagne à partir du lien situé dans le panneau déroulant.

* Si l’étape Exécuter ou Demander le flux d’une campagne comporte des choix, un clic sur la carte affiche un panneau déroulant contenant les informations suivantes :

   * Opération à laquelle appartient l’étape de flux
   * Liste des conditions de choix associées à l’étape de flux
   * Étape de flux de modification

* Si une campagne Exécuter ou Demander comprend des choix, un clic sur la carte de flux se développe afin d’afficher tous les choix dans des cartes individuelles. Cliquez sur la carte _choice_ pour développer la campagne associée au choix spécifique et afficher un panneau déroulant contenant les informations suivantes :

   * Campagne à laquelle le choix appartient
   * Modifier le choix
   * Liste des conditions de choix associées à l’étape de flux
   * Afficher la liste, qui ouvre une liste des campagnes qui utilisent la requête/exécution de campagne spécifique

  ![](assets/engagement-map-tab-10.png)

## Visualisation d’une campagne d’exécution imbriquée {#visualizing-a-nested-execute-campaign}

Exécutez les campagnes exécutées en série avec la campagne parente. Les personnes qui remplissent les critères d’une campagne exécutable doivent suivre toutes les étapes du flux de la campagne et revenir à la campagne principale pour continuer les étapes du flux de cette campagne.

Vous trouverez ci-dessous un exemple de campagne dynamique, &quot;Campagne A&quot;, qui comprend une étape d’exécution du flux de campagne. Considérez &quot;Campagne A&quot; comme votre campagne principale.

![](assets/engagement-map-tab-11.png)

1. Cliquez sur la carte d’exécution du flux de campagne pour afficher les détails de la &quot;campagne B&quot;.
1. La &quot;Campagne B&quot; comprend un filtre qui divise l&#39;audience en deux groupes : qualifiés et non qualifiés.
1. L’audience qualifiée passe par les étapes de flux associées à la &quot;campagne B&quot;.
1. Toutes les audiences (qualifiées et non qualifiées) reviennent à &quot;Campagne A&quot; et passent à l’étape suivante du flux.

   ![](assets/engagement-map-tab-12.png)

Vous pouvez cliquer sur l’étape Exécuter le flux de campagne de la &quot;Campagne B&quot;, qui s’agrandit pour afficher les cartes de choix et la campagne associées à chaque choix.

![](assets/engagement-map-tab-13.png)

## Visualisation de la campagne de requêtes {#visualizing-request-campaign}

Les campagnes de requête s’exécutent en parallèle de la campagne parente. Les personnes qui remplissent les critères d’une campagne de demande effectuent toutes les étapes de flux de la campagne, puis quittent celle-ci. Parallèlement, le même groupe de personnes passe par les étapes de flux de la campagne principale.

Voici un exemple de campagne dynamique, &quot;Campagne A&quot;, qui comprend une étape de flux de campagne de requête. Considérez &quot;Campagne A&quot; comme votre campagne principale.

![](assets/engagement-map-tab-14.png)

1. Cliquez sur la carte de flux de campagne de requête pour afficher les détails de la &quot;campagne B&quot;.
1. La &quot;Campagne B&quot; comprend un filtre qui divise l&#39;audience en deux groupes : qualifiés et non qualifiés.
1. L’audience qualifiée passe par les étapes de flux associées à la &quot;campagne B&quot;.
1. En même temps, toutes les audiences passent aux étapes de flux suivantes de la &quot;Campagne A&quot;.

   ![](assets/engagement-map-tab-15.png)

Vous pouvez approfondir l’analyse de vos campagnes imbriquées si l’une des étapes de flux comprend une autre campagne de requête en cliquant sur la carte de flux pour afficher les détails de la campagne.

![](assets/engagement-map-tab-16.png)

Voici un exemple de campagne de requêtes avec des choix.

![](assets/engagement-map-tab-17.png)

## Gestion des erreurs {#error-handling}

Les erreurs des listes dynamiques et des étapes de flux sont mises en surbrillance par une icône rouge dans la carte. En outre, un message d’erreur correspondant sera reflété dans le panneau de visualisation.

Les avertissements dans les listes dynamiques et les étapes de flux sont mis en surbrillance par une icône orange dans la carte. En outre, un message d’avertissement correspondant sera reflété dans le panneau déroulant.

Vous trouverez ci-dessous un exemple d’avertissement dans une carte Choix qui s’affiche dans la carte d’étape Exécuter la campagne , dans le panneau déroulant et dans la carte de choix Par défaut .

![](assets/engagement-map-tab-18.png)

>[!NOTE]
>
>Les avertissements sont des recommandations à examiner, mais ne sont pas des indicateurs d’erreurs dans la campagne dynamique.

**Les erreurs dans les cartes de filtre peuvent inclure :**

* Une erreur dans la liste dynamique qui empêchera l’affichage d’une audience qualifiée

* Une erreur dans la logique de filtre

* Une erreur dans les contraintes (ou leur absence) d’un ou plusieurs filtres

  ![](assets/engagement-map-tab-20.png)

>[!NOTE]
>
>Les erreurs au sein d’une campagne imbriquée ne seront pas visibles tant que vous n’aurez pas cliqué pour développer la campagne imbriquée.
