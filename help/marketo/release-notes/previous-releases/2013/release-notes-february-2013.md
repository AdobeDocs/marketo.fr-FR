---
unique-page-id: 2951103
description: Notes de mise à jour - Février 2013 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Février 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Notes de mise à jour : février 2013 {#release-notes-february}

La version de février comprend une fonctionnalité très demandée, la prise en charge d’Apple Safari et d’autres petites améliorations.

## Assistance officielle pour Apple Safari {#official-support-for-apple-safari}

Les dernières versions d’Apple Safari pour Mac et Windows sont entièrement prises en charge pour une utilisation avec la gestion des pistes Marketo. Remarque : Safari sur iOS n’est pas entièrement compatible.

## Améliorations apportées aux webhooks {#webhooks-enhancements}

Webhooks est amélioré de manière à ajouter des jetons d’échappement dans l’URL/la payload et peut également mettre à jour les champs de piste Marketo en analysant les réponses XML/JSON provenant de systèmes tiers (non disponibles dans Spark SMB Edition).

## Point de terminaison d’API SOAP mis à jour {#updated-soap-api-endpoint}

Le point de terminaison d’API SOAP préféré a été mis à jour, comme illustré dans l’API Admin -> SOAP. Mettez à jour vos appels pour utiliser ce nouveau point de terminaison. Les appels d’API vers l’ancien point de terminaison sont obsolètes, mais continueront à fonctionner. (API SOAP non disponible dans Spark SMB Edition)

## Prise en charge mobile des onglets Facebook {#mobile-support-for-facebook-tabs}

Les onglets facebook publiés à partir de Marketo détectent les périphériques mobiles et les redirigent vers une page d’entrée. Cela permet de s’assurer que l’utilisateur obtient le contenu approprié sur les appareils mobiles sur lesquels les onglets Facebook ne sont pas pris en charge (disponible dans Spark, Standard, Select SMB Editions et Marketo Social Marketing).

## Bientôt : prise en charge de plusieurs modèles {#coming-soon-support-for-multiple-models}

Nous préparons le terrain pour la prise en charge de plusieurs modèles de cycle des revenus, a voté #1 idée pour RCA dans la Communauté, dans une prochaine version. Dans cette version, vous remarquerez quelques modifications, notamment [Filtres de liste dynamique et Ajouter des choix dans les étapes de flux](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) pour prendre en charge la sélection d’un modèle et d’une étape. Nous déplaçons également les champs Intervalle de piste et Modèle de cycle de recettes de piste hors de l’onglet Grille de piste de liste dynamique.
