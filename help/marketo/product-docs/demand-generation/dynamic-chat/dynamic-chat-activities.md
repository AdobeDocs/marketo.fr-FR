---
description: Activités du Dynamic Chat - Documents Marketo - Documentation du produit
title: Activités Dynamic Chat
feature: Dynamic Chat
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: b1101617ec670d42aed8c35044b656ba5fa0f9f5
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Activités Dynamic Chat {#dynamic-chat-activities}

Dynamic Chat propose plusieurs filtres et déclencheurs à utiliser dans vos listes dynamiques.

![](assets/dynamic-chat-activities-1.png)

## Définitions {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td><b>Déclenché</b></td>
    <td>Un événement déclencheur se produit lorsqu’un visiteur répond aux critères de ciblage d’un dialogue ou d’un flux de conversation et s’affiche dans la boîte de dialogue.
    <br>Un événement de déclenchement par visiteur, par session.</td>
  </tr>
  <tr>
    <td><b>Engagé avec un flux/dialogue de conversation</b></td>
    <td>Un engagement se produit la première fois qu’un visiteur web clique sur une invite dans un flux de dialogue ou de conversation (en cliquant sur une option à choix multiples, en envoyant des informations, en réservant une réunion, en ouvrant un document, etc.). Si un visiteur ouvre un flux de dialogue ou de conversation, mais ne clique pas sur une invite, un engagement est <b>not</b> consigné. 
    <br>Un événement d’engagement par visiteur, par session.</td>
  </tr>
   <tr>
    <td><b>Engagé avec un agent</b></td>
    <td>survient lorsqu’un visiteur est connecté à un agent de conversation en direct.
    <br>L’un d’eux a interagi avec l’événement de l’agent par visiteur, par session.</td>
  </tr>
  <tr>
    <td><b>Interaction avec le document</b></td>
    <td>survient lorsqu’un visiteur clique sur un document d’une carte de document.
    <br>Il peut y avoir plusieurs interactions de documents par visiteur, par session.</td>
  </tr>
  <tr>
    <td><b>Objectifs atteints(s)</b></td>
    <td>Se produit lorsqu’un visiteur atteint un objectif. <br>Il peut y avoir plusieurs événements atteints par le but par visiteur, par session.</td>
  </tr>
  <tr>
    <td><b>Réunion planifiée</b></td>
    <td>survient lorsqu’un visiteur fait la réservation d’une réunion avec un agent Dynamic Chat.
    <br>Il peut y avoir plusieurs événements réservés à une réunion par visiteur, par session.</td>
  </tr>
</tbody>
</table>

## Informations à noter {#things-to-note}

* Les conditions sont prises en charge dans les étapes de flux du Dynamic Chat.
* Les activités de Dynamic Chat peuvent être synchronisées avec [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* Vous pouvez afficher des activités de Dynamic Chat individuelles dans le Journal d’activité d’un enregistrement de personne.
