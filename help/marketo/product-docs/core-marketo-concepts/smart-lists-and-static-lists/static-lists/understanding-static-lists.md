---
unique-page-id: 2949891
description: Présentation des listes statiques - Documents Marketo - Documentation du produit
title: Présentation des listes statiques
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 5%

---

# Présentation des listes statiques {#understanding-static-lists}

Les listes statiques sont l’une des fonctionnalités les plus simples et utiles de Marketo. Il s’agit simplement d’une liste de noms provenant de votre base de données. Tu trouveras de nombreuses raisons de les utiliser.

>[!NOTE]
>
>Une seule personne dans la base de données peut figurer dans de nombreuses listes statiques différentes.

Il est essentiel de comprendre la différence entre une liste statique et une liste dynamique.

| Type | Logique |
|---|---|
| Liste intelligente | Selon des **règles définies** |
| Liste statique | En fonction de **ajout/suppression de chaque personne** |

>[!CAUTION]
>
>L’une des erreurs les plus courantes consiste à penser que vous pouvez supprimer une personne d’une liste en la « supprimant » simplement. **C&#39;est faux**. La suppression de la personne la supprimera de **l’ensemble de la base de données** et pas seulement de la liste.

## Méthodes d’ajout ou de suppression de personnes d’une liste {#ways-to-add-remove-people-from-a-list}

1. Étape de flux de campagne intelligente ([Ajouter à la liste](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}, [Supprimer de la liste](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"})

1. [Étape de flux à action unique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. Faire glisser des personnes dans une liste de l&#39;arborescence
1. [Import de liste](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## Utilisation d’une liste statique {#some-uses-of-a-static-list}

* Une liste qui a été présélectionnée pour recevoir un message marketing.
* Une liste de « concurrents » que vous utilisez pour envoyer des messages de contre-espionnage malveillants.
* Liste temporaire de personnes dans un état particulier, qui sont ensuite supprimées par les campagnes intelligentes lorsqu’elles quittent cet état.

Profitez de la puissance de la LISTE !

>[!MORELIKETHIS]
>
>[Créer une liste statique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
