---
unique-page-id: 2949158
description: Intégration de RTP avec des Google Analytics - Docs marketing - Documentation du produit
title: Intégration de RTP avec des Google Analytics
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---


# Intégrer RTP aux Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics est désormais la norme d’exploitation et toutes les propriétés de Google ont été mises à niveau vers Universal Analytics.
>
>Cet article explique comment utiliser l’ancien Google Standard Analytics, mais nous vous recommandons de passer à Universal Analytics.
>
>Si vous n’utilisez pas déjà le code de suivi [analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), Google vous recommande vivement de remarquer votre site pour l’utiliser. Les éléments suivants sont déconseillés par Google :
>
>* ga.js
>* urchin.js
>* Extraits de code WAP/côté serveur
>* YT / MO
>* Variables personnalisées
>* Variables définies par l’utilisateur

>
>
Découvrez comment intégrer la [personnalisation Web à Universal Analytics](integrate-rtp-with-google-universal-analytics.md)

## Introduction {#introduction}

Analysez vos analyses Web sous un nouvel angle en utilisant le flux de données direct de la personnalisation en temps réel (RTP) vers votre compte de Google Analytics (GA). Mesurez vos visites Web en GA en fonction des organisations, des secteurs et des campagnes RTP. Les mesures de vue, telles que les types de secteurs ou les segments RTP dans GA et la manière dont ils effectuent et génèrent des pistes selon différentes sources de trafic (sociales, payées, organiques), l&#39;analyse des taux de clics publicitaires sur les campagnes et la mesure de l&#39;impact des campagnes de personnalisation sur votre site Web. Tirez parti de cette possibilité pour tirer le meilleur parti de votre compte RTP

**Audience Analytics RTP**

Avec l’intégration, vous avez une nouvelle dimension dans votre compte GA. RTP améliore automatiquement vos tableaux de bord avec :

1. Organisations et industries
1. Segments personnalisés dans RTP
1. Listes marketing basées sur le compte

Concentrez-vous sur vos prospects B2B clés. Analyser les canaux par secteurs et segments ciblés.

## Rapport canal {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

Le Tableau de bord RTP B2B vous aide à comprendre la ventilation de vos visiteurs selon les secteurs verticaux et la segmentation RTP. Vous pouvez voir les performances de vos visiteurs en fonction du secteur financier et de différentes campagnes marketing (payantes, organiques, sociales). Le tableau de bord fournit également un aperçu général des performances de vos segments RTP et analyse les principales organisations qui visitent votre site.

## Flux comportemental {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

Le rapport Flux de comportement (voir l’image) visualise le chemin parcouru par les visiteurs d’une page ou d’un Événement à l’autre. L&#39;exemple d&#39;image montre le chemin emprunté par tous les visiteurs du secteur financier. Ce rapport peut vous aider à découvrir quel contenu maintient les visiteurs en contact avec votre site.

## Performances RTP {#rtp-performance}

Mesurez vos campagnes RTP et corrélez-les à la moyenne globale de votre site. Découvrez comment ces campagnes affectent les mesures de votre site Web et utilisez ces données pour concentrer vos efforts de personnalisation sur les cibles appropriées. Générez des rapports personnalisés pour mieux comprendre les performances de vos campagnes de personnalisation.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Configuration de RTP avec des Google Analytics {#setting-up-rtp-with-google-analytics}

1. Ajoutez le courrier électronique [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#0674727628616734466b67746d6372692865696b), en tant qu’utilisateur de lecture et d’analyse dans votre compte GA. Pour plus de détails, voir [ici](https://support.google.com/analytics/answer/2884495?hl=en).
1. Dans votre compte RTP. Accédez à **Paramètres du compte**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Sous **Paramètres du compte**, **Domaine** et **Analyses**
1. Cliquez sur** Google Analytics.**
1. Activez les **variables personnalisées** et **Événements** appropriés pour ajouter ces données de RTP aux Google Analytics.
1. Entrez le **nombre d&#39;emplacements** pour envoyer des données de variable personnalisée (la valeur par défaut est 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

Cliquez sur **SAVE**.

>[!NOTE]
>
>Pour envoyer des données de segment à GA, sous la [page Modifier le segment](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) de la plate-forme RTP, cochez la case **Envoyer le Événement aux Google Analytics sur la correspondance de segment**.

## Configuration de rapports Google Analytics avec des données RTP {#setting-up-google-analytics-reports-with-rtp-data}

En Google Analytics, vous pouvez utiliser les tableaux de bord, la segmentation GA et le rapports pour vue de vos données RTP :

* [Les ](https://support.google.com/analytics/answer/1068216?hl=en) tableaux de bord donnent un aperçu des performances du site Web.
* Un segment GA est destiné à filtrer les visiteurs dans l’interface GA et à vue du trafic par segment. Voir comment créer un segment [ici](https://support.google.com/analytics/answer/3124493?hl=en).
* Création de [rapports personnalisés](https://support.google.com/analytics/answer/1033013?hl=en) à la vue et/ou configuration de courriers électroniques planifiés. Voir sous Personnalisation > Nouveau rapport personnalisé.
