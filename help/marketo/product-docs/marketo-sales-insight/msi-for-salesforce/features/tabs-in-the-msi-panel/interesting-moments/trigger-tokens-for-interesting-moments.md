---
unique-page-id: 1146999
description: Jetons de déclenchement pour les moments intéressants - Marketo Docs - Documentation du produit
title: Déclencher des jetons pour des moments intéressants
exl-id: 666a6eed-c432-4088-b4f1-54c996eca64c
translation-type: tm+mt
source-git-commit: 20a3bee9973340d7b772532d1be31fe745e5ffd7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 29%

---

# Déclencher des jetons pour des moments intéressants {#trigger-tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Découvrez comment utiliser l’[étape de flux Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Jetons disponibles {#available-tokens}

Consultez [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) pour voir tous les jetons que vous pouvez mettre à un moment intéressant.

## Jetons de déclenchement {#trigger-tokens}

En fonction du déclencheur utilisé dans une campagne dynamique, d’autres jetons de déclenchement sont disponibles.

* `{{trigger.Trigger Name}}` qui est toujours le déclencheur lui-même. Par exemple : Cliquez sur Lien dans le courrier électronique.
* `{{trigger.Name}}` est le nom de la ressource qui a déclenché la campagne. Par exemple : Clics sur le lien sur la page Web est l&#39;URL elle-même, sujet des déclencheurs Salesforce, etc.
* D’autres déclencheurs sont disponibles en fonction des contraintes, qui sont répertoriées ci-dessous.

**Triggers de messagerie**

<table> 
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
   <td>Clique sur lien dans e-mail</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td>Courrier électronique - Bond dur</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td>E-mail remis</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td>
  </tr> 
  <tr> 
   <td>Désabonné de l'e-mail</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Déclencheurs Salesforce**

<table> 
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
   <td>Clique sur lien dans e-mail de vente</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Est un e-mail de vente envoyé</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Ouvre l'e-mail de vente</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Renvoi de l'e-mail de vente</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td>Réception de l'e-mail de vente</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Mise à jour de l'opportunité</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td>Modifications détenteur</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td>Supprimer de la campagne SFDC</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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

**Déclencheurs de la connexion commerciale**

<table> 
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
   <td>Clique sur lien dans e-mail de vente</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Est un e-mail de vente envoyé</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Ouvre l'e-mail de vente</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Renvoi de l'e-mail de vente</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td>Réception de l'e-mail de vente</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Est ajouté à la campagne de ventes</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td>Modifications détenteur</td> 
   <td>Est supprimé de la campagne de ventes</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
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

**Divers**

<table> 
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
   <td>Remplit le formulaire</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Visite la page Internet</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Clique le lien sur page Web</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>S&#39;il n&#39;a pas de vérification ![(tick)](assets/check.svg) alors il retournerait une chaîne vide (rien) dans le moment intéressant.

*Le déclencheur **Visites Page Web** comporte quelques jetons supplémentaires :

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Testez toujours vos moments intéressants pour vous assurer qu&#39;ils rendent la façon dont vous voulez.
>
>Assurez-vous également que c&#39;est intéressant pour le vendeur, pas seulement pour vous. ![(évier)](assets/wink.svg)>
