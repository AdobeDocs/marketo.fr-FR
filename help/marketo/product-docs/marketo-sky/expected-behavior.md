---
description: Comportement attendu - Documents Marketo - Documentation du produit
title: Comportement attendu
hide: true
hidefromtoc: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
source-git-commit: fb77478cdcd2b455e9f2359e16aca50143ce492c
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Comportement attendu {#expected-behavior}

Dans cet article, vous trouverez des informations sur le comportement attendu associé aux audiences prédictives (PA).

## Considérations sur les données et la confidentialité

* Tous les traitements de données requis pour les modèles AI/ML ont lieu en Amérique du Nord.
* Les modèles AI/ML n’utilisent pas d’informations de piste spécifiques telles que les prénoms ou les noms, le genre, les emails, les numéros de contact, etc. Les modèles n’utilisent que des attributs généraux dérivés des journaux de l’activité et des données démographiques.

**Pour les audiences prédictives, vous pouvez vous attendre au comportement suivant :**

* PA est accessible dans Marketo Sky et dans l’expérience Marketo Classic. La disponibilité de fonctionnalités spécifiques est la suivante :
   * Filtres prédictifs - [!DNL Sky/Classic]
   * Inscriptions prévues - [!DNL Sky/Classic]
   * Prédictions de probabilité au niveau de l’piste - [!DNL Sky/Classic]
   * Objectifs et suivi - [!DNL Sky] only
   * Statistiques et recommandations - [!DNL Sky] only
* Les tâches d’activation initiales **24-48 heures** pour tous les processus à terminer une fois que l’option PA a été activée. Toutes les fonctionnalités d’ Audiences prédictives et de filtres prédictifs s’affichent dans l’interface, mais il peut s’écouler jusqu’à 24 heures avant que ces fonctionnalités ne commencent à fonctionner.
* **Les prédictions ne seront générées que pour les nouvelles campagnes créées une fois la fonctionnalité activée.**

**Il existe d’autres considérations spécifiques aux filtres prédictifs**:

* Les filtres de probabilité d’inscription et de présence ne peuvent être utilisés qu’avec des programmes d’événement ou de webinaire. Les filtres Lookalike et Unsubscribe peuvent être utilisés dans les programmes de messagerie, d’événement et de webinaire.
* Vous pouvez appliquer des filtres prédictifs à une campagne dynamique même si le programme parent est créé avant l’activation des filtres prédictifs.
* Les filtres prédictifs ne sont pas disponibles pour les campagnes de déclenchement.
* Pour exécuter une campagne dynamique, les filtres de probabilité doivent être utilisés conjointement avec d’autres filtres standard.
* La fonction Règles enregistrées n’est pas disponible pour être utilisée dans les campagnes qui contiennent des filtres prédictifs.
* Vous pouvez utiliser **jusqu’à 5** filtres prédictifs dans une liste dynamique.
* Les filtres prédictifs peuvent traiter une **1 million de pistes qualifiées au maximum**.
* Vous pouvez **jusqu’à 50 programmes actifs** avec des filtres prédictifs. Un programme actif est un programme qui utilise des filtres prédictifs et qui a été planifié au moins une fois.

## Quand les inscriptions prévues ne sont-elles pas disponibles ?

Les enregistrements prévus ne seront pas disponibles dans les cas d’utilisation suivants :

* si le programme a été créé avant l’ajout de Predictive Audiences
* lorsque les états du programme ne sont pas mappés aux états du système.
* lorsqu’il n’y a aucun membre dans le programme ;
* lorsqu’il n’existe aucun programme similaire au cours des 6 derniers mois qui répond aux critères requis ;
