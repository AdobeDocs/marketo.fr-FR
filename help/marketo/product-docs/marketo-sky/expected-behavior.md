---
description: Comportement Attendu - Documents Marketo - Documentation Du Produit
title: Comportement attendu
hide: true
hidefromtoc: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# Comportement attendu {#expected-behavior}

Dans cet article, vous trouverez des informations sur le comportement attendu associé aux [!UICONTROL audiences prédictives] (AP).

## Considérations relatives aux données et à la confidentialité

* Tous les traitements de données requis pour les modèles d’IA/ML ont lieu en Amérique du Nord.
* Les modèles d’IA/ML n’utilisent pas d’informations de prospect spécifiques telles que le prénom ou le nom, le genre, les e-mails, les numéros de contact, etc. Les modèles n’utilisent que des attributs généraux dérivés des graphiques de firme et des journaux d’activité.

**Pour les [!UICONTROL audiences prédictives], le comportement attendu est le suivant**

* PA est accessible dans [!DNL Marketo Sky] et dans l’expérience [!DNL Marketo Classic]. La disponibilité de fonctionnalités spécifiques est la suivante :
   * Filtres prédictifs - [!DNL Sky/Classic]
   * Inscriptions prévues - [!DNL Sky/Classic]
   * Prédictions de vraisemblance au niveau du lead - [!DNL Sky/Classic]
   * Objectifs et suivi - [!DNL Sky] uniquement
   * Informations et recommandations - [!DNL Sky] uniquement
* L’activation initiale prend **24 à 48 heures** pour que tous les processus se terminent une fois que PA a été activé. Toutes les fonctionnalités des Audiences prédictives et des Filtres prédictifs s’affichent dans l’interface, mais le fonctionnement de ces fonctionnalités peut prendre jusqu’à 24 heures.
* **Les prévisions ne seront générées que pour les nouvelles campagnes créées une fois la fonctionnalité activée.**

**Il existe d’autres considérations spécifiques aux filtres prédictifs** :

* Les filtres de probabilité d’inscription et de présence ne peuvent être utilisés qu’avec des programmes d’événement ou de webinaire. Les filtres de similaire et de désabonnement peuvent être utilisés dans les programmes d’e-mail, d’événement et de webinaire.
* Vous pouvez appliquer des filtres prédictifs à une campagne dynamique même si le programme parent est créé avant l’activation des filtres prédictifs.
* Les filtres prédictifs ne sont pas disponibles pour les campagnes de déclenchement.
* Pour exécuter une campagne intelligente, les filtres de vraisemblance doivent être utilisés conjointement avec d’autres filtres standard.
* La fonction Règles enregistrées n’est pas disponible pour les campagnes qui contiennent des filtres prédictifs.
* Vous pouvez utiliser **jusqu’à 5** filtres prédictifs dans une liste dynamique.
* Les filtres prédictifs peuvent traiter un **maximum d’1 million de prospects qualifiés**.
* Vous pouvez avoir **jusqu’à 50 programmes actifs** avec des filtres prédictifs. Un programme actif est tout programme qui utilise des filtres prédictifs et qui a été planifié au moins une fois.

## Quand les enregistrements prévus ne sont-ils pas disponibles ?

Les enregistrements prévus ne seront pas disponibles dans les cas d’utilisation suivants :

* si le programme a été créé avant l’ajout des audiences prédictives
* lorsque les états du programme ne sont pas mappés aux états du système
* lorsqu’il n’y a aucun membre dans le programme
* lorsqu’il n’existe pas de programmes similaires au cours des 6 derniers mois qui répondent aux critères requis
