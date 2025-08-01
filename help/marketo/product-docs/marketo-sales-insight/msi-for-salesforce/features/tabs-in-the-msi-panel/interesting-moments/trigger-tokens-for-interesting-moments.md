---
unique-page-id: 1146999
description: Jetons de déclenchement pour les moments significatifs - Documents Marketo - Documentation du produit
title: Jetons de déclenchement pour les moments significatifs
exl-id: 666a6eed-c432-4088-b4f1-54c996eca64c
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 67%

---

# Jetons de déclenchement pour les moments significatifs {#trigger-tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Découvrez comment utiliser l’étape de flux [ Moment intéressant ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Jetons disponibles {#available-tokens}

Consultez [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) pour afficher tous les jetons que vous pouvez placer dans un moment intéressant.

## Jetons de déclenchement {#trigger-tokens}

En fonction du déclencheur utilisé dans une campagne intelligente, des jetons de déclencheur supplémentaires sont disponibles.

* `{{trigger.Trigger Name}}` qui est toujours le déclencheur lui-même. Par exemple : clics sur le lien dans l’e-mail.
* `{{trigger.Name}}` est le nom de la ressource qui a déclenché la campagne. Par exemple : Clics sur le lien d’une page web est l’URL elle-même, l’objet des déclencheurs Salesforce, etc.
* D’autres déclencheurs sont disponibles en fonction des contraintes, qui sont répertoriées ci-dessous.

### Déclencheurs d’e-mail {#email-triggers}

<table style="table-layout:auto">
 <colgroup>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th><br></th>
   <th><code>{{trigger.Trigger Name}}</code></th>
   <th><code>{{trigger.Name}}</code></th>
   <th><code>{{trigger.Link}}</code></th>
   <th><code>{{trigger.Subject}}</code></th>
   <th><code>{{trigger.Category}}</code></th>
   <th><code>{{trigger.Details}}</code></th>
   <th><code>{{trigger.Web Page}}</code></th>
   <th><code>{{trigger.Client IP Address}}</code></th>
   <th><code>{{trigger.Sent By}}</code></th>
   <th><code>{{trigger.Received By}}</code></th>
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr>
  <tr>
   <td>Clique sur le lien dans l’e-mail</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Rebonds d’e-mails hard</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>L'e-mail est renvoyé provisoirement</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>L’E-Mail Est Diffusé</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Ouvre l'e-mail</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
    <tr>
   <td>E-mail de transfert à un ami reçu</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
    <tr>
   <td>E-mail de transfert à un ami envoyé</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
  </tr>
  <tr>
   <td>Désabonné de l'e-mail</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
 </tbody>
</table>

### Déclencheurs Salesforce {#salesforce-triggers}

<table style="table-layout:auto">
 <colgroup>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th><br></th>
   <th><code>{{trigger.Trigger Name}}</code></th>
   <th><code>{{trigger.Name}}</code></th>
   <th><code>{{trigger.Link}}</code></th>
   <th><code>{{trigger.Subject}}</code></th>
   <th><code>{{trigger.Category}}</code></th>
   <th><code>{{trigger.Details}}</code></th>
   <th><code>{{trigger.Web Page}}</code></th>
   <th><code>{{trigger.Client IP Address}}</code></th>
   <th><code>{{trigger.Sent By}}</code></th>
   <th><code>{{trigger.Received By}}</code></th>
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr>
  <tr>
   <td>Clics sur le lien dans l'e-mail de vente</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Est un e-mail de vente envoyé</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Ouvre l'e-mail de vente</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Renvoi de l'e-mail de vente</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>L'e-mail de vente est réceptionné</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
    <tr>
   <td>Mise à jour de l'opportunité</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
    <tr>
   <td>Modifications du détenteur</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>L'individu est converti</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Suppression de l’individu de SFDC</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Synchronisation de l’individu avec SFDC</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Supprimé de l'opportunité</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Supprimé de la campagne SFDC</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Activité consignée</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Activité mise à jour</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Ajouté à l'opportunité</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Ajouté à la campagne SFDC</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Modification du statut dans la campagne SFDC</td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
 </tbody>
</table>

### Déclencheurs de connexion aux ventes {#sales-connect-triggers}

