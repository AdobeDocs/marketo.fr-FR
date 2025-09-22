---
unique-page-id: 4720796
description: Reciblage avec des données Web Personalization - Documents Marketo - Documentation du produit
title: Reciblage avec des données de personnalisation web
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 3%

---

# Reciblage avec des données [!DNL Web Personalization] {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Le reciblage de site web se trouve désormais sous la mosaïque Web Personalization . Si vous avez acheté uniquement le reciblage, cette vignette s’affiche et vous accédez au produit [!DNL Web Personalization] avec les fonctionnalités de reciblage **uniquement** activées. Vous avez ainsi accès aux paramètres du compte, à la page de reciblage, aux segments et aux pages de suivi supplémentaires.

Le remarketing cible les prospects qui ont visité votre site par le passé avec des publicités display basées sur leur identité et leurs activités. Le reciblage personnalisé cible des audiences spécifiques avec des annonces pertinentes basées sur le secteur, les comptes nommés et les données de personnes connues.

Web Personalization ajoute actuellement des données aux plateformes de remarketing suivantes :

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

[!DNL Web Personalization] envoie les données suivantes aux plateformes de remarketing pour créer des audiences et exécuter des campagnes publicitaires de remarketing :

<table>
 <tbody>
  <tr>
   <th colspan="1">[!DNL Web Personalization] Données</th>
  </tr>
  <tr>
   <th><p>Secteur industriel</p></th>
  </tr>
  <tr>
   <th><p>Groupe (Entreprise, PME)</p></th>
  </tr>
  <tr>
   <th><p>Catégorie (Fortune 500/1000, Global 2000)</p></th>
  </tr>
  <tr>
   <th><p>Liste ABM (listes de comptes nommés)</p></th>
  </tr>
  <tr>
   <th><p>Audience Segmentée (basée sur les segments)</p></th>
  </tr>
  <tr>
   <th><p>Campagnes web sur lesquelles l’utilisateur a cliqué</p></th>
  </tr>
 </tbody>
</table>

## Configuration du remarketing {#remarketing-configuration}

1. Accédez à **[!UICONTROL Reciblage]**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >La configuration de reciblage s’applique par domaine ou sous-domaine. Activez les autres domaines si vous souhaitez envoyer des données de ces domaines vers la plateforme de reciblage.

1. Activer les paramètres pour Google Analytics ou [!DNL Google Universal Analytics] par domaine.

   >[!NOTE]
   >
   >La balise de reciblage Google doit être implémentée sur votre site web.
   >
   >Si vous avez déjà configuré votre intégration avec Web Personalization et Google Analytics, vous n’avez pas besoin de modifier cette partie, car il s’agit de la même configuration sous Paramètres du compte.

   ![](assets/two.png)

1. Activez la configuration pour Facebook. Cliquez sur l’accordéon [!DNL Facebook] et développez-le, puis cliquez sur **[!UICONTROL Activé]** pour envoyer l’événement et les données correspondants à Facebook Audience Manager. Cliquez sur **[!UICONTROL Enregistrer]**

   >[!NOTE]
   >
   >Pour que cette fonctionnalité fonctionne[[!DNL Facebook]  vous devez avoir installé ](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)Custom Audience Pixel sur votre site web.

   ![](assets/three.png)

## Création d’une audience segmentée {#creating-segmented-audience}

Une audience segmentée vous permet de sélectionner un segment existant en tant qu’audience à utiliser pour les campagnes de reciblage. Par exemple, en sélectionnant vos segments de personnes connues .

>[!TIP]
>
>Il n’est pas nécessaire de créer une audience segmentée pour les données du secteur ou d’autres données qui ont déjà été envoyées dans la configuration du domaine. Il est préférable d’utiliser des audiences segmentées pour les segments en fonction des données de personnes connues.

1. Cliquez sur **[!UICONTROL Créer une audience segmentée]**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Saisissez le Nom de l’audience, sélectionnez Canaux puis Segment dans la liste des Segments existants.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   Vous avez maintenant terminé la configuration du reciblage en [!DNL Web Personalization], vous vous connectez à vos plateformes de reciblage et créez vos audiences en fonction de ces données, puis configurez vos campagnes publicitaires de reciblage.
