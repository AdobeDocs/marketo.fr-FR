---
unique-page-id: 1147114
description: Présentation de mes jetons dans un programme - Documents Marketo - Documentation du produit
title: Présentation de mes jetons dans un programme
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
source-git-commit: b21f955bf98063e11f8ed3fdc6f164134ee4f5aa
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 3%

---

# Présentation de mes jetons dans un programme {#understanding-my-tokens-in-a-program}

Un jeton est une variable que vous pouvez utiliser dans les emails, les landing pages et les campagnes intelligentes pour faciliter votre vie.

Outre Mes jetons, vous pouvez également utiliser n’importe quel jeton intégré dans vos programmes. Consultez la section [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}.

## Mes jetons  {#my-tokens}

Mes jetons sont des variables personnalisées que n’importe qui peut créer. Ils sont [created](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} dans des dossiers de campagne ou des programmes.

Mes jetons s’affichent comme suit : `{{my.Name Of Token}}`

Exemples:

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>Type de jeton</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Fichier du calendrier <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilisez ce jeton pour <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">ajouter un fichier d’événement de calendrier (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> à vos emails et landing pages.</td> 
  </tr> 
  <tr> 
   <td><p>Date <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Ce jeton contient une valeur de date. La date s’affiche sous la forme d’un jour d’un mois (par exemple, 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>Script de l'e-mail <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilisez ce jeton pour exécuter un script Velocity dans vos emails. En savoir plus <a href="https://developers.marketo.com/documentation/email-scripting/" title="Lien de suivi" rel="nofollow">here</a>. </td> 
  </tr> 
  <tr> 
   <td>Numéro<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Tout entier. Il peut même être négatif.</td> 
  </tr> 
  <tr> 
   <td>Texte complet <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>C'est HTML. Utilisez-le dans les emails et les landing pages.</td> 
  </tr> 
  <tr> 
   <td>Évaluation <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilisez ce jeton dans la variable <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">étape du flux de score de changement</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">Campagne SFDC <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">Utilisez ce jeton pour permettre aux pistes qui font partie d’un programme Marketo d’être ajoutées à n’importe quelle campagne SFDC ajoutée.</td> 
  </tr> 
  <tr> 
   <td>Texte <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Juste du texte. Utilisez-le lorsque le HTML est sur-tué. La taille maximale des jetons de texte est de 524 288 caractères (UTF-8) ou 2 Mo.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Mes jetons ne seront pas résolus lors de l’envoi d’un email à partir de Sales Insight sur Microsoft Dynamics ou Salesforce ; seuls les jetons standard seront renseignés (prospect, société, etc.). Valeurs par défaut des jetons _will_ par contre.

## Imbrication de jetons {#nesting-tokens}

Lorsque vous créez un jeton, il peut être référencé par d’autres objets de l’arborescence. Il existe une structure d’affectation des noms pour l’emplacement où le jeton a été créé pour une gestion facile.

* **Jeton local :** Le jeton a été créé directement dans ce programme ou dossier.
* **Jeton hérité :** Le jeton a été créé dans l’arborescence dans un dossier ou un programme de niveau supérieur.
* **Jeton remplacé :** Le jeton a été hérité, puis une personne a fait une exception dans ce programme ou dossier.

Vous pouvez créer des variables globales, puis les remplacer aux niveaux inférieurs de l’arborescence.

Le déplacement de programmes et de dossiers affecte également les jetons. Vérifiez toujours que les références ne sont pas rompues lors du déplacement.

>[!NOTE]
>
>Si le courrier électronique que vous envoyez à partir d’un programme d’engagement est un courrier électronique enfant d’un programme par défaut (et non local de votre programme d’engagement), tous les Mes jetons utilisés dans le courrier électronique sont résolus dans le programme par défaut dans lequel réside le courrier électronique enfant.

>[!MORELIKETHIS]
>
>* [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}
>* [Gestion de mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
