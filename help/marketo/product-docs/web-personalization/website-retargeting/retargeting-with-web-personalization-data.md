---
unique-page-id: 4720796
description: Reciblage à l’aide de données Web Personalization - Documents Marketo - Documentation du produit
title: Reciblage à l’aide de données Personalization web
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 1%

---

# Reciblage à l’aide de données Personalization web {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Le reciblage de site web tombe désormais sous la mosaïque Personalization web. Si vous avez acheté uniquement le ciblage, cette mosaïque s’affiche et accédez au produit Web Personalization avec les fonctions de ciblage **uniquement** activées. Vous avez ainsi accès aux paramètres du compte, à la page de reciblage, aux segments et aux pages de suivi supplémentaires.

Le remarketing cible les prospects qui ont déjà visité votre site avec de la publicité display en fonction de qui ils sont et de ce qu’ils ont fait. Le reciblage personnalisé cible des audiences spécifiques avec des publicités pertinentes basées sur le secteur, les comptes nommés et les données de personnes connues.

Web Personalization ajoute actuellement des données aux plateformes de remarketing suivantes :

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Web Personalization envoie les données suivantes aux plateformes de remarketing afin de créer des audiences et d’exécuter des campagnes publicitaires de remarketing :

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Données Personalization Web</th> 
  </tr> 
  <tr> 
   <th><p>Industrie</p></th> 
  </tr> 
  <tr> 
   <th><p>Groupe (Enterprise, SMB)</p></th> 
  </tr> 
  <tr> 
   <th><p>Catégorie (Fortune 500/1000, Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>Liste ABM (listes de comptes nommés)</p></th> 
  </tr> 
  <tr> 
   <th><p>Audience segmentée (basée sur des segments)</p></th> 
  </tr> 
  <tr> 
   <th><p>Campagnes web ayant fait l’objet d’un clic</p></th> 
  </tr> 
 </tbody> 
</table>

## Configuration des remarketing {#remarketing-configuration}

1. Accédez à **Reciblage**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configuration de reciblage est par domaine ou sous-domaine. Activez les autres domaines si vous souhaitez envoyer des données de ces domaines à la plateforme de reciblage.

1. Activez les paramètres pour les Google Analytics ou Google Universal Analytics par domaine.

   >[!NOTE]
   >
   >La balise de reciblage Google doit être implémentée sur votre site web.
   >
   >Si vous avez déjà configuré votre intégration avec Web Personalization et Google Analytics, il n’est pas nécessaire de modifier cette partie, car il s’agit de la même configuration sous Paramètres du compte.

   ![](assets/two.png)

1. Activez la configuration pour Facebook. Cliquez sur et développez l’accordéon Facebook, cliquez sur **On** pour envoyer l’événement et les données respectifs à l’Audience Manager Facebook. Cliquez sur **Enregistrer**.

   >[!NOTE]
   >
   >Pour que cette fonctionnalité fonctionne, [Facebook Custom Audience Pixel](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) doit être installé sur votre site web.

   ![](assets/three.png)

## Création d’une audience segmentée {#creating-segmented-audience}

Une audience segmentée permet de sélectionner un segment existant comme audience à utiliser pour les campagnes de reciblage. Par exemple, en sélectionnant vos segments Personne connue .

>[!TIP]
>
>Il n’est pas nécessaire de créer une audience segmentée pour le secteur ou d’autres données qui ont déjà été envoyées dans la configuration du domaine. Il est préférable d’utiliser des audiences segmentées pour les segments basés sur des données de personnes connues.

1. Cliquez sur **Créer une audience segmentée**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Saisissez le nom de l’audience, sélectionnez Canaux, puis Segment dans la liste des segments existants.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Cliquez sur **Enregistrer**.

   Vous avez terminé la configuration du reciblage dans Web Personalization, vous êtes connecté à vos plateformes de reciblage, vous créez vos audiences en fonction de ces données et vous configurez vos campagnes publicitaires de reciblage.
