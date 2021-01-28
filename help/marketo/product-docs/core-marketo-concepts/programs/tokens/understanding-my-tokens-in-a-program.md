---
unique-page-id: 1147114
description: Présentation de mes jetons dans un Programme - Documents marketing - Documentation du produit
title: Présentation de mes jetons dans un Programme
translation-type: tm+mt
source-git-commit: e5050328cbddaf072dd60ddd8d7363a704e720b5
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# Présentation de mes jetons dans un Programme {#understanding-my-tokens-in-a-program}

Un jeton est une variable que vous pouvez utiliser dans les courriels, les landings page et les campagnes intelligentes pour simplifier votre vie.

Outre Mes jetons, vous pouvez également utiliser n’importe lequel des jetons intégrés de vos programmes. Consultez la section [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md).

## Mes jetons {#my-tokens}

Mes jetons sont des variables personnalisées que tout le monde peut créer. Ils sont [créés](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) dans des dossiers de campagne ou des programmes.

Mes jetons s&#39;affichent comme suit : `{{my.Name Of Token}}`

Exemples :

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
   <td>Fichier de calendrier <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilisez ce jeton pour <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">ajouter un fichier de événement de calendrier (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> à vos courriels et landings page.</td> 
  </tr> 
  <tr> 
   <td><p>Date <img alt="—" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Ce jeton contient une valeur de date. La date s’affiche sous forme d’année-mois-jour (p. ex., 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>Script de courriel <img alt="—" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilisez ce jeton pour exécuter un script Velocity dans vos courriels. Pour en savoir plus <a href="http://developers.marketo.com/documentation/email-scripting/" title="Lien de suivi" rel="nofollow">ici</a>. </td> 
  </tr> 
  <tr> 
   <td>Nombre<span> <img alt="—" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Tout entier. Cela peut même être négatif.</td> 
  </tr> 
  <tr> 
   <td>Texte enrichi <img alt="—" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Il s'agit de HTML. Utilisez-le dans les courriers électroniques et les landings page.</td> 
  </tr> 
  <tr> 
   <td>Score <img alt="—" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilisez ce jeton dans l'<a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">étape de flux de note de modification</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC Campaign <img alt="—" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="—"></td> 
   <td colspan="1">Utilisez ce jeton pour autoriser l’ajout de pistes qui font partie d’un Programme Marketo à n’importe quel Campaign SFDC.</td> 
  </tr> 
  <tr> 
   <td>Texte <img alt="—" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Juste du texte. Utilisez-la lorsque le code HTML est en excès. La taille maximale des jetons de texte est de 524 288 caractères (UTF-8), soit 2 Mo.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Mes jetons ne seront pas résolus lors de l&#39;envoi d&#39;un courrier électronique à partir de Sales Insight sur Microsoft Dynamics ou Salesforce ; seuls les jetons standard sont renseignés (piste, Société, etc.). Cependant, les valeurs par défaut des jetons _fonctionneront_.

## Jetons imbriqués {#nesting-tokens}

Lorsque vous créez un jeton, il peut être référencé par d’autres objets de l’arborescence. Il existe une structure d&#39;attribution de noms pour l&#39;emplacement où le jeton a été créé afin d&#39;en faciliter la gestion.

* **Jeton local :** le jeton a été créé directement dans ce programme ou dossier.
* **Jeton hérité :** le jeton a été créé dans l’arborescence dans un programme ou un dossier de niveau supérieur.
* **Jeton remplacé :** le jeton a été hérité, puis quelqu’un a fait une exception dans ce programme ou dossier.

Vous pouvez créer des variables globales, puis les remplacer à des niveaux inférieurs dans l’arborescence.

Le déplacement de programmes et de dossiers affecte également les jetons. Vérifiez toujours que les références ne sont pas rompues pendant le déplacement.

>[!NOTE]
>
>Si le courrier électronique que vous envoyez à partir d’un programme d’engagement est un message électronique enfant d’un programme par défaut (qui n’est pas local à votre programme d’engagement), tous les jetons utilisés dans le courrier électronique sont résolus à partir du programme par défaut dans lequel réside le courrier électronique enfant.

>[!MORELIKETHIS]
>
>* [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [Gestion de mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

