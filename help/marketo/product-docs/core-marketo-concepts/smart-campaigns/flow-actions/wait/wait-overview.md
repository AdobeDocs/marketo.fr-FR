---
unique-page-id: 1146950
description: Attente - Documents Marketo - Documentation du produit
title: Attendre
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 15%

---

# Vue d’ensemble de l’étape Attendre {#wait-overview}

Mettez en pause une personne dans un flux de campagne intelligente avec l’étape **wait** pratique.

![](assets/wait-overview-1.png)

Remarquez comment vous pouvez saisir du texte en langage naturel comme « 4 heures ». Toutefois **n** abrégez pas les mots (c.-à-d. 4 heures). La campagne intelligente s’exécuterait toujours, mais l’étape d’attente serait ignorée.

>[!CAUTION]
>
>La modification de la durée d’une étape d’attente n’affectera pas les personnes qui y ont déjà accédé. Par exemple : vous avez une étape d’attente de 5 jours, une personne la saisit, puis vous modifiez l’étape d’attente en 7 jours - cette personne n’attendra toujours que les 5 jours initiaux avant de passer à l’étape de flux suivante.

>[!TIP]
>
>Si une personne se trouve déjà dans une étape d’attente et que vous ne souhaitez pas qu’elle avance après la fin de la période d’attente, insérez [supprimer du flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) juste après l’étape d’attente. Indiquez qui vous souhaitez supprimer à l’aide de l’option [ajouter un choix](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md).

Il existe trois façons principales d’utiliser une étape de flux d’attente :

1. [Utiliser une durée dans une étape de flux Attendre](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Utiliser une date spécifique dans une étape de flux Attendre](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Utiliser un jeton de date dans une étape de flux Attendre](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
