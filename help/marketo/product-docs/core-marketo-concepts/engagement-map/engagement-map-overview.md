---
description: Présentation de la carte de l’engagement - Documents Marketo - Documentation du produit
title: Présentation de la carte des engagements
hide: true
hidefromtoc: true
exl-id: 0b445ac7-bfa4-4f86-bb92-86d4d982555e
source-git-commit: 3c7eb2fc2e64898e12f08743225c0b802bf97474
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Présentation de la carte des engagements {#engagement-map-overview}

>[!AVAILABILITY]
>
>Cette fonctionnalité est actuellement disponible pour les campagnes dynamiques. Il n’est pas disponible pour les programmes.

La carte de l’engagement vous permet de créer des campagnes intelligentes réutilisables à l’aide de visuels intuitifs. Il offre une compatibilité ascendante complète avec toutes les campagnes dynamiques de Marketo Engage existantes, sans perte de fonctionnalités actuelles.

![](assets/engagement-map-overview-1.png)

## Accès à la carte de l’engagement {#accessing-engagement-map}

Accédez à une campagne existante, puis cliquez sur le bouton **Carte d’engagement** bouton .

![](assets/engagement-map-overview-2.png)

Deux onglets s’affichent une fois dans la carte Engagement : [Carte d’engagement](/help/marketo/product-docs/core-marketo-concepts/engagement-map/engagement-map-tab.md){target="_blank"} and [Settings](/help/marketo/product-docs/core-marketo-concepts/engagement-map/settings-tab.md){target="_blank"}.

![](assets/engagement-map-overview-3.png)

## Descriptions des cartes {#card-descriptions}

**Triggers**: dans les campagnes qui incluent des déclencheurs, la carte comporte une carte &quot;Présentation du déclencheur&quot;. Si vous cliquez sur cette option, une carte s’affiche pour chaque déclencheur, ainsi qu’un panneau déroulant contenant des informations supplémentaires.

**Filtres**: dans les campagnes qui incluent des filtres, la carte contiendra une carte pour chacune d’elles. Si vous cliquez dessus, un panneau déroulant contenant des informations supplémentaires s’affiche.

**Étapes de flux**: chaque campagne comprend une carte pour chaque étape de flux. Si vous cliquez dessus, un panneau déroulant contenant des informations supplémentaires s’affiche.

**Choix**: si une étape de flux comprend un ou plusieurs choix, un clic sur la carte de flux affiche une carte pour chaque choix, ainsi qu’un panneau de sortie avec des informations supplémentaires.

## Campagnes imbriquées {#nested-campaigns}

* Si une campagne comprend une étape de flux Demander ou Exécuter la campagne , un clic sur la carte de flux affiche les détails de l’opération en cours d’appel, ainsi qu’un panneau de sortie avec des informations supplémentaires.

* Si une campagne comprend une étape de flux Demander ou Exécuter une campagne avec des choix, un clic sur la carte de flux affiche une carte de choix, ainsi qu’un panneau d’affichage avec des informations supplémentaires sur les choix. Cliquez sur chaque carte de choix pour afficher les détails de la campagne en cours d’appel, ainsi qu’un panneau déroulant contenant des informations supplémentaires.

* De plus, si l’une des campagnes imbriquées comporte une étape de flux Demander ou Exécuter la campagne , cliquez sur la carte de flux pour afficher les détails de la campagne. Il en va de même lorsque l’étape de flux comprend des choix.

## Navigation supérieure {#top-navigation}

Le volet de navigation supérieur comprend les fonctionnalités suivantes :

* Nom de la campagne et accès au modal &quot;Modifier la campagne&quot;, vous pouvez modifier le nom et la description de la campagne ici.

* L’état et le type de campagne de la campagne seront reflétés sous le nom de la campagne.

* Bouton Activer/Désactiver pour les campagnes de déclenchement

* Modifier la liste dynamique : vous accédez à l’interface Liste dynamique dans un nouvel onglet où vous pouvez ajouter ou modifier votre liste dynamique.

* Modifier le flux : vous accédez à l’interface Flux dans un nouvel onglet où vous pouvez ajouter ou modifier votre liste dynamique.

* Exporter : télécharge une image de visualisation de campagne. La version téléchargée reflète les branches que vous avez développées.

* Afficher les membres de campagne : un nouvel onglet contenant les détails des membres de campagne s’ouvre.

>[!NOTE]
>
>Les modifications apportées dans un onglet de liste dynamique et de flux ouvert seront répercutées dans l’onglet de carte de l’engagement lors de l’actualisation. Elle ne sera pas mise à jour automatiquement. Les mises à jour et modifications enregistrées automatiquement sont répercutées.

## Questions fréquentes {#faq}

**Dois-je reconstruire toutes mes campagnes dans la carte de l’engagement ?**

Nombre La carte des engagements présente une compatibilité descendante complète. Cliquez sur un bouton pour afficher chacune de vos campagnes existantes dans l’interface de la carte de l’engagement visuelle.

**Avoir une carte de l’engagement en Marketo Engage signifie-t-il que je n’aurai plus accès à la structure de dossiers et devront réapprendre à créer une campagne dynamique ?**

Nombre Ce qui est génial avec la carte de l’engagement, c’est qu’elle vous donne le meilleur des deux mondes ; elle est complémentaire à la façon dont vous créez des campagnes actuellement. Vous pouvez choisir si vous souhaitez utiliser l’interface utilisateur existante ou créer/visualiser dans la nouvelle interface utilisateur. Tous les utilisateurs disposeront toujours d’une puissante fonctionnalité de Marketo Engage, désormais complétée par un outil de création visuelle.

**La carte de l’engagement est-elle un module complémentaire payant ?**

Nombre Tous les utilisateurs Marketo Engage existants ou nouveaux sous tous les abonnements auront accès à cette fonctionnalité gratuite.

**En tant qu’administrateur Marketo Engage, suis-je responsable de l’activation/la désactivation de la carte de l’engagement ?**

Nombre La carte de l’engagement sera disponible pour tous les utilisateurs dans leurs instances. Vous ne pourrez pas l’activer/désactiver pour certains utilisateurs, espaces de travail, etc.

**Tout ce qui est actuellement disponible dans les campagnes intelligentes est-il également disponible dans la carte de l’engagement ?**

Oui. La carte de l’engagement présente une parité complète des fonctionnalités avec les campagnes dynamiques.

**En quoi cela diffère-t-il des autres créateurs visuels ?**

Trois éléments clés distinguent la carte de l’engagement :

* Flexibilité : gérez et validez facilement des campagnes interconnectées ou imbriquées de manière approfondie grâce à la visualisation.

* Fonctionnalité : tous les visuels sont prêts à l’emploi, ce qui facilite leur utilisation ; la structure imbriquée vous permet de plonger et d’obtenir l’image entière.

* Pouvoir : Vous conservez toute la sophistication existante du Marketo Engage, maintenant dans un format visuel.

>[!MORELIKETHIS]
>
>* [Onglet Carte d’engagement](/help/marketo/product-docs/core-marketo-concepts/engagement-map/engagement-map-tab.md){target="_blank"}
>* [Onglet Paramètres](/help/marketo/product-docs/core-marketo-concepts/engagement-map/settings-tab.md){target="_blank"}
