---
description: Présentation de la synchronisation CRM Veeva - Documents Marketo - Documentation du produit
title: Présentation de la synchronisation CRM Veeva
hide: true
hidefromtoc: true
source-git-commit: 93e6bb881e10cda26b3a33569dc67627d628a178
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%

---

# Présentation de la synchronisation CRM Veeva {#understanding-the-veeva-crm-sync}

En quelques étapes simples, il est facile d&#39;exécuter une synchronisation entre Adobe Marketo Engage et la CRM Veeva.

## Fonctionnement de la synchronisation {#how-the-sync-works}

Les Marketo Engage se synchronisent avec Veeva CRM toute la journée, tous les jours. Chaque synchronisation prend un certain temps, s’interrompt pendant 5 minutes, puis recommence.

>[!NOTE]
>
>La toute première synchronisation peut prendre des heures, voire des jours, car Marketo Engage copie la totalité de la base de données depuis Veeva. Ensuite, chaque synchronisation prend généralement des minutes (parfois des secondes) et synchronise uniquement les données qui ont changé.

![](assets/understanding-the-veeva-sync-1.png)

La synchronisation entre Veeva et Marketo Engage est bidirectionnelle uniquement pour les champs Contact de l’objet de compte Personne. Dans ce cas, chaque fois que vous apportez des modifications à Veeva ou à Marketo Engage, vos mises à jour seront répercutées dans les deux systèmes. Toutes les autres synchronisations sont de Veeva à Marketo Engage uniquement. Cliquez sur les liens ci-dessous pour plus de détails sur chacun d’eux.

## Ce qui est synchronisé entre Marketo Engage et Veeva {#what-is-synced-between-marketo-engage-and-veeva}

* Comptes de personne
* Utilisateurs
* Appeler et appeler des objets clés
* Objets personnalisés

## Informations à connaître {#things-to-know}

* Les informations d’identification que vous saisissez en Marketo Engage pour Veeva sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

* Veeva CRM est basé sur force.com et le riche Marketo Engage d&#39;expérience avec la plateforme est hérité dans cette synchronisation.

* La Veeva CRM : prospect, contact, compte (comptes d’entreprise, opportunité, campagne et activité). Toutefois, ils ne sont pas pris en charge dans la synchronisation avec Marketo Engage.
