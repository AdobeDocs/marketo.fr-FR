---
description: Onglet Nom - Documents Marketo - Documentation du produit
title: Onglet Nom
hide: true
hidefromtoc: true
exl-id: f54b9258-451b-4607-b5a9-f8627c6f420a
source-git-commit: 50f6f82e0e7e55007905f824dea7707a1cf25d09
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 0%

---

# Onglet Nom {#name-tab}

Les parcours sont représentés par le biais d’une série de cartes de déclencheur, de filtre et de flux. Cliquez sur chacune de ces cartes pour ouvrir le panneau déroulant correspondant.

Présentation du déclencheur : La carte affiche le nombre de déclencheurs dans la campagne spécifique. Cliquer sur cette carte se développe également pour afficher les cartes de détails Trigger et ouvrir simultanément le panneau de diapositives avec les informations suivantes :

Campagne à laquelle le déclencheur appartient

Bouton Modifier le déclencheur pour accéder à l’onglet Liste dynamique

Liste des noms des déclencheurs

CAPTURE D’ÉCRAN

Détails du déclencheur : La carte affiche le nom du déclencheur. Cliquez sur cette carte pour ouvrir le panneau de visualisation avec les informations suivantes :

Campagne à laquelle le déclencheur appartient

Bouton Modifier le déclencheur pour accéder à l’onglet Liste dynamique

Liste des contraintes associées au déclencheur

CAPTURE D’ÉCRAN

Filtres : Cliquez sur cette carte pour ouvrir le panneau de visualisation avec les informations suivantes :

Campagne à laquelle le déclencheur appartient

Bouton Modifier le filtre pour accéder à l’onglet Liste dynamique

Nombre estimé de personnes qui remplissent les critères du filtre

Liste des filtres et leurs contraintes respectives

CAPTURE D’ÉCRAN

Etapes de flux : Si une étape de flux n’inclut aucun choix, la carte affiche les attributs associés à l’étape de flux. Cliquez sur la carte pour ouvrir le panneau de visualisation avec les informations suivantes :

Campagne à laquelle l’étape Flux appartient

Bouton Modifier le flux pour accéder à l’onglet Flux

Liste des attributs associés à l’étape de flux

CAPTURE D’ÉCRAN

Etapes de flux : Si une étape de flux comprend des choix, la carte indique le nom de l’étape de flux. Cliquez sur la carte pour ouvrir le panneau de visualisation avec les informations suivantes :

Campagne à laquelle l’étape Flux appartient

Bouton Modifier le flux pour accéder à l’onglet Flux

Liste des conditions de choix associées à l’étape de flux

CAPTURE D’ÉCRAN

Étape de flux pour exécuter et demander des campagnes :

Si l’étape de flux Exécuter ou Demander la campagne ne comporte aucun choix, la carte affichera le nom de la campagne. Cliquez sur la carte pour ouvrir le panneau de visualisation avec les informations suivantes :

Campagne à laquelle appartient l’étape de flux

Bouton Modifier le flux pour accéder à l’onglet Flux

Liste des attributs associés à l’étape de flux

Bouton Afficher la liste qui affiche la liste des campagnes qui utilisent la requête spécifique ou exécutent une campagne

Remarque : Vous pouvez modifier l’étape de flux à partir d’une Principale campagne. Pour modifier les campagnes imbriquées, vous devez accéder à la campagne à partir du lien hypertexte du panneau de sortie.

CAPTURE D’ÉCRAN

CAPTURE D’ÉCRAN

Si l’étape de flux Exécuter ou Demander la campagne comprend des choix, la carte affichera le nom de la campagne. Cliquez sur la carte pour ouvrir le panneau de visualisation avec les informations suivantes :

Campagne à laquelle appartient l’étape de flux

Bouton Modifier le flux pour accéder à l’onglet Flux

Liste des conditions de choix associées à l’étape de flux

CAPTURE D’ÉCRAN

CAPTURE D’ÉCRAN

Si une campagne d’exécution ou de requête comprend des choix, un clic sur la carte de flux se développe afin d’afficher tous les choix dans des cartes individuelles.

Cliquez sur la carte de choix pour développer la campagne associée au choix spécifique et ouvrir simultanément le panneau de visualisation avec les informations suivantes :

Campagne à laquelle le choix appartient

