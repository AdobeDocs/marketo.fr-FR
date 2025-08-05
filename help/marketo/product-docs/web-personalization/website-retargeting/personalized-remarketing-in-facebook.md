---
unique-page-id: 4720917
description: Remarketing personnalisé sur Facebook - Documents Marketo - Documentation du produit
title: Remarketing personnalisé sur Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
feature: Web Personalization
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 8%

---

# Remarketing personnalisé dans [!DNL Facebook] {#personalized-remarketing-in-facebook}

Le remarketing personnalisé vous permet de réengager vos utilisateurs à l’aide des données RTP et de la puissance du remarketing Facebook.

>[!PREREQUISITES]
>
>* Effectuez la configuration [Reciblage avec données Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Consultez la [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [documentation Facebook sur les audiences personnalisées](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) et le remarketing.

## Création d’une audience dans [!DNL Facebook] {#creating-an-audience-in-facebook}

1. Dans [!DNL Facebook], accédez à l’onglet [ Audience ](https://www.facebook.com/ads/audience_manager) dans le Gestionnaire de publicités.

1. Cliquez sur **[!UICONTROL Outils]** et sélectionnez **[!UICONTROL Audiences]**.

![](assets/one-1.png)

1. Cliquez sur **[!UICONTROL Créer une audience personnalisée]**.

![](assets/two-1.png)

1. Sélectionnez **[!UICONTROL Trafic du site web]**.

![](assets/image2015-1-19-16-3a32-3a2.png)

1. Dans la liste [!UICONTROL Trafic du site Web], sélectionnez **[!UICONTROL Combinaison personnalisée]**.

![](assets/image2015-1-19-16-3a33-3a21.png)

1. Dans la liste Inclure, sélectionnez **[!UICONTROL Événement]**.

![](assets/image2015-1-19-16-3a34-3a9.png)

1. Dans la liste [!UICONTROL Événement], sélectionnez **[!UICONTROL Remarketing RTP]** et sélectionnez un paramètre.

![](assets/image2015-1-19-16-3a52-3a29.png)

1. Pour cet exemple, sélectionnez [!UICONTROL Industrie] pour contenir **[!UICONTROL Éducation]**. Entrez **[!UICONTROL Formation]** et modifiez **[!UICONTROL Au cours des derniers]** pour être de 180 jours. Saisissez le nom de l’audience : **secteur de l’éducation**. Cliquez sur **[!UICONTROL Créer une audience]**.

![](assets/image2015-1-19-16-3a56-3a15.png)

1. Vous avez maintenant créé une audience personnalisée à l’aide des données RTP dans [!DNL Facebook].

![](assets/image2015-1-19-16-3a59-3a2.png)

## Points de données RTP dans [!DNL Facebook] {#rtp-data-points-in-facebook}

<table>
 <tbody>
  <tr>
   <th>Nom de l’événement</th>
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
        <td colspan="1"><p>Entreprise</p><p>PME</p></td>
       </tr>
       <tr>
        <td>Secteur industriel</td>
        <td><p>Défense</p><p>Formation</p><p>Services financiers</p><p>État</p><p>Santé, Pharmacie, Biotechnologie</p><p>Logiciels et Internet</p><p>etc... (selon les options de RTP Industry)</p></td>
       </tr>
       <tr>
        <td colspan="1">Public segmenté</td>
        <td colspan="1">(Nom de l’audience segmentée créée dans le RTP)</td>
       </tr>
      </tbody>
     </table>
    </div></td>
  </tr>
 </tbody>
</table>

## Cibler votre audience avec une publicité {#target-your-audience-with-an-ad}

Pour plus d’informations, voir [documentation de Facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Accédez au Gestionnaire de publicités, cliquez sur **[!UICONTROL Créer une publicité]**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Sélectionnez **[!UICONTROL Envoyer des personnes à votre site web]** comme objectif de votre campagne.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Saisissez l’URL de votre site web.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Créez votre visionneuse d’annonces. Sélectionnez une audience personnalisée dans la liste des audiences que vous avez créées, par exemple, Secteur de l’éducation.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Sélectionnez toutes les autres options de visionneuse d’annonces, définissez votre budget et vos contenus publicitaires.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Vous disposez désormais tous d’une campagne de remarketing personnalisée en [!DNL Facebook].

>[!MORELIKETHIS]
>
>* [Reciblage avec des données Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [ Remarketing personnalisé dans Google ](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
