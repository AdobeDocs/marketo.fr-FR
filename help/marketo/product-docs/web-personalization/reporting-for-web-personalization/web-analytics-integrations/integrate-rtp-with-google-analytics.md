---
unique-page-id: 2949158
description: Intégration de RTP à Google Analytics - Documents Marketo - Documentation du produit
title: Intégration de RTP à des Google Analytics
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Intégration de RTP à des Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics est désormais la norme de fonctionnement et toutes les propriétés de Google ont été mises à niveau vers Universal Analytics.
>
>Cet article explique comment utiliser l’ancien Google Standard Analytics, mais nous vous recommandons de passer à Universal Analytics.
>
>Si vous n’utilisez pas encore le [code de suivi analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), Google vous recommande vivement de remarquer votre site pour l’utiliser. Google abandonne les éléments suivants :
>
>* ga.js
>* urchin.js
>* Fragments de code WAP/serveur
>* YT / MO
>* Variables personnalisées
>* Variables définies par l’utilisateur
>
>Découvrez comment intégrer [Web Personalization avec Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Introduction {#introduction}

Analysez vos analyses web sous un nouvel angle à l’aide du flux de données direct de Marketo Real-Time Personalization (RTP) vers votre compte Google Analytics (GA). Mesurez vos visites web en disponibilité générale en fonction des organisations, des secteurs et des campagnes RTP. Affichez des mesures telles que les types de secteurs ou de segments RTP dans la disponibilité générale et la manière dont ils exécutent et génèrent des pistes en fonction de différentes sources de trafic (sociales, payantes, organiques), analysez les taux de clics publicitaires sur les campagnes et mesurez l’impact des campagnes de personnalisation sur votre site web. Tirer parti de cette capacité pour tirer le meilleur parti de votre compte RTP

**Audience Analytics RTP**

Avec l’intégration, vous disposez d’une nouvelle dimension dans votre compte GA. La technologie RTP améliore automatiquement vos tableaux de bord avec :

1. Organisations et industries
1. Segments personnalisés dans RTP
1. Listes Account-Based Marketing

Concentrez-vous sur vos prospects B2B clés. Analysez les canaux par secteurs et segments ciblés.

## Rapport Canal {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

Le tableau de bord B2B RTP vous permet de comprendre la ventilation de vos visiteurs selon les secteurs verticaux et la segmentation RTP. Vous pouvez afficher les performances de vos visiteurs en fonction du secteur financier et de différentes campagnes marketing (payantes, organiques, sociales). Le tableau de bord fournit également un aperçu général des performances de vos segments RTP et détaille les principales organisations qui visitent votre site.

## Flux comportemental {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

Le rapport Flux de comportement (voir image) visualise le chemin que les visiteurs empruntent pour passer d’une page ou d’un événement à l’autre. L&#39;exemple d&#39;image montre le chemin de tous les visiteurs du secteur financier. Ce rapport peut vous aider à découvrir le contenu qui maintient les visiteurs en contact avec votre site.

## Performances RTP {#rtp-performance}

Mesurez vos campagnes RTP et corrélez-les à la moyenne globale de votre site. Découvrez comment ces campagnes affectent les mesures de votre site web et utilisez ces données pour concentrer vos efforts de personnalisation sur les cibles appropriées. Générez des rapports personnalisés pour mieux comprendre les performances de vos campagnes de personnalisation.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Configuration du protocole RTP avec des Google Analytics {#setting-up-rtp-with-google-analytics}

1. Ajoutez le courrier électronique rtp.ga2@gmail.com en tant qu’utilisateur Read &amp; Analyze à votre compte GA. Pour plus d’informations, voir [ici](https://support.google.com/analytics/answer/2884495?hl=en).

1. Dans votre compte RTP. Accédez à **Paramètres du compte**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Sous **Paramètres du compte**, **Domaine** et **Analytics**.

1. Cliquez sur **Google Analytics**.

1. Activez les **Variables personnalisées** et **Événements** appropriés pour ajouter ces données de la HTTP aux Google Analytics.

1. Saisissez le numéro **Emplacement** pour envoyer les données de variable personnalisée (la valeur par défaut est 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Cliquez sur **Enregistrer**.

>[!NOTE]
>
>Pour envoyer des données de segment à GA, sous la [page Modifier le segment](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) de la plateforme RTP, cochez la case **Envoyer l’événement aux Google Analytics sur la correspondance de segment**.

## Configuration de rapports Google Analytics avec des données RTP {#setting-up-google-analytics-reports-with-rtp-data}

En Google Analytics, vous pouvez utiliser des tableaux de bord, la segmentation GA et la création de rapports pour afficher vos données RTP :

* [Les tableaux de bord](https://support.google.com/analytics/answer/1068216?hl=en) fournissent un aperçu des performances du site Web.
* Un segment GA est conçu pour filtrer les visiteurs dans l’interface GA et afficher le trafic par segment. Découvrez comment créer un segment [ici](https://support.google.com/analytics/answer/3124493?hl=en).
* Création de [rapports personnalisés](https://support.google.com/analytics/answer/1033013?hl=en) pour afficher et/ou configurer des emails planifiés Voir sous Personnalisation > Nouveau rapport personnalisé.
