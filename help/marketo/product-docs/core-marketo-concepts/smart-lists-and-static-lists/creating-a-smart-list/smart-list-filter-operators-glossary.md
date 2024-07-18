---
unique-page-id: 557312
description: Opérateurs de filtre de liste dynamique - Documentation Marketo - Documentation du produit
title: Glossaire des opérateurs de filtre de liste dynamique
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 13%

---

# Glossaire des opérateurs de filtre de liste dynamique {#smart-list-filter-operators-glossary}

Un opérateur fait partie de la liste dynamique qui vous permet d’obtenir des informations spécifiques. Il vous permet de décrire votre filtre ou votre déclencheur dans un langage simple. Les opérateurs disponibles sont différents pour chaque type de champ.

Voici un glossaire décrivant chaque ensemble d&#39;opérateurs.

## Champs de date {#date-fields}

![](assets/smart-list-filter-operators-glossary-1.png)

Lorsque vous choisissez un opérateur, le côté droit change dynamiquement.

<table><thead>
  <tr>
    <th>Opérateur</th>
    <th>Côté droit</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>est</td>
    <td>Date unique</td>
    <td>Correspondance exacte de la date</td>
  </tr>
  <tr>
    <td>n'est pas</td>
    <td>Date unique</td>
    <td>Toute date SAUF celle spécifiée</td>
  </tr>
  <tr>
    <td>entre</td>
    <td>Deux champs de date</td>
    <td>Toute date incluant et comprise entre deux dates spécifiées</td>
  </tr>
  <tr>
    <td>dans le passé</td>
    <td>Entrée du langage naturel*</td>
    <td>Voir diagramme ci-dessous</td>
  </tr>
  <tr>
    <td>dans le passé avant</td>
    <td>Entrée du langage naturel*</td>
    <td>Voir diagramme ci-dessous</td>
  </tr>
  <tr>
    <td>à l’avenir</td>
    <td>Entrée du langage naturel*</td>
    <td>Voir diagramme ci-dessous</td>
  </tr>
  <tr>
    <td>à l’avenir après</td>
    <td>Entrée du langage naturel*</td>
    <td>Voir diagramme ci-dessous</td>
  </tr>
  <tr>
    <td>dans la période</td>
    <td>Paramètres prédéfinis (dernier trimestre, hier, etc.)</td>
    <td>Défini dans la liste de sélection</td>
  </tr>
  <tr>
    <td>après</td>
    <td>Date unique</td>
    <td>Tous les enregistrements après la date spécifiée</td>
  </tr>
  <tr>
    <td>avant</td>
    <td>Date unique</td>
    <td>Tous les enregistrements avant celui spécifié</td>
  </tr>
  <tr>
    <td>le ou après le</td>
    <td>Date unique</td>
    <td>Identique à "after" mais inclusif</td>
  </tr>
  <tr>
    <td>maintenant ou avant</td>
    <td>Date unique</td>
    <td>Identique à "l'avant" mais inclusif</td>
  </tr>
  <tr>
    <td>est vide</td>
    <td>Aucun</td>
    <td>Tous les enregistrements sans date</td>
  </tr>
  <tr>
    <td>n'est pas vide</td>
    <td>Aucun</td>
    <td>Tous les enregistrements avec une date quelconque</td>
  </tr>
</tbody></table>

**&#42;** L’entrée du langage naturel est cool. Voici quelques-uns des modèles que vous pouvez saisir :

* 1 heure
* 82 jours
* 3 semaines
* 14 mois
* 1 an

Il suffit de taper le numéro et l&#39;unité pour que ça marche !

>[!NOTE]
>
>&quot;Dans le passé&quot; _est_ inclut le jour (jusqu’à l’heure, et non après) que vous créez votre liste dynamique.

