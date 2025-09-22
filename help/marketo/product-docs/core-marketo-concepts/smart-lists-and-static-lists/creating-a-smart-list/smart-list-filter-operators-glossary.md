---
unique-page-id: 557312
description: Glossaire Des Opérateurs De Filtre De Liste Dynamique - Documents Marketo - Documentation Du Produit
title: Glossaire des opérateurs de filtre de liste intelligente
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 14%

---

# Glossaire des opérateurs de filtre de liste intelligente {#smart-list-filter-operators-glossary}

Un opérateur/une opératrice fait partie de la liste dynamique qui vous permet d’être plus précis. Il vous permet de décrire votre filtre ou déclencheur dans un langage simple. Les opérateurs disponibles sont différents pour chaque type de champ.

Voici un glossaire décrivant chaque ensemble d’opérateurs.

## Champs de date {#date-fields}

![](assets/smart-list-filter-operators-glossary-1.png)

Lorsque vous choisissez un opérateur, le côté droit change dynamiquement.

<table><thead>
  <tr>
    <th>Opérateur</th>
    <th>Côté Droit</th>
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
    <td>Deux Champs De Date</td>
    <td>Toute date comprise entre deux dates spécifiées</td>
  </tr>
  <tr>
    <td>dans le passé</td>
    <td>Entrée en langage naturel*</td>
    <td>Voir le diagramme ci-dessous</td>
  </tr>
  <tr>
    <td>dans le passé avant</td>
    <td>Entrée en langage naturel*</td>
    <td>Voir le diagramme ci-dessous</td>
  </tr>
  <tr>
    <td>à l’avenir</td>
    <td>Entrée en langage naturel*</td>
    <td>Voir le diagramme ci-dessous</td>
  </tr>
  <tr>
    <td>à l’avenir après</td>
    <td>Entrée en langage naturel*</td>
    <td>Voir le diagramme ci-dessous</td>
  </tr>
  <tr>
    <td>dans la période</td>
    <td>Paramètres prédéfinis (dernier trimestre, hier, etc.)</td>
    <td>Défini dans la liste de sélection</td>
  </tr>
  <tr>
    <td>après</td>
    <td>Date unique</td>
    <td>Tous les enregistrements postérieurs à la date spécifiée</td>
  </tr>
  <tr>
    <td>avant</td>
    <td>Date unique</td>
    <td>Tous les enregistrements avant celui spécifié</td>
  </tr>
  <tr>
    <td>le ou après le</td>
    <td>Date unique</td>
    <td>Identique à « après » mais inclus</td>
  </tr>
  <tr>
    <td>maintenant ou avant</td>
    <td>Date unique</td>
    <td>Identique à « avant » mais inclus</td>
  </tr>
  <tr>
    <td>est vide</td>
    <td>Aucune</td>
    <td>Tous les enregistrements sans date</td>
  </tr>
  <tr>
    <td>n'est pas vide</td>
    <td>Aucune</td>
    <td>Tous les enregistrements avec n’importe quelle date</td>
  </tr>
</tbody></table>

**&#42;** L’entrée en langage naturel est cool. Voici quelques-uns des modèles que vous pouvez entrer :

* 1 heure
* 82 jours
* 3 semaines
* 14 mois
* 1 an

Tapez simplement le numéro et l&#39;unité ensemble et cela fonctionnera !

>[!NOTE]
>
>« Dans le passé » _inclut_ le jour (jusqu’au moment de la création de la liste dynamique, et non après).

>[!CAUTION]
>
>Lorsque vous créez une liste dynamique à l’aide d’un filtre de champ de date (par exemple, date de naissance, date de création SFDC) et que vous utilisez les contraintes **[!UICONTROL avant]**, **[!UICONTROL le ou avant]** ou **[!UICONTROL dans le passé avant]**, la liste dynamique inclut également les personnes qui n’ont aucune valeur dans ce champ de date.

Utilisez le diagramme suivant pour comprendre la différence entre les opérateurs de date.

![](assets/smart-list-filter-operators-glossary-2.png)

>[!NOTE]
>
>**Exemple**
>
>Les champs de date peuvent devenir difficiles à gérer lorsque vous travaillez avec des événements passés et futurs. Voici quelques exemples.
>
>**[!UICONTROL Dans le passé]**
>
>Pour votre nouvelle promotion, utilisez cet opérateur pour envoyer des e-mails uniquement aux personnes qui ne se sont pas inscrites ou n&#39;ont pas renouvelé votre service dans l&#39;année ou qui n&#39;ont jamais été abonnées.
>
>**[!UICONTROL Dans le futur après]**
>
>Supposons que vous souhaitiez voir les clients dont le renouvellement est prévu dans 90 jours. Vous devez utiliser deux filtres distincts. Utilisez d’abord « Dans le futur après 90 jours », puis « Dans les 91 jours à venir ». Cela s&#39;appliquerait à toute personne qui a une date dans 90 jours.

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
    <td>Premières lettres de correspondance de chaîne</td>
  </tr>
  <tr>
    <td>ne commence pas par</td>
    <td>Les premières lettres de la chaîne NE CORRESPONDENT PAS</td>
  </tr>
  <tr>
    <td>contient</td>
    <td>Toutes les lettres ensemble dans la correspondance de chaîne (exemple : californie, fortune, par conséquent)</td>
  </tr>
  <tr>
    <td>ne contient pas</td>
    <td>Aucune lettre ensemble dans la correspondance de chaîne. (verso de « contient »)</td>
  </tr>
  <tr>
    <td>est vide</td>
    <td>Enregistrements sans valeur (NULL)</td>
  </tr>
  <tr>
    <td>n'est pas vide</td>
    <td>Enregistrements avec UNE VALEUR QUELCONQUE</td>
  </tr>
</tbody>
</table>

>[!TIP]
>
>Utilisez des opérateurs positifs plutôt que négatifs. Les filtres « n’est pas » doivent rechercher l’ensemble du jeu de données dans votre instance, ce qui peut prendre énormément de temps. Les filtres positifs « est » peuvent utiliser des algorithmes de recherche plus efficaces.

## Champs Entiers {#integer-fields}

![](assets/smart-list-filter-operators-glossary-4.png)

<table><thead>
  <tr>
    <th>Opérateur</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>est</td>
    <td>Correspondance exacte du nombre ( = 0 renvoie les deux prospects avec 0 et NULL)</td>
  </tr>
  <tr>
    <td>n'est pas</td>
    <td>Tout sauf une correspondance de nombre exacte</td>
  </tr>
  <tr>
    <td>entre</td>
    <td>Définir deux valeurs pour trouver tout le monde entre les deux (inclus)</td>
  </tr>
  <tr>
    <td>supérieur à</td>
    <td>Au-dessus du spécifié</td>
  </tr>
  <tr>
    <td>inférieur à</td>
    <td>Inférieur au spécifié</td>
  </tr>
  <tr>
    <td>au moins</td>
    <td>Au-dessus du spécifié (inclus)</td>
  </tr>
  <tr>
    <td>au plus</td>
    <td>Inférieur à l’élément spécifié (inclus)</td>
  </tr>
  <tr>
    <td>est vide</td>
    <td>Enregistrements sans valeur (NULL) - zéro est un nombre, il n'est pas NULL</td>
  </tr>
  <tr>
    <td>n'est pas vide</td>
    <td>Enregistrements avec TOUTE valeur (y compris zéro)</td>
  </tr>
</tbody>
</table>

Comme vous pouvez le constater, ces opérateurs permettent de parler facilement le Marketo avec aisance !
