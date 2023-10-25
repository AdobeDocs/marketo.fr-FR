---
unique-page-id: 2949891
description: Présentation des listes statiques - Documents Marketo - Documentation du produit
title: Présentation des listes statiques
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# Présentation des listes statiques {#understanding-static-lists}

Les listes statiques sont l’une des fonctionnalités les plus simples et utiles de Marketo. Il s’agit simplement d’une liste de noms de votre base de données. Vous trouverez plein de raisons de les utiliser.

>[!NOTE]
>
>Une seule personne dans la base de données peut se trouver dans de nombreuses listes statiques différentes.

La différence entre une liste statique et une liste dynamique est essentielle pour comprendre.

| Type | Logique |
|---|---|
| Liste intelligente | Basé sur **règles définies** |
| Liste statique | Basé sur **ajout/suppression de chaque personne** |

>[!CAUTION]
>
>Une des erreurs les plus courantes est de penser que vous pouvez retirer une personne d&#39;une liste en la &quot;supprimant&quot; simplement. **C&#39;est faux.**. La suppression de la personne les supprime de **toute la base**, pas seulement la liste.

## Méthodes pour ajouter/supprimer des personnes d’une liste {#ways-to-add-remove-people-from-a-list}

1. Étape de flux de campagne dynamique ([Ajouter à la liste](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}, [Remove from List](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"})

1. [Étape de flux d’action unique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. Faire glisser des personnes dans une liste de l’arborescence
1. [Import de liste](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## Certaines utilisations d’une liste statique {#some-uses-of-a-static-list}

* Liste qui a été présélectionnée pour recevoir un message marketing.
* Une liste de &quot;concurrents&quot; que vous utilisez pour envoyer des messages de contre-intelligence espiègles.
* Liste temporaire des personnes d’un état particulier, qui sont ensuite supprimées par les campagnes dynamiques lorsqu’elles quittent cet état.

Profitez de la puissance de LIST !

>[!MORELIKETHIS]
>
>[Création d’une liste statique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
