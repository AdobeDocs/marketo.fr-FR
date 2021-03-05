---
unique-page-id: 1146999
description: Jetons pour les moments intéressants - Documents marketing - Documentation du produit
title: Jetons pour les moments intéressants
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Jetons pour les moments intéressants {#tokens-for-interesting-moments}

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
   <td>Clics sur le lien dans le courrier électronique</td> 
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
   <td>Retours douces du courrier électronique</td> 
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
   <td>Ouvre le courrier électronique</td> 
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
   <td>Envoi au courrier électronique de l'ami reçu</td> 
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
   <td>Envoyer un courriel à un ami</td> 
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
   <td>Se désabonne du courrier électronique</td> 
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
   <td>Lien de clics dans le courriel commercial</td> 
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
   <td>Adresse électronique de vente envoyée</td> 
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
   <td>Ouvre le courriel de vente</td> 
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
   <td>Retours de courriel de vente</td> 
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
   <td>Courriel de vente reçu</td> 
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
   <td>L'opportunité est mise à jour</td> 
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
   <td>Modifications du propriétaire</td> 
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
   <td>Personne convertie</td> 
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
   <td>Personne supprimée de SFDC</td> 
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
   <td>La personne est synchronisée avec SFDC</td> 
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
   <td>Retrait de SFDC Campaign</td> 
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
   <td>Ajouté à SFDC Campaign</td> 
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
   <td>Etat modifié dans SFDC Campaign</td> 
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
   <td>Lien de clics dans le courriel commercial</td> 
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
   <td>Adresse électronique de vente envoyée</td> 
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
   <td>Ouvre le courriel de vente</td> 
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
   <td>Retours de courriel de vente</td> 
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
   <td>Courriel de vente reçu</td> 
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
   <td>Est Ajouté au Campaign de vente</td> 
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
   <td>Modifications du propriétaire</td> 
   <td>Est Supprimé De La Campaign De Ventes</td> 
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
   <td>Remplir le formulaire</td> 
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
   <td>Page Web Visites</td> 
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
   <td>Clics sur le lien sur la page Web</td> 
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
