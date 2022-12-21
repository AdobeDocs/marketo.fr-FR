---
unique-page-id: 4720917
description: Remarketing personnalisé dans Facebook - Documents Marketo - Documentation du produit
title: Remarketing personnalisé dans Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 6%

---

# Remarketing personnalisé dans Facebook {#personalized-remarketing-in-facebook}

Le remarketing personnalisé vous permet de réengager vos utilisateurs à l’aide des données RTP et de la puissance du remarketing Facebook.

>[!PREREQUISITES]
>
>* Procédez comme suit : [Reciblage à l’aide de données de personnalisation web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) setup
>* Consultez la section [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Documentation facebook sur les audiences personnalisées](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) et Remarketing.


## Création d’une audience dans Facebook {#creating-an-audience-in-facebook}

1. Dans Facebook, accédez à la [Onglet Audience](https://www.facebook.com/ads/audience_manager) dans Ads Manager.

1. Cliquez sur **Outils** et sélectionnez **Audiences**.

   ![](assets/one-1.png)

1. Cliquez sur **Création d’une audience personnalisée**.

   ![](assets/two-1.png)

1. Sélectionner **Trafic du site web**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Dans la liste Trafic du site Web, sélectionnez **Combinaison personnalisée**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Dans la liste Inclure, sélectionnez **Événement**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Dans la liste Evénement, sélectionnez **Remarketing RTP** et sélectionnez un paramètre.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Pour cet exemple, sélectionnez Secteur à contenir. **Éducation**. Entrée **Éducation** et modifier **Dans le dernier** pour 180 jours. Saisissez le nom de l’audience : **Secteur de l&#39;éducation**. Cliquez sur **Création d’une audience**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Vous avez maintenant créé une audience personnalisée à l’aide des données RTP dans Facebook.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## Points de données RTP dans Facebook {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>Nom de l'événement</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>Remarketing RTP</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>Paramètre</th> 
        <th>Valeur</th> 
       </tr> 
       <tr> 
        <td>Liste ABM</td> 
        <td>(Nom de la liste basée sur les comptes)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Catégorie</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Groupe</td> 
        <td colspan="1"><p>Entreprise</p><p>Small &amp; Medium Business</p></td> 
       </tr> 
       <tr> 
        <td>Secteur</td> 
        <td><p>Défense</p><p>Formation</p><p>Services financiers</p><p>État</p><p>Santé, pharmacie, biotechnologie</p><p>Logiciels et Internet</p><p>etc.. (conformément aux options du secteur de la technologie de pointe)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Public segmenté</td> 
        <td colspan="1">(Nom de l’audience segmentée créée dans RTP)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Ciblage de votre audience avec une publicité {#target-your-audience-with-an-ad}

Pour plus d’informations, voir [Documentation de facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Accédez au Gestionnaire de publicités, puis cliquez sur **Créer une publicité**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Sélectionner **Envoyer des personnes à votre site web** comme objectif de votre campagne.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Saisissez l’URL de votre site web.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Créez votre visionneuse d’annonces. Sélectionnez une audience personnalisée dans la liste des audiences que vous avez créées, par exemple, le secteur de l’éducation.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Sélectionnez toutes les autres options de jeux de publicités, définissez votre budget et vos créations publicitaires.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Vous êtes désormais tous configurés avec une campagne de remarketing personnalisée dans Facebook.

>[!MORELIKETHIS]
>
>* [Reciblage à l’aide de données de personnalisation web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personnalisé dans Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

