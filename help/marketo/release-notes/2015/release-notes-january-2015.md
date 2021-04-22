---
unique-page-id: 4720758
description: Notes de mise à jour - Janvier 2015 - Marketo Docs - Documentation du produit
title: Notes de mise à jour - Janvier 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 4%

---

# Notes de mise à jour : Janvier 2015 {#release-notes-january}

Les fonctionnalités suivantes sont incluses dans la version de janvier 2015. Veuillez vérifier la disponibilité des fonctionnalités de Marketo Edition. Après la publication, n&#39;oubliez pas de revenir pour trouver des liens vers des articles détaillés pour chaque fonctionnalité !

## Mises à jour de l’automatisation marketing {#marketing-automation-updates}

**Landings page compatibles avec les dispositifs portables**

Vous pouvez désormais [créer des vues mobiles pour les landings page](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) à partir de l&#39;éditeur de landings page. Diffusez efficacement votre message, quel que soit le périphérique, et augmentez l’engagement en adaptant votre contenu pour une consommation facile en déplacement. Cette fonctionnalité sera progressivement introduite au cours de la semaine qui suit la publication.

[-Vidéo de présentation par Landing page](https://youtu.be/aPQHlG2X6c0)

**Nouveaux appels d’API REST**

Trois nouveaux appels pour l&#39;API ReST de piste et d&#39;Activité :

* Supprimer lead
* Obtenir des pistes par identifiant de Programme
* Obtenir les pistes supprimées

Il existe également une nouvelle option pour l&#39;option &quot;Piste de synchronisation&quot;, qui permet d&#39;écrire la modification de piste de manière asynchrone pour un appel d&#39;API plus rapide. Les détails complets seront disponibles après la publication à l’adresse [developpeurs.marketo.com](https://developers.marketo.com).

**Prise en charge des objets personnalisés dans le script d’e-mail**

Accédez maintenant aux objets personnalisés associés à l’objet Compte dans les scripts de courrier électronique !

## Real-Time Personalization (Personnalisation en temps réel){#real-time-personalization}

**Remarketing personnalisé pour Google et Facebook**

Le remarketing présente des publicités destinées aux visiteurs de votre site Web. Vous pouvez désormais personnaliser vos campagnes de remarketing sur [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) et [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) à l’aide des données de la personnalisation en temps réel. Remarquez les audiences provenant de différents secteurs d&#39;activité, les listes de compte nommées, la taille des sociétés ou toute donnée provenant de pistes connues.

[Module de Liste de compte nommé](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Les améliorations apportées au module Comptes nommés amélioreront les taux de correspondance et les validations pour les utilisateurs. Les ajouts incluent :

* Association d’organisations à partir de votre liste de comptes nominés à l’aide de l’adresse électronique de l’prospect (également pour les clients RTP uniquement)
* Prise en charge de jusqu’à 100 000 enregistrements par compte
* Modèle de fichier CSV à vue et à télécharger

![](assets/image2015-1-14-11-3a12-3a16.png)

**Options de balise RTP mises à jour**

Les options de balise RTP sous Paramètres du compte ont été mises à jour pour inclure :

1. CDN et asynchrone (balise recommandée)
1. CDN et synchrone (haute vitesse)
1. Balise asynchrone sans CDN
1. Balise synchrone sans CDN

Pour de meilleures performances, il est recommandé de placer la balise en haut de l’en-tête dans votre page Web après `<head>`. Toutes les balises permettent l&#39;utilisation de l&#39;[API RTP](https://developers.marketo.com/documentation/websites/rtp-js-api/). Pour plus d’informations sur la façon de déployer la balise RTP, voir [ici](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
