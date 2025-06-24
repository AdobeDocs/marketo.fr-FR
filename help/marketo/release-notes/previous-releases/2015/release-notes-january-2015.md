---
unique-page-id: 4720758
description: Notes De Mise À Jour - Janvier 2015 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Janvier 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 3%

---

# Notes De Mise À Jour : Janvier 2015 {#release-notes-january}

Les fonctionnalités suivantes sont incluses dans la version de janvier 2015. Consultez votre édition Marketo pour connaître la disponibilité des fonctionnalités. Après la publication, veillez à revenir pour trouver des liens vers des articles détaillés pour chaque fonctionnalité.

## Mises à jour de l’automatisation du marketing {#marketing-automation-updates}

**Pages de destination compatibles avec les appareils mobiles**

Vous pouvez désormais [créer des vues mobiles pour les pages de destination](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) à partir de l’éditeur de page de destination. Diffusez votre message efficacement, quel que soit l’appareil et augmentez l’engagement en personnalisant votre contenu pour une consommation facile en déplacement. Cette fonctionnalité sera déployée progressivement tout au long de la semaine suivant la publication de la version.

[-Présentation De La Page De Destination Vidéo-](https://youtu.be/aPQHlG2X6c0)

**Nouveaux appels de l’API REST**

Trois nouveaux appels pour l’API REST de lead et d’activité :

* Supprimer un lead
* Obtenir les leads par ID de programme
* Obtenir les leads supprimés

Il existe également une nouvelle option pour le prospect de synchronisation, permettant d’écrire le changement de prospect de manière asynchrone pour un appel API plus rapide. Des détails complets seront disponibles après la publication sur [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/home](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/home)

**Prise en charge des objets personnalisés dans le script d’e-mail**

Accédez maintenant aux objets personnalisés associés à l’objet Compte dans les scripts d’e-mail.

## Personnalisation en temps réel {#real-time-personalization}

**Remarketing personnalisé pour Google et[!DNL Facebook]**

Le remarketing présente des publicités destinées aux personnes qui ont visité votre site web. Vous pouvez désormais personnaliser vos campagnes de remarketing sur [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) et [[!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) à l’aide des données de Real-Time Personalization. Remarquez les audiences de différents secteurs d’activité, les listes de comptes nommés, les tailles d’entreprise ou toute donnée provenant de prospects connus.

[Module de liste de comptes nommés](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Les améliorations apportées au module Comptes nommés amélioreront les taux de correspondance et les validations pour les utilisateurs. Les ajouts incluent :

* Correspondance des organisations de votre liste de comptes nommés à l’aide de l’adresse e-mail du prospect (également pour les clients RTP uniquement)
* Prise en charge de 100 000 enregistrements maximum par compte
* Modèle de fichier CSV à afficher et à télécharger

![](assets/image2015-1-14-11-3a12-3a16.png)

**Mise à jour des options de balise RTP**

Les options de balise RTP sous Paramètres du compte ont été mises à jour pour inclure les éléments suivants :

1. Réseau CDN et asynchrone (balise recommandée)
1. Réseau CDN et synchrone (haute vitesse)
1. Balise asynchrone sans réseau CDN
1. Balise synchrone sans réseau CDN

Pour de meilleures performances, il est recommandé de placer la balise en haut de l’en-tête de votre page web après `<head>`. Toutes les balises permettent d’utiliser l’[API RTP](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation). Pour plus d’informations sur le déploiement de la balise RTP, voir [ici](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
