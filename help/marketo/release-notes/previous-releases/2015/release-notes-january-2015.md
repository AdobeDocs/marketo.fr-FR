---
unique-page-id: 4720758
description: Notes de mise à jour - Janvier 2015 - Documentation Marketo - Documentation du produit
title: Notes de mise à jour - Janvier 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 4%

---

# Notes de mise à jour : janvier 2015 {#release-notes-january}

Les fonctionnalités suivantes sont incluses dans la version de janvier 2015. Vérifiez la disponibilité de vos fonctionnalités dans Marketo Edition. Après la publication de la version, veillez à revenir à la page de liens vers des articles détaillés pour chaque fonctionnalité.

## Mises à jour de l’automatisation du marketing {#marketing-automation-updates}

**Pages d’entrée compatibles avec les périphériques mobiles**

Vous pouvez désormais [création de vues mobiles pour les landing pages](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) depuis l’éditeur de landing page. Diffusez efficacement votre message quel que soit l’appareil utilisé et augmentez l’engagement en adaptant votre contenu pour une consommation facile à l’emploi. Cette fonctionnalité sera déployée progressivement au cours de la semaine qui suit la publication de la version.

[- Vidéo de présentation de la page d’entrée -](https://youtu.be/aPQHlG2X6c0)

**Nouveaux appels d’API REST**

Trois nouveaux appels pour l’API Lead &amp; Activity ReST :

* Supprimer un lead
* Obtenir des pistes par identifiant de programme
* Obtenir les pistes supprimées

Il existe également une nouvelle option pour le pistes de synchronisation, qui permet d’écrire le changement de piste de manière asynchrone pour un appel API plus rapide. Des détails complets seront disponibles après cette version à l’adresse [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/home](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/home)

**Prise en charge des objets personnalisés dans le script d’e-mail**

Accédez maintenant aux objets personnalisés associés à l’objet Compte dans les scripts de courrier électronique !

## Personnalisation en temps réel {#real-time-personalization}

**Remarketing personnalisé pour Google et Facebook**

Le remarketing présente des publicités destinées aux visiteurs de votre site Web. Vous pouvez désormais personnaliser vos campagnes de remarketing sur la page [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) et [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) à l’aide des données de la personnalisation en temps réel. Remarketing aux audiences provenant de différents secteurs, de listes de comptes nommés, de tailles d’entreprise ou de toute donnée provenant de pistes connues.

[Module de liste de comptes nommés](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Les améliorations apportées au module Comptes nommés amélioreront les taux de correspondance et les validations pour les utilisateurs. Les ajouts incluent :

* Correspondance d’organisations à partir de votre liste de comptes nommés à l’aide de l’adresse électronique du prospect (également pour les clients RTP uniquement)
* Prise en charge de 100 000 enregistrements par compte
* Modèle de fichier CSV à afficher et à télécharger

![](assets/image2015-1-14-11-3a12-3a16.png)

**Options de balise RTP mises à jour**

Les options de balise RTP sous Paramètres du compte ont été mises à jour afin d’inclure :

1. CDN et asynchrone (balise recommandée)
1. Réseau de diffusion de contenu et synchrone (haute vitesse)
1. Balise asynchrone sans CDN
1. Balise synchrone sans CDN

Pour de meilleures performances, il est recommandé de placer la balise en haut de l’en-tête de votre page web après `<head>`. Toutes les balises permettent d’utiliser la variable [API RTP](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation). Pour plus d’informations sur le déploiement de la balise RTP, voir [here](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