>[!CAUTION]
>
>Lorsque vous créez une liste dynamique à l’aide d’un filtre de champ de date (par exemple, Date de naissance, Date de création de la SFDC) et que vous utilisez les contraintes **[!UICONTROL avant]**, **[!UICONTROL au plus tard]** ou **[!UICONTROL avant]**, la liste dynamique inclut également les personnes qui n’ont aucune valeur dans ce champ de date.

Utilisez le diagramme suivant pour comprendre la différence entre les opérateurs de date.

![](assets/smart-list-filter-operators-glossary-2.png)

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
>**[!UICONTROL À l’avenir après]**
>
>Supposons que vous souhaitiez voir des clients qui seront renouvelés dans 90 jours. Vous utiliserez deux filtres distincts. Utilisez d’abord &quot;Dans l’avenir après 90 jours&quot;, puis &quot;Dans les 91 prochains jours&quot;. Cela capturerait quiconque aura une date dans 90 jours.

## Champs de chaîne {#string-fields}

![](assets/smart-list-filter-operators-glossary-3.png)

<table><thead>
  <tr>
    <th>Opérateur</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>est</td>
    <td>Correspondance exacte (non sensible à la casse)</td>
  </tr>
  <tr>
    <td>n'est pas</td>
    <td>Tout sauf une correspondance exacte</td>
  </tr>
  <tr>
    <td>commence par</td>
    <td>Première correspondance de chaînes</td>
  </tr>
  <tr>
    <td>ne commence pas par</td>
    <td>Les premières lettres de la chaîne NE correspondent PAS</td>
  </tr>
  <tr>
    <td>contient</td>
    <td>Toutes les lettres ensemble dans la correspondance de chaîne (par exemple : california, fortune, etc.)</td>
  </tr>
  <tr>
    <td>ne contient pas</td>
    <td>Aucune lettre ne correspond dans la chaîne. (inversé de "contains")</td>
  </tr>
  <tr>
    <td>est vide</td>
    <td>Enregistrements sans valeur (NULL)</td>
  </tr>
  <tr>
    <td>n'est pas vide</td>
    <td>Enregistrements avec TOUTE valeur</td>
  </tr>
</tbody>
</table>

>[!TIP]
>
>Utilisez des opérateurs positifs plutôt que négatifs. Les filtres &quot;N’est pas&quot; doivent rechercher l’ensemble des données de votre instance, ce qui peut prendre beaucoup de temps. Les filtres &quot;is&quot; positifs peuvent utiliser des algorithmes de recherche plus efficaces.

## Champs entiers {#integer-fields}

![](assets/smart-list-filter-operators-glossary-4.png)

<table><thead>
  <tr>
    <th>Opérateur</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>est</td>
    <td>Correspondance exacte du nombre ( = 0) renvoie les deux pistes avec 0 et NULL.</td>
  </tr>
  <tr>
    <td>n'est pas</td>
    <td>Tout SAUF une correspondance de nombre exacte</td>
  </tr>
  <tr>
    <td>entre</td>
    <td>Définissez deux valeurs pour rechercher toutes les personnes entre les deux (inclusif).</td>
  </tr>
  <tr>
    <td>supérieur à</td>
    <td>Au-dessus de la valeur spécifiée</td>
  </tr>
  <tr>
    <td>inférieur à</td>
    <td>Inférieur à la valeur spécifiée</td>
  </tr>
  <tr>
    <td>au moins</td>
    <td>Au-dessus de la valeur spécifiée (incluse)</td>
  </tr>
  <tr>
    <td>au plus</td>
    <td>Inférieur à la valeur spécifiée (incluse)</td>
  </tr>
  <tr>
    <td>est vide</td>
    <td>Enregistrements sans valeur (NULL) - zéro est un nombre, il n’est pas NULL</td>
  </tr>
  <tr>
    <td>n'est pas vide</td>
    <td>Enregistrements avec TOUTE valeur (y compris zéro)</td>
  </tr>
</tbody>
</table>

Comme vous pouvez le voir, ces opérateurs permettent de parler facilement Marketo-ese avec fluidité !