Bouton Modifier le choix pour accéder à l’onglet Flux

Liste des conditions de choix associées à l’étape de flux

Bouton Afficher la liste qui affiche la liste des campagnes qui utilisent la requête spécifique ou exécutent une campagne

CAPTURE D’ÉCRAN

Visualisation de l’exécution de campagne imbriquée (nouvelle section)

Exécutez les campagnes exécutées en série avec la campagne parente, c’est-à-dire les pistes qui remplissent les critères d’une campagne exécutable, effectuez toutes les étapes de flux de la campagne et revenez à la Principale campagne pour continuer à suivre les étapes de flux de cette campagne.

Voici un exemple de campagne dynamique &quot;Campagne A&quot; qui comprend une étape d’exécution du flux de campagne. Vous pouvez considérer la &quot;Campagne A&quot; comme votre Principale campagne.

CAPTURE D’ÉCRAN

Cliquez sur la carte d’exécution du flux de campagne pour développer et afficher les détails de la &quot;campagne B&quot;.

La campagne B comprend un filtre qui s’étend à une audience non qualifiée et non qualifiée.

L’audience qualifiée passe en revue les étapes de flux associées à la &quot;campagne B&quot;.

L’ensemble de l’audience (qualifiée et non qualifiée) revient à &quot;Campagne A&quot; et passe à l’étape de flux suivante.

CAPTURE D’ÉCRAN

Vous pouvez cliquer sur l’étape Exécuter la campagne dans &quot;Campagne B&quot;, qui s’agrandit pour afficher les cartes de choix et la campagne associées à chaque choix.

CAPTURE D’ÉCRAN

Visualisation de la campagne de requête (nouvelle section)

Les campagnes de requête s’exécutent en parallèle de la campagne parente, c’est-à-dire que les pistes qui remplissent les critères d’une campagne de requête effectuent toutes les étapes de flux de la campagne et quittent la campagne. En parallèle, le même ensemble de pistes passe également par les étapes de flux de la campagne Principale.

Voici un exemple de campagne dynamique &quot;Campagne A&quot; qui comprend une étape de flux de campagne de requête. Vous pouvez considérer la &quot;Campagne A&quot; comme votre Principale campagne.

CAPTURE D’ÉCRAN

Cliquez sur la carte de flux de campagne de requête pour afficher les détails de la &quot;campagne B&quot;.

La campagne B comprend un filtre qui s’étend à une audience qualifiée.

L’audience qualifiée passe en revue les étapes de flux associées à la &quot;campagne B&quot;.

En parallèle, toutes les audiences passent aux étapes de flux suivantes dans &quot;Campagne A&quot;

CAPTURE D’ÉCRAN

Vous pouvez approfondir l’analyse des campagnes imbriquées si l’une des étapes de flux inclut une autre campagne de requête en cliquant sur la carte de flux pour afficher les détails de la campagne.

CAPTURE D’ÉCRAN

Voici un exemple de campagne de requête avec choix.

CAPTURE D’ÉCRAN

Gestion des erreurs :

Les erreurs dans les étapes de flux et de liste dynamique sont mises en surbrillance par l’icône d’erreur dans la carte. En outre, le message d’erreur correspondant sera reflété dans le panneau de sortie.

Voici un exemple d’erreur dans le déclencheur qui sera indiqué dans la carte d’aperçu du déclencheur, le panneau déroulant ainsi que la carte de déclencheur détaillée.

CAPTURE D’ÉCRAN

CAPTURE D’ÉCRAN

Une erreur dans la carte de filtre peut inclure

Erreur dans la liste dynamique, ce qui empêchera l’affichage de l’audience qualifiée

Erreur dans la logique de filtre

Erreur dans les contraintes ou absence de contraintes dans un ou plusieurs filtres

CAPTURE D’ÉCRAN

Si vous ne saisissez pas de valeurs (attributs), elles ne seront pas marquées comme des erreurs, car elles continueront à fonctionner comme dans l’onglet Flux . Par conséquent, les campagnes existantes ne seront pas perturbées. Cependant, lorsque les étapes de flux n’incluent aucun attribut, elles s’affichent sous la forme d’avertissements.

CAPTURE D’ÉCRAN

Remarque : Les erreurs d’une campagne imbriquée ne seront pas visibles tant que vous n’aurez pas cliqué pour développer la campagne imbriquée.
