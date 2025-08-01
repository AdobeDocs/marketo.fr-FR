---
unique-page-id: 1147114
description: Présentation de mes jetons dans un programme - Documents Marketo - Documentation du produit
title: Présentation de mes jetons dans un programme
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 4%

---

# Présentation de mes jetons dans un programme {#understanding-my-tokens-in-a-program}

Un jeton est une variable que vous pouvez utiliser dans les e-mails, les landing pages et les campagnes intelligentes pour vous faciliter la vie.

Outre Mes jetons, vous pouvez également utiliser l’un des jetons intégrés dans vos programmes. Consultez la [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}.

## Mes jetons  {#my-tokens}

Mes jetons sont des variables personnalisées que tout le monde peut créer. Localement, ils sont [créés](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} dans des dossiers ou des programmes de campagne.

Mes jetons s’affichent comme suit : `{{my.Name Of Token}}`

Exemples :

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
   <td>Utilisez ce jeton pour <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">ajouter un fichier d’événement de calendrier (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> à vos e-mails et landing pages.</td>
  </tr>
  <tr>
   <td><p>Date <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td>
   <td>Ce jeton contient une valeur de date. La date s’affiche sous la forme année-mois-jour (par exemple, 2016-05-23).</td>
  </tr>
  <tr>
   <td>Script de l’e-mail <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Utilisez ce jeton pour exécuter un script Velocity dans vos e-mails. En savoir plus <a href="https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/email-scripting" title="Suivre le lien" rel="nofollow">ici</a>. </td>
  </tr>
  <tr>
   <td>Nombre <span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td>
   <td>N’importe quel entier. Elle peut même être négative.</td>
  </tr>
  <tr>
   <td>Texte complet <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Voici HTML. Utilisez-la dans les e-mails et les landing pages.</td>
  </tr>
  <tr>
   <td>Score <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Utilisez ce jeton dans l’étape <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">modifier le flux de score</a>. </td>
  </tr>
  <tr>
   <td colspan="1">Campagne SFDC <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td>
   <td colspan="1">Utilisez ce jeton pour autoriser les prospects qui font partie d’un programme Marketo à être également ajoutés à toute campagne SFDC.</td>
  </tr>
  <tr>
   <td>Texte <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Juste du texte. Utilisez-le lorsque HTML est trop puissant. La taille maximale des jetons de texte est de 524 288 caractères (UTF-8), soit 2 Mo.</td>
  </tr>
 </tbody>
</table>

>[!CAUTION]
>
>Mes jetons ne seront pas résolus lors de l’envoi d’un e-mail de Sales Insight sur [!DNL Microsoft Dynamics] ou [!DNL Salesforce] ; seuls les jetons standard seront renseignés (prospect, société, etc.). Les valeurs par défaut des jetons _vont_ fonctionnent toutefois.

## Imbrication de jetons {#nesting-tokens}

Lorsque vous créez un jeton, il peut être référencé par d’autres objets dans l’arborescence. Il existe une structure de dénomination pour l’emplacement où le jeton a été créé afin de faciliter la gestion.

* **Jeton local :** le jeton a été créé directement dans ce programme ou dossier.
* **Jeton hérité :** le jeton a été créé dans l’arborescence quelque part dans un programme ou un dossier de niveau supérieur.
* **Jeton remplacé :** le jeton a été hérité, puis une exception a été créée dans ce programme ou dossier.

Vous pouvez créer des variables globales, puis les remplacer à des niveaux inférieurs dans l’arborescence.

Le déplacement de programmes et de dossiers affecte également les jetons. Vérifiez toujours que les références ne sont pas rompues lors du déplacement.

>[!IMPORTANT]
>
>Les jetons imbriqués ne sont pas pris en charge dans les [campagnes par lots](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/understanding-batch-and-trigger-smart-campaigns.md#batch-campaign){target="_blank"}.

>[!NOTE]
>
>Si l’e-mail que vous envoyez à partir d’un programme d’engagement est un e-mail enfant d’un programme par défaut (et non local à votre programme d’engagement), tous les jetons utilisés dans l’e-mail sont résolus à partir du programme par défaut dans lequel réside l’e-mail enfant.

>[!MORELIKETHIS]
>
>* [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}
>* [Gestion de mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
