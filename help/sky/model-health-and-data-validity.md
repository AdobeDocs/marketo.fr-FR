---
title: modèle-santé-et-données-validité
description: Santé du modèle et Validité des données
exl-id: b14ec648-be1c-467b-b41d-2c53d74e25ea
source-git-commit: 41a51afde7942d6973a01636810bc5862d023e99
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Santé du modèle et Validité des données

Les performances de vos modèles dépendent de la qualité et de l’exhaustivité des données d’entrée. Consultez le facteur d’influence supérieur pour chacun de vos modèles AI de probabilité. Consultez également les principaux facteurs qui entraînent une inscription plus ou moins élevée, une participation à un événement ou des désabonnements.

>[!NOTE]
>
>Les comportements marqués par le signe (+) influencent positivement les prédictions (et inversement).

Voici comment évaluer la santé de votre modèle.

Accédez à la section **[!UICONTROL Modèles et santé des données]** section **[!UICONTROL Public prédictif]** dans la **[!UICONTROL Administrateur]** zone de Marketo Classic. Vous y verrez tous vos modèles et leurs statuts.

![Image Un](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **Statut de formation**: Indique si votre modèle s’entraîne activement (amélioration des prévisions). La formation se déroule automatiquement toutes les 2 semaines. Tout modèle qui _Traitement_ peut prendre jusqu&#39;à 24 heures pour finir. Pour _Échec_ modèles, veuillez contacter [Prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).
* **État d’évaluation**: Indique si votre modèle calcule activement les prédictions (pourcentages de probabilité) pour les membres du programme.
* **Performances**: catégorisation de la santé de votre modèle en fonction de l&#39;intégralité des données et de la qualité des données (voir ci-dessous).
* **Complétude des données**: Pourcentage d&#39;attributs de données présents/complets.
* **Qualité des données**: Pourcentage d&#39;attributs qui contiennent des données fiables et utilisables.
