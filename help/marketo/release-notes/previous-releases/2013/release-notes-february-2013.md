---
unique-page-id: 2951103
description: Notes De Mise À Jour - Février 2013 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Février 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Notes De Mise À Jour : Février 2013 {#release-notes-february}

La version de février comprend une fonctionnalité très demandée, la prise en charge de [!DNL Apple Safari] et d’autres petites améliorations.

## Soutien officiel à [!DNL Apple Safari] {#official-support-for-apple-safari}

Les dernières versions d’[!DNL Apple Safari] pour Mac et [!DNL Windows] sont entièrement prises en charge pour une utilisation avec la gestion des prospects Marketo. Remarque : [!DNL Safari] sur iOS n’est pas entièrement compatible.

## Améliorations des Webhooks {#webhooks-enhancements}

Webhooks est amélioré pour échapper les jetons dans l’URL/la payload et peut également mettre à jour les champs de prospect Marketo en analysant les réponses XML/JSON de systèmes tiers (non disponibles dans le [!DNL Spark SMB Edition]).

## Point d’entrée de l’API SOAP mis à jour {#updated-soap-api-endpoint}

Le point d’entrée préféré de l’API SOAP a été mis à jour. Il est affiché dans [!UICONTROL Admin] -> API SOAP. Mettez à jour vos appels pour utiliser ce nouveau point d’entrée. Les appels d’API vers l’ancien point d’entrée sont obsolètes, mais continueront à fonctionner. (API SOAP non disponible dans le [!DNL Spark SMB Edition])

## Prise en charge mobile des onglets [!DNL Facebook] {#mobile-support-for-facebook-tabs}

[!DNL Facebook] onglets publiés depuis Marketo détectent les appareils mobiles et les acheminent vers une page de destination. Cela permet de s’assurer que l’utilisateur obtient le contenu approprié sur les appareils mobiles sur lesquels les onglets [!DNL Facebook] ne sont pas pris en charge (disponibles dans [!DNL Spark], [!DNL Standard], [!DNL Select SMB Editions] et [!DNL Marketo Social Marketing]).

## Prochainement : prise en charge de plusieurs modèles {#coming-soon-support-for-multiple-models}

Nous jetons les bases pour soutenir plusieurs modèles de cycle de revenus, avons voté #1 idée pour RCA dans la Communauté, dans une prochaine version. Dans cette version, vous remarquerez quelques modifications, notamment [filtres de liste dynamique et Ajouter des choix dans les étapes de flux](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) pour prendre en charge la sélection d’un modèle et d’une étape. Nous déplaçons également les champs Étape de revenus de leads et Modèle de cycle de revenus de leads hors de l’onglet Grille de leads de liste dynamique.
