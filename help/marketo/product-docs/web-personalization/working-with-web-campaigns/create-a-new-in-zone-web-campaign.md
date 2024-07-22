---
unique-page-id: 4719400
description: Créer une campagne web dans Zone - Documents Marketo - Documentation du produit
title: Créer une campagne web dans la zone
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 1%

---

# Créer une campagne web dans la zone {#create-a-new-in-zone-web-campaign}

Une campagne web est une réaction personnalisée associée à un segment spécifique et peut être une [boîte de dialogue](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) sur votre site web, un remplacement de zone, une [fonction de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) ou une alerte par e-mail. Une campagne web In Zone remplace un élément de votre site web basé sur l’identifiant de zone par du contenu ou des bannières graphiques.

## Créer une campagne web dans la zone {#create-an-in-zone-web-campaign}

1. Accédez à **Campagnes Web**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Sélectionnez **Créer une campagne web.**

   ![](assets/create-new-web-campaign-hand.png)

1. Sélectionnez le type de campagne **Dans Zone** . Personnalisez et ajoutez un **ID Zone.** Définissez la campagne sur **Attractif** et ajoutez votre contenu créatif dans l’éditeur. Ajoutez l’URL de la page à prévisualiser et cliquez sur **Aperçu** pour voir comment la campagne va réagir sur votre site.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Qu’est-ce qu’un identifiant de zone ?**
   >
   >Un ID de zone est l’emplacement sur lequel vous souhaitez que votre campagne web &quot;Dans la zone&quot; soit située sur le site. Pour trouver un &quot;Zone ID&quot;, accédez simplement à votre site web et sélectionnez la zone que vous souhaitez remplacer par une campagne web, puis cliquez avec le bouton droit de la souris. Dans Chrome, l’option est &quot;Elément Inspect&quot; ; dans d’autres navigateurs, elle peut varier.
   >
   >Ensuite, vous souhaitez trouver l’&quot;id&quot; associé à cette section du site web, qui est mis en surbrillance car vous inspectez cet élément. Par exemple, si vous cliquez avec le bouton droit de la souris dans Chrome, le texte mis en surbrillance indique `<div id="featured-slider">`, alors &quot;feature-slider&quot; est ce que vous devez saisir dans la section &quot;zone id&quot;. En règle générale, &quot;div id&quot; est utilisé, mais tout ID peut également être utilisé, comme l’ID h1, l’ID p, etc.

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
   <td colspan="1" rowspan="1"><p>Saisissez le nom de l'identifiant présent dans le code d'HTML de l'élément de votre site web que remplace la campagne.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Fixe </strong></p></td> 
   <td colspan="1" rowspan="1">La case à cocher Attractif est sélectionnée par défaut pour la campagne Dans la zone et conserve la campagne Dans la zone à sa position d’identifiant de zone pendant toute la session du visiteur sur le site web. Il est recommandé de toujours définir une zone Dans sur Attractif.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Fondu</strong> </p></td> 
   <td colspan="1" rowspan="1">Si vous cochez la case Utiliser l’effet et Fondu , l’effet de fondu s’atténue dans la zone d’identifiant de zone du site web. Si la zone In Zone est une bannière graphique, la page se charge d’abord, puis la campagne s’active avec un effet de fondu.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Glissement</strong></td> 
   <td colspan="1">La sélection de la case à cocher Utiliser l’effet et de l’option Glisser permet de faire glisser l’effet vers la zone d’ID de zone du site web. Si l’option Dans la zone est une bannière graphique, la page se charge d’abord, puis la campagne s’active avec un effet coulissant de gauche à droite.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Éditeur de texte enrichi  </strong></td> 
   <td colspan="1">L’éditeur de texte enrichi permet le formatage de texte, la liaison et l’insertion d’images. <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">En savoir plus ici</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Aperçu sur le site   </strong></td> 
   <td colspan="1">Prévisualisez les campagnes avant de les lancer. <br> 
    <ul> 
     <li> URL : saisissez un exemple d’URL où s’exécuterait la campagne pour afficher un exemple d’aperçu de l’aspect réel de la campagne.</li> 
     <li>Appareil : prévisualisez l’affichage de votre campagne par appareil : Bureau, Portrait mobile, Paysage mobile, Portrait tablette, Paysage portrait.</li> 
     <li> Aperçu : cliquez sur <strong>Aperçu</strong> pour ouvrir une nouvelle fenêtre de l’exemple d’URL afin de visualiser la réaction de la campagne.</li> 
     <li> Partager : utilisez le bouton Partager pour envoyer un courrier électronique à un collègue contenant un lien pour afficher la campagne proxy.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Accélérez et simplifiez votre processus de création de campagne en utilisant nos [modèles intégrés](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) ou en [enregistrant votre campagne existante](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) comme modèle à réutiliser.

>[!NOTE]
>
>**Vous souhaitez tester vos campagnes web ?** Une ou plusieurs campagnes web peuvent être [A/B testées pour des résultats optimaux](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). Grâce à la fonctionnalité d’optimisation automatique, la plateforme reconnaît automatiquement les campagnes les plus performantes, poursuit avec le taux de conversion le plus élevé et met les autres en pause.

## Modifier une campagne web {#edit-a-web-campaign}

Sur la page **Campagnes Web**, cliquez sur **Modifier** dans la campagne.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Pour faciliter la recherche de la campagne de votre choix, utilisez la [fonction de filtrage](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## Prévisualiser une campagne web {#preview-a-web-campaign}

1. Sur la page Campagnes Web, cliquez sur **Aperçu** dans la campagne Web que vous souhaitez afficher.

   ![](assets/in-zone-web-campaign-preview.png)

## Cloner une campagne web {#clone-a-web-campaign}

Voir [Cloner une campagne web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Supprimer une campagne web {#delete-a-web-campaign}

1. Sur la page Campagnes Web, cliquez sur **Supprimer** dans la campagne que vous souhaitez supprimer.

   ![](assets/in-zone-web-campaign-delete.png)

1. Un message de confirmation s’affiche pour confirmer si vous souhaitez supprimer la campagne.

>[!MORELIKETHIS]
>
>* [Créer une campagne web de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Créer une campagne Web de boîte de dialogue](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
