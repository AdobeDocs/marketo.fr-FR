---
unique-page-id: 557312
description: Opérateurs de filtre de Liste dynamique Glossaire - Documents marketing - Documentation du produit
title: Glossaire des opérateurs de filtre de Liste dynamique
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---


# Opérateurs de filtre de Liste dynamique Glossaire {#smart-list-filter-operators-glossary}

Un opérateur fait partie de la liste intelligente qui vous aide à obtenir des informations spécifiques. Il vous permet de décrire votre filtre ou déclencheur en langage simple. Les opérateurs disponibles sont différents pour chaque type de champ.

Voici un glossaire décrivant chaque ensemble d&#39;opérateurs.

## Champs de date {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Lorsque vous choisissez un opérateur, le côté droit change dynamiquement.

| Opérateur | Côté droit | Description |
|---|---|---|
| is | Date unique | Correspondance de date exacte |
| is not | Date unique | Toute date SAUF celle spécifiée |
| between | Deux champs de date | Toute date comprise entre deux dates spécifiées |
| dans le passé | Entrée de langue naturelle* | Voir le diagramme ci-dessous |
| dans le passé | Entrée de langue naturelle* | Voir le diagramme ci-dessous |
| futur | Entrée de langue naturelle* | Voir le diagramme ci-dessous |
| dans le futur après | Entrée de langue naturelle* | Voir le diagramme ci-dessous |
| dans le délai | Paramètres prédéfinis (dernier trimestre, hier, etc.) | Défini dans la liste de sélection |
| after | Date unique | Tous les enregistrements après la date spécifiée |
| before | Date unique | Tous les enregistrements avant celui spécifié |
| le ou après | Date unique | Identique à &quot;after&quot; mais inclusive |
| le ou avant | Date unique | Identique à &quot;before&quot; mais inclusive |
| est vide | Aucun | Tous les enregistrements sans date |
| n’est pas vide | Aucun | Tous les enregistrements avec une date quelconque |

* L&#39;entrée du langage naturel est cool. Vous pouvez entrer quelques-uns des modèles suivants :

* 1 heure
* 82 jours
* 3 semaines
* 14 mois
* 1 an

Il suffit de taper le numéro et l&#39;unité ensemble et ça marchera !

>[!NOTE]
>
>&quot;Dans le passé&quot; **fait** inclure le jour (jusqu&#39;à l&#39;heure, pas après) que vous avez créé votre liste intelligente.

>[!CAUTION]
>
>Lorsque vous créez une liste dynamique à l’aide d’un filtre de champ de date (par exemple, Date de naissance, Date de création de la DDC) et que vous utilisez les contraintes **avant** ou **le ou avant**, la liste dynamique inclut également les personnes qui n’ont aucune valeur dans ledit champ de date.

Utilisez le diagramme suivant pour comprendre la différence entre les opérateurs de date.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Exemple**
>
>Les champs de date peuvent devenir délicats lorsque vous travaillez sur des événements passés et futurs. Voici quelques exemples.
>
>**Dans le passé**
>
>Pour votre nouvelle promotion, utilisez cet opérateur pour envoyer des courriels uniquement aux personnes qui ne se sont pas abonnées à votre service ou qui n&#39;ont pas renouvelé votre service dans un délai d&#39;un an ou qui n&#39;ont jamais été abonnées.
>
>**Dans le futur après**
>
>Supposons que vous souhaitiez voir les clients qui sont en renouvellement dans 90 jours. Vous utiliseriez deux filtres distincts. Utilisez d&#39;abord &quot;Dans l&#39;avenir après 90 jours&quot;, puis &quot;Dans l&#39;avenir 91 jours&quot;. Cela capturerait quiconque aura une date dans 90 jours.

## Champs de chaîne {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Opérateur | Description |
|---|---|
| is | Correspondance exacte (non sensible à la casse) |
| is not | Tout sauf une correspondance exacte |
| débuts avec | Première correspondance de chaîne |
| non débuts avec | Les premières lettres de la chaîne NE correspondent PAS |
| contient | Toutes les lettres regroupées dans la chaîne correspondent (exemple : californie, fortune, par là) |
| not contient | Aucune lettre ne correspond dans la chaîne. (inversée de &quot;contient&quot;) |
| est vide | Enregistrements sans valeur (NULL) |
| n’est pas vide | Enregistrements avec une valeur TOUT |

>[!TIP]
>
>Utilisez des opérateurs positifs plutôt que négatifs. Les filtres &quot;n’est pas&quot; doivent rechercher l’ensemble des données de votre instance, ce qui peut prendre beaucoup de temps. Les filtres positifs &quot;est&quot; peuvent exploiter des algorithmes de recherche plus efficaces.

## Champs entiers {#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Opérateur</th> 
   <th colspan="1" rowspan="1">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">is</td> 
   <td colspan="1" rowspan="1">Correspondance exacte du nombre ( = 0 renvoie les deux pistes avec 0 <em>et </em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">is not</td> 
   <td colspan="1" rowspan="1">Tout SAUF la correspondance exacte du nombre</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">between</td> 
   <td colspan="1" rowspan="1">Définissez deux valeurs pour rechercher tous les intermédiaires (inclus)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">supérieur à</td> 
   <td colspan="1" rowspan="1">Au-dessus de la valeur spécifiée</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">inférieur à</td> 
   <td colspan="1" rowspan="1">Inférieur à la valeur spécifiée</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">au moins</td> 
   <td colspan="1" rowspan="1">Au-dessus de la valeur spécifiée (incluse)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">au plus</td> 
   <td colspan="1" rowspan="1">Inférieur à la valeur spécifiée (incluse)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">est vide</td> 
   <td colspan="1" rowspan="1">Enregistrements sans valeur (NULL) - zéro est un nombre, <em>pas</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">n’est pas vide</td> 
   <td colspan="1" rowspan="1">Enregistrements avec TOUTE valeur (y compris zéro)</td> 
  </tr> 
 </tbody> 
</table>

Comme vous pouvez le voir, ces opérateurs permettent de parler facilement à Marketo-ese avec aisance !
