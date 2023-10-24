---
unique-page-id: 557312
description: Opérateurs de filtre de liste dynamique - Documentation Marketo - Documentation du produit
title: Glossaire des opérateurs de filtre de liste dynamique
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 12%

---

# Glossaire des opérateurs de filtre de liste dynamique {#smart-list-filter-operators-glossary}

Un opérateur fait partie de la liste dynamique qui vous permet d’obtenir des informations spécifiques. Il vous permet de décrire votre filtre ou votre déclencheur dans un langage simple. Les opérateurs disponibles sont différents pour chaque type de champ.

Voici un glossaire décrivant chaque ensemble d&#39;opérateurs.

## Champs de date {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Lorsque vous choisissez un opérateur, le côté droit change dynamiquement.

| Opérateur | Côté droit | Description |
|---|---|---|
| est | Date unique | Correspondance exacte de la date |
| n’est pas | Date unique | Toute date SAUF celle spécifiée |
| entre | Deux champs de date | Toute date incluant et comprise entre deux dates spécifiées |
| dans le passé | Entrée du langage naturel&#42; | Voir diagramme ci-dessous |
| dans le passé avant | Entrée du langage naturel&#42; | Voir diagramme ci-dessous |
| à l’avenir | Entrée du langage naturel&#42; | Voir diagramme ci-dessous |
| à l’avenir après | Entrée du langage naturel&#42; | Voir diagramme ci-dessous |
| dans la période | Paramètres prédéfinis (dernier trimestre, hier, etc.) | Défini dans la liste de sélection |
| après | Date unique | Tous les enregistrements après la date spécifiée |
| avant | Date unique | Tous les enregistrements avant celui spécifié |
| le ou après le | Date unique | Identique à &quot;after&quot; mais inclusif |
| maintenant ou avant | Date unique | Identique à &quot;l&#39;avant&quot; mais inclusif |
| est vide | Aucun | Tous les enregistrements sans date |
| n’est pas vide | Aucun | Tous les enregistrements avec une date quelconque |

&#42; L&#39;entrée du langage naturel est cool. Voici quelques-uns des modèles que vous pouvez saisir :

* 1 heure
* 82 jours
* 3 semaines
* 14 mois
* 1 an

Il suffit de taper le numéro et l&#39;unité pour que ça marche !

>[!NOTE]
>
>&quot;Dans le passé&quot; _does_ incluez le jour (jusqu’à l’heure, et non après) où vous créez votre liste dynamique.

>[!CAUTION]
>
>Lorsque vous créez une liste dynamique à l’aide d’un filtre de champ de date (par exemple, Date de naissance, Date de création de la collecte de données régionale) et que vous utilisez les contraintes **[!UICONTROL before]**, **[!UICONTROL le ou avant]**, ou **[!UICONTROL auparavant]**, la liste dynamique inclut également les personnes qui n’ont aucune valeur dans ce champ de date.

Utilisez le diagramme suivant pour comprendre la différence entre les opérateurs de date.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Exemple**
>
>Les champs de date peuvent devenir délicats lorsque vous travaillez avec des événements passés et futurs. Voici quelques exemples.
>
>**[!UICONTROL Avant]**
>
>Pour votre nouvelle promotion, utilisez cet opérateur pour envoyer des emails uniquement aux personnes qui ne se sont pas abonnées à ou qui n&#39;ont pas renouvelé votre service dans un délai d&#39;un an ou qui n&#39;ont jamais été abonnés.
>
>**[!UICONTROL À venir après]**
>
>Supposons que vous souhaitiez voir des clients qui seront renouvelés dans 90 jours. Vous utiliserez deux filtres distincts. Utilisez d’abord &quot;Dans l’avenir après 90 jours&quot;, puis &quot;Dans les 91 prochains jours&quot;. Cela capturerait quiconque aura une date dans 90 jours.

## Champs de chaîne {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Opérateur | Description |
|---|---|
| est | Correspondance exacte (non sensible à la casse) |
| n’est pas | Tout sauf une correspondance exacte |
| commence par | Première correspondance de chaînes |
| ne commence pas par | Les premières lettres de la chaîne NE correspondent PAS |
| contient | Toutes les lettres ensemble dans la correspondance de chaîne (par exemple : california, fortune, etc.) |
| ne contient pas | Aucune lettre ne correspond dans la chaîne. (inversé de &quot;contains&quot;) |
| est vide | Enregistrements sans valeur (NULL) |
| n’est pas vide | Enregistrements avec TOUTE valeur |

>[!TIP]
>
>Utilisez des opérateurs positifs plutôt que négatifs. Les filtres &quot;N’est pas&quot; doivent rechercher l’ensemble des données de votre instance, ce qui peut prendre beaucoup de temps. Les filtres &quot;is&quot; positifs peuvent utiliser des algorithmes de recherche plus efficaces.

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
   <td colspan="1" rowspan="1">est</td> 
   <td colspan="1" rowspan="1">Correspondance exacte du nombre ( = 0) renvoie les deux pistes avec 0 <em>et</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">n’est pas</td> 
   <td colspan="1" rowspan="1">Tout SAUF une correspondance de nombre exacte</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">entre</td> 
   <td colspan="1" rowspan="1">Définissez deux valeurs pour rechercher toutes les personnes entre les deux (inclusif).</td> 
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
   <td colspan="1" rowspan="1">Enregistrements sans valeur (NULL) - zéro est un nombre, c’est <em>not</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">n’est pas vide</td> 
   <td colspan="1" rowspan="1">Enregistrements avec TOUTE valeur (y compris zéro)</td> 
  </tr> 
 </tbody> 
</table>

Comme vous pouvez le voir, ces opérateurs permettent de parler facilement Marketo-ese avec fluidité !
