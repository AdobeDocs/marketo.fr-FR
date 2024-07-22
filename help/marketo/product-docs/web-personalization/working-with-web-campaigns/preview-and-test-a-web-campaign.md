---
unique-page-id: 10092925
description: Aperçu et test d’une campagne web - Documents Marketo - Documentation du produit
title: Prévisualiser et tester une campagne web
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Prévisualiser et tester une campagne web {#preview-and-test-a-web-campaign}

Cet article vous présente différentes manières de prévisualiser une campagne web, ainsi que comment la tester à l’aide d’un segment sandbox actif sur votre site web.

>[!NOTE]
>
>L’aperçu affiche uniquement l’aspect de la campagne sur le site choisi. Les liens et les widgets ne seront pas fonctionnels afin d’éviter les clics/vues erronés dans les analyses.

## Prévisualiser une campagne web sur la page de création {#preview-a-web-campaign-on-the-creation-page}

1. Accédez à **Campagnes Web**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Cliquez sur **Créer une campagne web** ou sur l&#39;icône pour modifier une campagne existante.

   ![](assets/create-new-or-edit-web-campaign.png)

1. Dans Preview on site, ajoutez l&#39;URL de la page et cliquez sur **Preview**. Une nouvelle fenêtre ou un nouvel onglet s’ouvre et affiche l’aperçu de l’opération.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Cliquez sur **Partager** pour ouvrir un email avec une URL fixe de l&#39;aperçu de campagne.

   >[!NOTE]
   >
   >Vous avez également la possibilité d’installer un module externe de navigateur ([Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) ou [Firefox](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)) pour obtenir un aperçu de la meilleure expérience de prévisualisation de votre campagne. Consultez la section ci-dessous.

## Aperçu d’une campagne web sur la page de création à l’aide du plug-in de navigateur {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Suivez les étapes 1 et 2 de la section ci-dessus.

1. Cliquez sur le lien vers le module externe de navigateur (dans ce cas, nous utilisons Chrome).

   ![](assets/4-1.png)

1. Une nouvelle fenêtre ou un nouvel onglet s’ouvre. Cliquez sur **Ajouter à Chrome**.

   ![](assets/five.png)

1. Cliquez sur **Ajouter l’extension**.

   ![](assets/six.png)

1. Revenez à Marketo. Ajoutez l’URL de la page et cliquez sur **Aperçu**.

   ![](assets/seven.png)

1. Une nouvelle fenêtre ou un nouvel onglet s’ouvre. Il vous permet de prévisualiser l’apparence de votre campagne sur un ordinateur, un téléphone ou une tablette.

   ![](assets/campaign-preview.png)

## Prévisualiser une campagne web sur la page des campagnes web {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Lorsque vous consultez la liste de vos campagnes web, sélectionnez simplement une campagne et cliquez sur l’icône **Aperçu** .

   ![](assets/web-campaigns-1-preview-hand.png)

   Facile !

## Prévisualiser une campagne web sur votre site web {#preview-a-web-campaign-on-your-website}

Créez un segment et une campagne d’environnement de test.

1. Accédez à **Segments**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Cliquez sur **Créer**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Nommez le segment.

1. Sous Comportement, faites glisser Inclure des pages sur la zone de travail. Ajoutez la valeur &#42;sandbox=1&#42;. Cliquez sur **Enregistrer et définir la campagne**.

   ![](assets/segment.png)

1. Sur la page Définir une campagne web , remplacez le segment cible par le segment sandbox en le sélectionnant dans la liste.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Terminez la création de la campagne et cliquez sur **Launch**.

   ![](assets/click-launch.jpg)

1. Accédez à votre site web, ajoutez le paramètre d’URL &quot;?sandbox=1&quot; à la fin de l’URL. Exemple : `www.marketo.com?sandbox=1`.

1. Découvrez les réactions à la campagne sur votre site web.

>[!NOTE]
>
>Les campagnes ne réagissent qu’une seule fois au cours d’une session de visiteur. Pour afficher à nouveau la campagne, effacez les cookies de votre navigateur.

>[!NOTE]
>
>Les campagnes de redirection ne peuvent pas être prévisualisées. Le seul moyen de les tester consiste à utiliser un segment sandbox (qui cible par des pages spécifiques - &#42;sandbox=redirect&#42;).
