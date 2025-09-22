---
unique-page-id: 4719400
description: Création d’une campagne web dans la zone - Documents Marketo - Documentation du produit
title: Créer une campagne web dans la zone
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 4%

---

# Créer une campagne web dans la zone {#create-a-new-in-zone-web-campaign}

Une campagne web est une réaction personnalisée associée à un segment spécifique et peut être une [boîte de dialogue](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) sur votre site web, un remplacement dans la zone, une [fonctionnalité de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) ou une alerte par e-mail. Une campagne web Dans la zone remplace un élément de votre site web basé sur l’identifiant de zone par du contenu ou des bannières graphiques.

## Création d’une campagne web dans la zone {#create-an-in-zone-web-campaign}

1. Accédez à **[!UICONTROL Campagnes web]**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Sélectionnez **[!UICONTROL Créer Une Campagne Web].**

   ![](assets/create-new-web-campaign-hand.png)

1. Sélectionnez le type de campagne **[!UICONTROL Dans la zone]**. Personnalisez et ajoutez un **[!UICONTROL ID de zone].** Définissez la campagne sur **[!UICONTROL Sticky]** et ajoutez votre contenu créatif dans l’éditeur. Ajoutez l’URL de la page à prévisualiser et cliquez sur **[!UICONTROL Aperçu]** pour voir comment la campagne réagira sur votre site.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Qu’est-ce qu’un identifiant de zone ?**
   >
   >L’identifiant de zone correspond à l’emplacement de la campagne web « [!UICONTROL In Zone] » sur le site. Pour trouver un « [!UICONTROL Identifiant de zone] », il vous suffit d’accéder à votre site web, de sélectionner la zone à remplacer par une campagne web et de cliquer avec le bouton droit de la souris. Dans Chrome, l’option est « Inspect Element », elle peut varier dans d’autres navigateurs.
   >
   >Ensuite, vous devez rechercher l’« id » associé à cette section du site web, qui est mis en surbrillance car vous inspectez cet élément. Par exemple, si une fois que vous avez cliqué avec le bouton droit de la souris dans Chrome, le texte mis en surbrillance indique `<div id="featured-slider">`, vous devez saisir « feature-slider » dans la section « zone id » (identifiant de zone). En règle générale, l’ID « div » est utilisé, mais n’importe quel ID peut également être utilisé, tel que l’ID h1, l’ID p, etc.

<table>
 <thead>
  <tr>
   <th colspan="1" rowspan="1">Nom</th>
   <th colspan="1" rowspan="1">Description</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><strong> ID de zone </strong></td>
   <td colspan="1" rowspan="1"><p>Saisissez le nom de l’identifiant trouvé dans le code HTML de l’élément de site web que la campagne remplace.</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong> Fixe </strong></p></td>
   <td colspan="1" rowspan="1">La case à cocher persistante est sélectionnée par défaut pour la campagne dans la zone et conserve la campagne dans la zone à sa position d’identifiant de zone tout au long de la session du visiteur sur le site web. Il est recommandé de toujours définir une zone d’entrée sur « Collant ».</td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong> Fondu</strong> </p></td>
   <td colspan="1" rowspan="1">Si vous cochez la case Utiliser l’effet et que l’option Fondu est sélectionnée, un effet de fondu est appliqué à la zone d’identifiant de zone du site web. Si la zone d’entrée est une bannière graphique, la page est d’abord chargée, puis la campagne est activée avec un effet de fondu.</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Glissement</strong></td>
   <td colspan="1">Si vous cochez la case Utiliser l’effet et que vous activez l’option Coulissement, un glissement s’effectue dans la zone d’identifiant de zone du site web. Si la zone d’insertion est une bannière graphique, la page commence par se charger, puis la campagne s’active avec un effet de glissement de la gauche vers la droite.</td>
  </tr>
  <tr>
   <td colspan="1"><strong> Éditeur de texte enrichi  </strong></td>
   <td colspan="1">L’éditeur de texte enrichi permet la mise en forme du texte, la liaison et l’insertion d’images. <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">En savoir plus ici</a> .</td>
  </tr>
  <tr>
   <td colspan="1"><strong> Aperçu sur le site   </strong></td>
   <td colspan="1">Prévisualisez les campagnes avant leur lancement. <br>
    <ul>
     <li> URL : saisissez un exemple d’URL où la campagne serait exécutée pour afficher un exemple d’aperçu de l’apparence de la campagne en direct.</li>
     <li>Appareil : prévisualisez l’aspect de votre campagne par appareil : ordinateur de bureau, portrait pour mobile, paysage pour mobile, portrait pour tablette, paysage pour portrait.</li>
     <li> Prévisualisation - Cliquez sur <strong>Prévisualisation</strong> pour ouvrir une nouvelle fenêtre de l’exemple d’URL et voir comment la campagne réagit.</li>
     <li> Partager : utilisez le bouton Partager pour envoyer un e-mail à un collègue avec un lien afin d’afficher la campagne proxy.</li>
    </ul></td>
  </tr>
 </tbody>
</table>

>[!TIP]
>
>Accélérez et simplifiez le processus de création de vos campagnes à l’aide de nos [modèles intégrés](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) ou en [enregistrant votre campagne existante](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) en tant que modèle à réutiliser.

>[!NOTE]
>
>**Vous souhaitez tester vos campagnes web A/B ?** Une ou plusieurs campagnes web peuvent être testées [A/B pour obtenir des résultats optimaux](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). Grâce à la fonction Réglage automatique, la plateforme reconnaît automatiquement les campagnes les plus performantes, continue avec les campagnes de conversion les plus performantes et met les autres en pause.

## Modification d’une campagne web {#edit-a-web-campaign}

Sur la page **Campagnes web**, cliquez sur **Modifier** dans la campagne.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Pour trouver plus facilement la campagne souhaitée, utilisez la [fonction de filtre](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## Prévisualiser une campagne web {#preview-a-web-campaign}

1. Sur la page [!UICONTROL Campagnes web], cliquez sur **[!UICONTROL Aperçu]** sur la campagne web que vous souhaitez afficher.

   ![](assets/in-zone-web-campaign-preview.png)

## Cloner une campagne web {#clone-a-web-campaign}

Voir [Cloner une campagne web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Supprimer une campagne web {#delete-a-web-campaign}

1. Sur la page Campagnes web, cliquez sur **[!UICONTROL Supprimer]** sur la campagne que vous souhaitez supprimer.

   ![](assets/in-zone-web-campaign-delete.png)

1. Un message de confirmation s’affiche pour confirmer la suppression de la campagne.

>[!MORELIKETHIS]
>
>* [Créer une campagne web de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Créer une campagne web de boîte de dialogue](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
