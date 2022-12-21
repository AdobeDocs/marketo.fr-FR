---
unique-page-id: 1146950
description: Attente - Documents Marketo - Documentation du produit
title: Attendre
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# Attendre {#wait}

## APERÇU {#overview}

Mettez une personne dans un flux de campagne dynamique à l’aide de la méthode pratique **étape d’attente**.

![](assets/wait-overview.png)

Remarquez comment vous pouvez taper en langage naturel comme &quot;4 heures&quot;. Do **not**, toutefois, abréger les mots (c’est-à-dire, 4 heures). La campagne dynamique s’exécute toujours, mais l’étape d’attente est ignorée.

>[!CAUTION]
>
>La modification de la durée d’une étape d’attente n’affecte pas les personnes qui y ont déjà participé. Par exemple : vous avez une étape d’attente de 5 jours, une personne y accède, puis vous définissez l’étape d’attente sur 7 jours. cette personne n’attendra que les 5 jours d’origine avant de passer à l’étape suivante.

>[!TIP]
>
>Si vous avez déjà un utilisateur dans une étape d’attente et que vous ne souhaitez pas qu’il avance une fois la période d’attente terminée, insérez [supprimer du flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) juste après l’étape d’attente. Indiquez qui vous souhaitez supprimer en utilisant la variable [ajouter un choix](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) .

## Utilisation {#usage}

Il existe trois méthodes principales pour utiliser une étape de flux d’attente :

1. [Utilisation d’une durée dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Utilisation d’une date spécifique dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Utilisation d’un jeton de date dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
