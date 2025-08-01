---
unique-page-id: 6094879
description: Ajout d’une URL Target à une campagne web - Documents Marketo - Documentation du produit
title: Ajout d’une URL Target à une campagne web
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 1%

---

# Ajout d’une URL Target à une campagne web {#adding-a-target-url-to-a-web-campaign}

L’URL de Target se trouve sous la page Définir la campagne et définit l’URL ou les URL spécifiques sur lesquelles une campagne web apparaîtra.

## Ajout d’une URL cible pour les campagnes web de boîte de dialogue ou de widget {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. Accédez à **[!UICONTROL Campagnes web]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Sélectionnez **[!UICONTROL Créer Une Campagne Web]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Ajoutez un **[!UICONTROL Nom de la campagne]**. Sélectionnez un **[!UICONTROL segment cible]**. Ajoutez **[!UICONTROL URL cible]**.

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
   <td colspan="1" rowspan="1"><strong>[!UICONTROL Any Page]</strong></td>
   <td colspan="1" rowspan="1"><p>Autoriser l’affichage de la campagne sur n’importe quelle page</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>[!UICONTROL Inclure le paramètre d’URL lors de la correspondance]</strong></p></td>
   <td colspan="1" rowspan="1">Ajoutez le paramètre d’URL pour faire correspondre et afficher la campagne sur les URL comprenant ce paramètre. Par exemple, campaign=cpc</td>
  </tr>
 </tbody>
</table>

## Ajout de plusieurs URL à l’URL cible {#adding-multiple-urls-to-target-url}

Cliquez sur l’icône plus (![-](assets/image2015-2-18-8-3a40-3a59.png)) pour ouvrir la boîte de dialogue [!UICONTROL Entrée de plusieurs valeurs] et ajouter plusieurs URL. Ajoutez une URL par ligne.

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* Les campagnes web de boîte de dialogue et de widget peuvent utiliser les options N’importe quelle page et Caractère générique (&#42;).
>* Dans les cas d’utilisation avancés, les campagnes web Dans la zone peuvent utiliser des caractères génériques à la fin du chemin de l’URL. Exemple : [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* L’URL respecte la casse.

## Ajout d’une URL Target pour les campagnes web de zone {#adding-a-target-url-for-in-zone-web-campaigns}

1. Accédez à **[!UICONTROL Campagnes web]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Sélectionnez **[!UICONTROL Créer Une Campagne Web]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Ajoutez un **[!UICONTROL Nom de la campagne]**. Sélectionnez un **[!UICONTROL segment cible]**. Ajoutez **[!UICONTROL URL cible]**.

   >[!NOTE]
   >
   >L’URL cible avec des zones d’entrée doit définir une ou plusieurs URL spécifiques. Dans les cas d’utilisation avancés, les campagnes web Dans la zone peuvent utiliser des caractères génériques à la fin du chemin de l’URL. Exemple : [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [Créer une campagne de dialogue](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Créer un RTP dans Zone Campaign](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Créer une campagne de widget RTP](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
