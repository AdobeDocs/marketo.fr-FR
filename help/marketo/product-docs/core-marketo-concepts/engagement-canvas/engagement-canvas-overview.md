---
description: Présentation du canevas d’engagement - Documents Marketo - Documentation du produit
title: Présentation du canevas d’engagement
hide: true
hidefromtoc: true
exl-id: 0b445ac7-bfa4-4f86-bb92-86d4d982555e
source-git-commit: 60b3abf6639e4a257b37fd3ace3cb5a3a6c318fb
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Présentation du canevas d’engagement {#engagement-canvas-overview}

>[!AVAILABILITY]
>
>Cette fonctionnalité est actuellement disponible pour les campagnes dynamiques. Il n’est pas disponible pour les programmes.

Le canevas d’engagement vous permet de créer des campagnes dynamiques réutilisables à l’aide de visuels intuitifs. Il offre une compatibilité ascendante complète avec toutes les campagnes dynamiques de Marketo Engage existantes, sans perte de fonctionnalités actuelles.

CAPTURE D’ÉCRAN

## Accès au canevas d’engagement {#accessing-engagement-canvas}

Accédez à une campagne existante, puis cliquez sur le bouton **Canevas d’engagement** bouton .

CAPTURE D’ÉCRAN

Deux onglets s’affichent une fois dans la zone de travail Engagement : [Canevas d’engagement](/help/marketo/product-docs/core-marketo-concepts/engagement-canvas/engagement-canvas-tab.md){target="_blank"} and [Settings](/help/marketo/product-docs/core-marketo-concepts/engagement-canvas/engagement-canvas-tab.md){target="_blank"}.

CAPTURE D’ÉCRAN

EN-TÊTE - DESCRIPTIONS DE CARTE ? - LOPA CONFIRME

**Triggers**: Dans les campagnes qui incluent des déclencheurs, la zone de travail dispose d’une carte &quot;Présentation du déclencheur&quot;. Si vous cliquez sur cette option, une carte s’affiche pour chaque déclencheur, ainsi qu’un panneau déroulant contenant des informations supplémentaires.

**Filtres**: Dans les campagnes qui incluent des filtres, la zone de travail contient une carte pour chacune d’elles. Si vous cliquez dessus, un panneau déroulant contenant des informations supplémentaires s’affiche.

**Étapes de flux**: Chaque campagne comprend une carte pour chaque étape de flux. Si vous cliquez dessus, un panneau déroulant contenant des informations supplémentaires s’affiche.

**Choix**: Si une étape de flux comprend un ou plusieurs choix, un clic sur la carte de flux affiche une carte pour chaque choix, ainsi qu’un panneau de sortie avec des informations supplémentaires.

## Campagnes imbriquées {#nested-campaigns}

* Si une campagne comprend une étape de flux Demander ou Exécuter la campagne , un clic sur la carte de flux affiche les détails de l’opération en cours d’appel, ainsi qu’un panneau de sortie avec des informations supplémentaires. (La campagne imbriquée comprend également une pilule de fermeture, si vous cliquez dessus, les cartes associées à la campagne imbriquée sont réduites.) !!!!!!!!!!!! - REMODER OU SUPPRIMER - LOPA CONFIRME

* Si une campagne comprend une étape de flux Demander ou Exécuter une campagne avec des choix, un clic sur la carte de flux affiche une carte de choix, ainsi qu’un panneau d’affichage avec des informations supplémentaires sur les choix. Cliquez sur chaque carte de choix pour afficher les détails de la campagne en cours d’appel, ainsi qu’un panneau déroulant contenant des informations supplémentaires.

* En outre, si l’une des campagnes imbriquées comporte une étape de flux Demander ou Exécuter la campagne , cliquez sur la carte de flux pour afficher les détails de la campagne. Il en va de même lorsque l’étape de flux comprend des choix.

## Navigation supérieure {#top-navigation}

CAPTURE D’ÉCRAN

Le volet de navigation supérieur comprend les fonctionnalités suivantes :

!!!!! CAPTURE D’ÉCRAN DÉPASSÉE - NOUVEAU GRAB

* Nom de la campagne et accès au modal &quot;Modifier la campagne&quot;, vous pouvez modifier le nom et la description de la campagne ici.

* L’état et le type de campagne de la campagne seront reflétés sous le nom de la campagne.

* Bouton Activer/Désactiver pour les campagnes de déclenchement

* Modifier la liste dynamique : vous accédez à l’interface Liste dynamique dans un nouvel onglet où vous pouvez ajouter ou modifier votre liste dynamique.

* Modifier le flux : vous accédez à l’interface Flux dans un nouvel onglet où vous pouvez ajouter ou modifier votre liste dynamique.

* Exporter : télécharge une image de visualisation de campagne. La version téléchargée reflète les branches que vous avez développées.

* Afficher les membres de campagne : un nouvel onglet contenant les détails des membres de campagne s’ouvre.

>[!NOTE]
>
>Les modifications apportées dans un onglet de liste dynamique et de flux ouvert seront répercutées dans l’onglet Canevas d’engagement lors de l’actualisation. Elle ne sera pas mise à jour automatiquement. Les mises à jour et modifications enregistrées automatiquement sont répercutées.

## Questions fréquentes {#faq}

**Dois-je reconstruire toutes mes campagnes dans la zone de travail Engagement ?**

Nombre Le canevas d’engagement est entièrement rétrocompatible. Cliquez sur un bouton pour afficher chacune de vos campagnes existantes dans l’interface du Canevas d’engagement visuel.

**Avoir un canevas d’engagement en Marketo Engage signifie-t-il que je n’aurai plus accès à la structure de dossiers et devront réapprendre à créer une campagne dynamique ?**

Nombre Le canevas d’engagement offre un meilleur des deux mondes. il est complémentaire à la manière dont vous créez des campagnes actuellement. Vous pouvez choisir si vous souhaitez utiliser l’interface utilisateur existante ou créer/visualiser dans la nouvelle interface utilisateur. Tous les utilisateurs disposeront toujours d’une puissante fonctionnalité de Marketo Engage, désormais complétée par un outil de création visuelle.

**Le canevas d’engagement est-il un module complémentaire payant ?**

Nombre Tous les utilisateurs Marketo Engage existants ou nouveaux sous tous les abonnements auront accès à cette fonctionnalité gratuite.

**En tant qu’administrateur Marketo Engage, suis-je responsable de l’activation/désactivation du canevas d’engagement ?**

Nombre Le canevas d’engagement sera disponible pour tous les utilisateurs dans leurs instances. Vous ne pourrez pas l’activer/désactiver pour certains utilisateurs, espaces de travail, etc.

**Tout ce qui est actuellement disponible dans les campagnes dynamiques est-il également disponible dans la zone de travail Engagement ?**

Oui. Le canevas d’engagement offre une parité complète des fonctionnalités avec les campagnes dynamiques.

**En quoi cela diffère-t-il des autres créateurs visuels ?**

Trois éléments clés distinguent le canevas d’engagement :

* Flexibilité : Gérez et validez facilement des campagnes interconnectées ou imbriquées de manière approfondie grâce à la visualisation.

* Fonctionnalité : Tous les visuels sont prêts à l’emploi, ce qui facilite leur utilisation. la structure imbriquée vous permet de plonger et d&#39;obtenir le tableau entier.

* Puissance : Vous conservez toute la sophistication existante du Marketo Engage, maintenant dans un format visuel.

>[!MORELIKETHIS]
>
>* [Onglet Canevas d’engagement](/help/marketo/product-docs/core-marketo-concepts/engagement-canvas/engagement-canvas-tab.md){target="_blank"}
>* [Onglet Paramètres](/help/marketo/product-docs/core-marketo-concepts/engagement-canvas/settings-tab.md){target="_blank"}
