---
title: comportement attendu
description: Comportement attendu
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---


# Comportement attendu

<br> 

Dans cet article, vous trouverez des informations sur le comportement attendu associé aux Audiences prédictives (AP).

## Considérations relatives aux données et à la confidentialité

* Tous les traitements de données requis pour les modèles AI/ML se déroulent en Amérique du Nord.
* Les modèles AI/ML n&#39;utilisent pas d&#39;informations de piste spécifiques telles que les prénoms ou les noms de famille, le sexe, les courriels, les numéros de contact, etc. Les modèles utilisent uniquement les attributs généraux dérivés des données fimographiques et des journaux d&#39;activité.

## Pour les Audiences prédictives, vous pouvez vous attendre au comportement suivant :

* PA est accessible en Marketo Sky et en Marketo Classic. La disponibilité de fonctionnalités spécifiques est la suivante :
   * Filtres prédictifs - [!DNL Sky/Classic]
   * Inscriptions prévues - [!DNL Sky/Classic]
   * Prédictions de probabilités au niveau des pistes - [!DNL Sky/Classic]
   * Objectifs et suivi - [!DNL Sky] uniquement
   * Informations et recommandations - [!DNL Sky] seulement
* [L’activation](/help/sky/getting-started-with-predictive-audiences.md) initiale prend **24 à 48 heures** pour que tous les processus se terminent une fois l’AP activée. Toutes les fonctions d’Audiences prédictives et de Filtres prédictifs sont visibles dans l’interface, mais ces fonctions peuvent prendre jusqu’à 24 heures pour commencer à fonctionner.
* **Les prédictions ne seront générées que pour les nouvelles campagnes créées après l&#39;activation de la fonction.**

## Il y a d&#39;autres considérations spécifiques aux filtres prédictifs :

* Inscription et participation Les filtres de probabilité ne peuvent être utilisés qu&#39;avec des programmes événements ou webinaires. Les filtres Looksos et Unsubscription peuvent être utilisés dans les programmes de messagerie électronique, de événement et de webinar.
* Vous pouvez appliquer des filtres prédictifs à une campagne dynamique même si le programme parent est créé avant l’activation des filtres prédictifs.
* Les filtres prédictifs ne sont pas disponibles pour les campagnes de déclenchement.
* Pour exécuter une campagne intelligente, les filtres de probabilité doivent être utilisés conjointement avec d’autres filtres réguliers.
* La fonction Règles enregistrées n’est pas disponible pour les campagnes qui contiennent des filtres prédictifs.
* Vous pouvez utiliser **jusqu’à 5** filtres prédictifs dans une liste intelligente.
* Les filtres prédictifs peuvent traiter un **maximum de 1 million de pistes** qualifiées.
* Vous pouvez avoir **jusqu&#39;à 50 programmes** principaux avec des filtres prédictifs. Un programme principal est un programme qui utilise des filtres prédictifs et qui a été planifié au moins une fois.

## Quand les inscriptions prévues ne sont-elles pas disponibles ?

Les inscriptions prévues ne seront pas disponibles dans les cas d&#39;utilisation suivants :

* si le programme a été créé avant l’ajout d’Audiences prédictives
* lorsque les états de programme ne sont pas associés aux états système
* lorsqu&#39;il n&#39;y a pas de membres au programme
* lorsqu&#39;il n&#39;y a pas de programmes similaires antérieurs au cours des 6 derniers mois qui répondent aux critères requis
