---
unique-page-id: 6094879
description: Ajout d’une URL Target à une campagne web - Documents Marketo - Documentation du produit
title: Ajout d'une URL cible à une campagne web
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 3%

---

# Ajout d&#39;une URL cible à une campagne web {#adding-a-target-url-to-a-web-campaign}

Une URL cible se trouve sous la page Définir la campagne et définit la ou les URL spécifiques sur lesquelles une campagne web doit apparaître.

## Ajout d’une URL cible pour les campagnes web de boîte de dialogue ou de widget {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. Accédez à **Campagnes Web**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Sélectionnez **Créer une campagne web**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Ajoutez un **nom de campagne**. Sélectionnez un **segment cible**. Ajoutez **Target URL**.

   ![](assets/set-web-campaign-hands.jpg)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Nom</th> 
   <th colspan="1" rowspan="1">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Toutes les pages</strong></td> 
   <td colspan="1" rowspan="1"><p>Permet à la campagne d’apparaître sur n’importe quelle page.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Inclure les paramètres de l’URL lors des correspondances</strong></p></td> 
   <td colspan="1" rowspan="1">Ajoutez le paramètre d’URL à faire correspondre et affichez la campagne sur les URL, y compris ce paramètre. Par exemple, campaign=cpc</td> 
  </tr> 
 </tbody> 
</table>

## Ajout de plusieurs URL à une URL cible {#adding-multiple-urls-to-target-url}

Cliquez sur l’icône &quot;+&quot; (![—](assets/image2015-2-18-8-3a40-3a59.png)) pour ouvrir la boîte de dialogue Saisie de plusieurs valeurs afin d’ajouter plusieurs URL. Ajoutez une URL par ligne.

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* Les campagnes web de boîte de dialogue et de widgets peuvent utiliser les options N’importe quelle page et Caractère générique (&#42;).
* Dans les cas d’utilisation avancés, les campagnes Web In Zone peuvent utiliser des caractères génériques à la fin du chemin d’accès à l’URL. Exemple : [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
* L’URL est sensible à la casse

## Ajout d’une URL cible pour les campagnes web dans la zone {#adding-a-target-url-for-in-zone-web-campaigns}

1. Accédez à **Web** **Campagnes**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Sélectionnez **Créer une campagne web**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Ajoutez un **nom de campagne**. Sélectionnez un **segment cible**. Ajoutez **Target URL**.

   >[!NOTE]
   >
   L’URL cible avec des zones In Zones doit définir une ou plusieurs URL spécifiques. Dans les cas d’utilisation avancés, les campagnes Web In Zone peuvent utiliser des caractères génériques à la fin du chemin d’accès à l’URL. Exemple : [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
* [Créer une campagne de boîte de dialogue](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
* [Créer un RTP dans Zone Campaign](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
* [Créer une campagne de widget RTP](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
