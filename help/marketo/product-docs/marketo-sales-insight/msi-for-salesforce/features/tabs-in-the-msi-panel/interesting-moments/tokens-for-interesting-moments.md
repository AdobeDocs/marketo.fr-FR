---
unique-page-id: 1146999
description: Jetons pour les moments intéressants - Documents marketing - Documentation du produit
title: Jetons pour les moments intéressants
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Jetons pour les moments intéressants {#tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>* Découvrez comment utiliser l’[étape de flux Moment intéressant](../../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).
>* En savoir plus sur les [jetons](https://docs.marketo.com/display/docs/tokens).

>



## Jetons disponibles {#available-tokens}

Consultez [Présentation des jetons](../../../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) pour voir tous les jetons que vous pouvez mettre à un moment intéressant.

## Jetons de déclenchement {#trigger-tokens}

En fonction du déclencheur utilisé dans une campagne dynamique, d’autres jetons de déclenchement sont disponibles.

* `{{trigger.Trigger Name}}` qui est toujours le déclencheur lui-même. Par exemple : Cliquez sur Lien dans le courrier électronique.
* `{{trigger.Name}}` est le nom de la ressource qui a déclenché la campagne. Par exemple : Clics sur le lien sur la page Web est l&#39;URL elle-même, sujet des déclencheurs Salesforce, etc.
* D’autres déclencheurs sont disponibles en fonction des contraintes, qui sont répertoriées ci-dessous :

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
  </tr> 
  <tr> 
   <td>Se désabonne du courrier électronique</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
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
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Courriel de vente envoyé</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Ouvre le courriel de vente</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Courriel de vente reçu</td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(coche)"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Courrier électronique de vente abandonné</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(coche)"></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(coche)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
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
   <td><p><br></p></td> 
  </tr> 
  <tr> 
   <td colspan="1">Visites de la page Web*</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(coche)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(coche)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
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

