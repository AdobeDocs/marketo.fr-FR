---
description: Activités [!DNL Dynamic Chat] - Documents Marketo - Documentation Du Produit
title: Activités [!DNL Dynamic Chat]
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 4%

---

# Activités [!DNL Dynamic Chat] {#dynamic-chat-activities}

[!DNL Dynamic Chat] propose plusieurs filtres et déclencheurs à utiliser dans vos listes dynamiques.

![](assets/dynamic-chat-activities-1.png)

## Définitions {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>Déclenché</b></td>
    <td>Un événement déclencheur se produit lorsqu’un visiteur répond aux critères de ciblage d’une boîte de dialogue ou d’un flux de conversation et s’affiche dans la boîte de dialogue.
    <br>Un événement déclencheur par visiteur et par session.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Engagé dans un flux de conversation/dialogue</b></td>
    <td>Un engagement se produit la première fois qu’un visiteur web clique sur une invite dans une boîte de dialogue ou un flux de conversation (il clique sur une option à choix multiples, envoie des informations, réserve une réunion, ouvre un document, etc.). Si un visiteur ouvre une boîte de dialogue ou un flux de conversation, mais ne clique pas sur une invite, un engagement est <b>non</b> consigné.
    <br>Un événement d’engagement par visiteur et par session.</td>
  </tr>
   <tr>
    <td style="width:25%"><b>Actuellement occupé avec un agent</b></td>
    <td>Se produit lorsqu’un visiteur est correctement connecté à un agent de chat en direct.
    <br>Un engagé avec l’événement d’agent par visiteur, par session.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>A interagi avec le document</b></td>
    <td>Se produit lorsqu’un visiteur clique sur un document dans une carte de document.
    <br>Il peut y avoir plusieurs interactions de documents par visiteur et par session.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Objectifs atteints</b></td>
    <td>Se produit lorsqu’un visiteur atteint un objectif. <br>Il peut y avoir plusieurs événements d’objectif atteint par visiteur et par session.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Réunion planifiée</b></td>
    <td>Se produit lorsqu’un visiteur réserve une réunion avec un agent Dynamic Chat.
    <br>Il peut y avoir plusieurs événements réservés à une réunion par visiteur et par session.</td>
  </tr>
</tbody>
</table>

## Éléments à noter {#things-to-note}

* Les conditions sont prises en charge dans les étapes de flux [!DNL Dynamic Chat]
* [!DNL Dynamic Chat] activités peuvent être synchronisées avec [[!DNL Marketo Sales Insight]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* Vous pouvez afficher les activités de [!DNL Dynamic Chat] individuelles dans le journal des activités d’un enregistrement de personne