<table style="table-layout:auto">
 <colgroup>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th><br></th>
   <th><code>{{trigger.Trigger Name}}</code></th>
   <th><code>{{trigger.Name}}</code></th>
   <th><code>{{trigger.Link}}</code></th>
   <th><code>{{trigger.Subject}}</code></th>
   <th><code>{{trigger.Category}}</code></th>
   <th><code>{{trigger.Details}}</code></th>
   <th><code>{{trigger.Web Page}}</code></th>
   <th><code>{{trigger.Client IP Address}}</code></th>
   <th><code>{{trigger.Sent By}}</code></th>
   <th><code>{{trigger.Received By}}</code></th>
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr>
  <tr>
   <td>Clics sur le lien dans l'e-mail de vente</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Est un e-mail de vente envoyé</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Ouvre l'e-mail de vente</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Renvoi de l'e-mail de vente</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>L'e-mail de vente est réceptionné</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Est ajouté à la campagne de ventes</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Modifications du détenteur</td>
   <td>Est supprimé de la campagne de ventes</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Appel de vente reçu</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
 </tbody>
</table>

### Jetons de déclenchement de Dynamic Chat {#dynamic-chat-trigger-tokens}

<table>
<thead>
  <tr>
    <th> </th>
    <th><code>{{trigger.Agent Email}}</code></th>
    <th><code>{{trigger.Agent Name}}</code></th>
    <th><code>{{trigger.Conversation Status}}</code></th>
    <th><code>{{trigger.Conversation Summary}}</code></th>
    <th><code>{{trigger.Conversation Transcript}}</code></th>
    <th><code>{{trigger.Document Downloaded}}</code></th>
    <th><code>{{trigger.Document Name}}</code></th>
    <th><code>{{trigger.Document Opened}}</code></th>
    <th><code>{{trigger.Document URL}}</code></th>
    <th><code>{{trigger.Goal name}}</code></th>
    <th><code>{{trigger.meeting status}}</code></th>
    <th><code>{{trigger.Name}}</code></th>
    <th><code>{{trigger.Page URL}}</code></th>
    <th><code>{{trigger.routing queue name}}</code></th>
    <th><code>{{trigger.Scheduled For}}</code></th>
    <th><code>{{trigger.source name}}</code></th>
    <th><code>{{trigger.source type}}</code></th>
    <th><code>{{trigger.Trigger Name}}</code></th>
    <th><code>{{trigger.ui type}}</code></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>A pris contact via une boîte de dialogue</td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>A pris contact via un formulaire de conversation</td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
  </tr>
  <tr>
    <td>A pris contact avec un agent dans la boîte de dialogue</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>A pris contact avec un agent dans le formulaire de conversation</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>A planifié une réunion dans la boîte de dialogue</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Réunion planifiée dans le formulaire de conversation</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>A atteint l’objectif du dialogue</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Objectif du formulaire de conversation atteint</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>A interagi avec un document dans la boîte de dialogue</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>A interagi avec le document dans le formulaire de conversation</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
</tbody>
</table>

### Divers {#miscellaneous}

<table style="table-layout:auto">
 <colgroup>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th><br></th>
   <th><code>{{trigger.Trigger Name}}</code></th>
   <th><code>{{trigger.Name}}</code></th>
   <th><code>{{trigger.Link}}</code></th>
   <th><code>{{trigger.Subject}}</code></th>
   <th><code>{{trigger.Category}}</code></th>
   <th><code>{{trigger.Details}}</code></th>
   <th><code>{{trigger.Web Page}}</code></th>
   <th><code>{{trigger.Client IP Address}}</code></th>
   <th><code>{{trigger.Sent By}}</code></th>
   <th><code>{{trigger.Received By}}</code></th>
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr>
  <tr>
   <td>Remplit le formulaire.</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Visites sur la page web</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Clics sur le lien de la page Web</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>S’il ne comporte pas de ![ de vérification (coche)](assets/check.png) il renvoie une chaîne vide (rien) au moment intéressant.

&#42;La page web Déclencheur **Visites** comporte quelques jetons supplémentaires :

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Testez toujours vos moments intéressants pour vous assurer qu’ils s’affichent comme vous le souhaitez.
>
>Assurez-vous également qu’il intéresse le commercial et pas seulement vous !
