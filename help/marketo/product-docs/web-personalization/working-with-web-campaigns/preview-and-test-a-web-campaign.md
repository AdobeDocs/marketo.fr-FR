---
unique-page-id: 10092925
description: Prévisualiser et tester une campagne web - Documents Marketo - Documentation du produit
title: Prévisualiser et tester une campagne web
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 4%

---

# Prévisualiser et tester une campagne web {#preview-and-test-a-web-campaign}

Cet article vous explique différentes manières de prévisualiser une campagne web et de la tester à l’aide d’un segment de sandbox en direct sur votre site web.

>[!NOTE]
>
>L’aperçu ne montre que l’aspect de la campagne sur le site sélectionné. Les liens et les widgets ne seront pas fonctionnels, de manière à éviter les clics/vues erronés dans les analyses.

## Prévisualiser une campagne web sur la page de création {#preview-a-web-campaign-on-the-creation-page}

1. Accédez à **[!UICONTROL Campagnes web]**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Cliquez sur **[!UICONTROL Créer une campagne web]** ou sur l’icône pour modifier une campagne existante.

   ![](assets/create-new-or-edit-web-campaign.png)

1. Dans Aperçu sur le site, ajoutez l’URL de la page et cliquez sur **[!UICONTROL Aperçu]**. Une nouvelle fenêtre/un nouvel onglet s’ouvre, affichant l’aperçu de la campagne.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Cliquez sur **[!UICONTROL Partager]** pour ouvrir un e-mail avec une URL fixe de l’aperçu de la campagne.

   >[!NOTE]
   >
   >Vous avez également la possibilité d’installer un plug-in de navigateur ([[!DNL Chrome]](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) ou [[!DNL Firefox]](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)) pour bénéficier de la meilleure expérience en prévisualisant votre campagne. Voir la section ci-dessous.

## Prévisualisez une campagne web sur la page de création à l’aide du module externe de navigateur {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Suivez les étapes 1 et 2 de la section ci-dessus.

1. Cliquez sur le lien vers le plug-in du navigateur (dans ce cas, nous utilisons [!DNL Chrome]).

   ![](assets/4-1.png)

1. Une nouvelle fenêtre/un nouvel onglet s’ouvre. Cliquez sur **[!UICONTROL Ajouter à Chrome]**.

   ![](assets/five.png)

1. Cliquez sur **[!UICONTROL Ajouter une extension]**.

   ![](assets/six.png)

1. Revenez à Marketo. Ajoutez l’URL de la page et cliquez sur **[!UICONTROL Aperçu]**.

   ![](assets/seven.png)

1. Une nouvelle fenêtre/un nouvel onglet s’ouvre, vous permettant de prévisualiser l’apparence de votre campagne sur un bureau, un téléphone ou une tablette.

   ![](assets/campaign-preview.png)

## Prévisualiser une campagne web sur la page des campagnes web {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Lorsque vous consultez la liste de vos campagnes web, sélectionnez simplement une campagne et cliquez sur l’icône **[!UICONTROL Aperçu]**.

   ![](assets/web-campaigns-1-preview-hand.png)

   Doucement !

## Prévisualiser une campagne web sur votre site web {#preview-a-web-campaign-on-your-website}

Créez un segment et une campagne sandbox.

1. Accédez à **[!UICONTROL Segments]**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Nommez le segment.

1. Sous [!UICONTROL Comportemental], faites glisser [!UICONTROL Inclure des pages] sur la zone de travail. Ajoutez la valeur &#42;sandbox=1&#42;. Cliquez sur **[!UICONTROL Enregistrer et définir la campagne]**.

   ![](assets/segment.png)

1. Sur la page Définir une campagne web , remplacez le segment cible par le segment sandbox en le sélectionnant dans la liste.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Terminez la création de la campagne et cliquez sur **[!UICONTROL Lancer]**.

   ![](assets/click-launch.jpg)

1. Sur votre site web, ajoutez le paramètre d’URL «?sandbox=1» à la fin de l’URL. Exemple : `www.marketo.com?sandbox=1`.

1. Affichez la réaction de la campagne sur votre site web.

>[!NOTE]
>
>Les campagnes ne réagissent qu’une seule fois au cours d’une session visiteur. Pour afficher à nouveau la campagne, effacez les cookies de votre navigateur.

>[!NOTE]
>
>Les campagnes de redirection ne peuvent pas être prévisualisées. La seule façon de les tester est d’utiliser un segment sandbox (qui cible par des pages spécifiques - &#42;sandbox=redirect&#42;)
