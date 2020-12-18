---
unique-page-id: 4719400
description: Créer un Campaign Web en zone - Documents marketing - Documentation du produit
title: Créer une Campaign Web en zone
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---


# Créer une Campaign Web en zone {#create-a-new-in-zone-web-campaign}

Une campagne Web est une réaction personnalisée associée à un segment spécifique et peut être une [boîte de dialogue](create-a-new-dialog-web-campaign.md) sur votre site Web, un remplacement de zone, une fonction de widget [](create-a-new-widget-web-campaign.md) ou une alerte par courrier électronique. Une campagne Web In Zone remplace un élément de votre site Web basé sur l’identifiant de zone par du contenu ou des bannières graphiques.

## Créer une Campaign Web en zone {#create-an-in-zone-web-campaign}

1. Accédez à **Campagnes Web**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Sélectionnez **Créer une nouvelle Campaign Web.**

   ![](assets/create-new-web-campaign-hand.png)

1. Sélectionnez le type de campagne **Dans Zone**. Personnalisez et ajoutez un ID de zone **Zone.** Définissez la campagne sur  **** Attractif et ajoutez votre élément créatif dans l’éditeur. Ajoutez l’URL de la page à la prévisualisation et cliquez sur **Prévisualisation** pour savoir comment la campagne va réagir sur votre site.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >
   >**Qu’est-ce qu’un identifiant de zone ?**
   >
   >
   >Un identifiant de zone correspond à l’emplacement de votre campagne Web &quot;Dans la zone&quot; sur le site. Pour trouver un &quot;identifiant de zone&quot;, il vous suffit d&#39;aller sur votre site Web sélectionner la zone que vous souhaitez remplacer par une campagne Web et de cliquer avec le bouton droit de la souris. Dans Chrome, l’option est &quot;Inspect Element&quot;, et dans d’autres navigateurs, elle peut varier.
   >
   >
   >Ensuite, vous souhaitez trouver l&#39;&quot;id&quot; associé à cette section du site Web, qui est mise en évidence car vous inspectez cet élément. Par exemple, si vous cliquez avec le bouton droit de la souris dans Chrome, le texte en surbrillance indique `<div id="featured-slider">` alors &quot;featured-slider&quot; est ce que vous devez taper dans la section &quot;zone id&quot;. En règle générale, &quot;div id&quot; est utilisé, mais tout ID peut également être utilisé, tel que h1 id, p id, etc.

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
   <td colspan="1" rowspan="1"><p>Entrez le nom de l'identifiant figurant dans le code HTML de l'élément de site Web que la campagne remplace.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Attractif </strong></p></td> 
   <td colspan="1" rowspan="1">La case à cocher Attractif est cochée par défaut pour la campagne En zone et conserve la position d’ID de la campagne En zone dans l’ensemble de la session de l’visiteur sur le site Web. Il est recommandé de toujours définir une zone d’entrée sur Attractif.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Fondu</strong> </p></td> 
   <td colspan="1" rowspan="1">La sélection de la case à cocher Effet d’utilisation et Fondu permet d’atténuer la zone d’identifiant de zone du site Web. Si la zone d’entrée est une bannière graphique, la page est d’abord chargée, puis la campagne s’active avec un effet de fondu.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Diapositive</strong></td> 
   <td colspan="1">La sélection de la case à cocher Utiliser l’effet et de l’option Diapositive permet de faire glisser la zone d’identifiant de zone sur le site Web. Si la zone d’entrée est une bannière graphique, la page est d’abord chargée, puis la campagne s’active avec un effet de glissement de gauche à droite.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Editeur de texte enrichi  </strong></td> 
   <td colspan="1">L’éditeur de texte enrichi permet le formatage de texte, la liaison et l’insertion d’images. <a href="using-the-web-personalization-rich-text-editor.md">Lire plus ici</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Prévisualisation sur site   </strong></td> 
   <td colspan="1">Campagnes de prévisualisation avant leur lancement. <br> 
    <ul> 
     <li> URL : saisissez un exemple d'URL où la campagne s'exécuterait pour afficher un exemple prévisualisation de l'aspect de la campagne.</li> 
     <li>Périphérique - Prévisualisation de l'affichage de votre campagne par périphérique : Bureau, Portrait mobile, Paysage mobile, Portrait tablette, Paysage portrait.</li> 
     <li> Prévisualisation - Cliquez sur <strong>Prévisualisation</strong> pour ouvrir une nouvelle fenêtre de l'exemple d'URL afin de voir comment la campagne réagit.</li> 
     <li> Partager - Utilisez le bouton Partager pour envoyer un courriel à un collègue avec un lien afin d'afficher la campagne proxy.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Accélérez et simplifiez le processus de création de vos campagnes en utilisant [les modèles intégrés](../../../product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) ou en [enregistrant votre campagne existante](../../../product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) comme modèle à réutiliser.

>[!NOTE]
>
>**Souhaitez-vous tester A/B vos campagnes Web ?** Une ou plusieurs campagnes Web peuvent être testées  [A/B pour des résultats](ab-test-your-web-campaign.md) optimaux. Grâce à la fonction d’ajustement automatique, la plate-forme reconnaît automatiquement les campagnes les plus performantes, poursuit les campagnes ayant le plus fort taux de conversion et interrompt les autres campagnes.

## Modifier une Campaign Web {#edit-a-web-campaign}

Dans la page **Campagnes Web**, cliquez sur **Modifier** dans le Campaign.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Pour faciliter la recherche de la campagne souhaitée, utilisez la fonction de filtre [](filter-web-campaigns.md).

## Prévisualisation d’un Campaign Web {#preview-a-web-campaign}

1. Dans la page Campagnes Web, cliquez sur **Prévisualisation **sur la campagne Web que vous souhaitez vue.

   ![](assets/in-zone-web-campaign-preview.png)

## Cloner une Campaign Web {#clone-a-web-campaign}

Voir [Cloner une Campaign Web](clone-a-web-campaign.md).

## Supprimer une Campaign Web {#delete-a-web-campaign}

1. Dans la page Campagnes Web, cliquez sur **Supprimer **sur la Campaign que vous souhaitez supprimer.

   ![](assets/in-zone-web-campaign-delete.png)

1. Un message de confirmation s’affiche pour confirmer si vous souhaitez supprimer le Campaign.

>[!MORELIKETHIS]
>
>* [Créer un widget Web Campaign](create-a-new-widget-web-campaign.md)
>* [Créer une Campaign Web de boîte de dialogue](create-a-new-dialog-web-campaign.md)

