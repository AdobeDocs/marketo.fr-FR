---
unique-page-id: 2949158
description: Intégration du RTP à Google Analytics - Documentation de Marketo - Documentation du produit
title: Intégrer RTP à Google Analytics
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 2%

---

# Intégrer RTP à Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics est désormais la norme de fonctionnement et toutes les propriétés de Google ont été mises à niveau vers Universal Analytics.
>
>Cet article explique comment utiliser l’ancienne version de Google Standard Analytics, mais nous vous recommandons de passer à Universal Analytics.
>
>Si vous n’utilisez pas déjà le code de suivi [analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), Google vous recommande vivement de rebaliser votre site pour l’utiliser. Google rend obsolètes les éléments suivants :
>
>* ga.js
>* urchin.js
>* Fragments de code WAP/côté serveur
>* YT/MO
>* Variables personnalisées
>* Variables définies par l’utilisateur
>
>Découvrez comment intégrer [Web Personalization à Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Introduction {#introduction}

Analysez vos analyses web sous un nouvel angle à l’aide du flux de données direct de Marketo Real-Time Personalization (RTP) vers votre compte Google Analytics (GA). Mesurez vos visites web en GA en fonction des organisations, des secteurs d&#39;activité et des campagnes RTP. Affichez des mesures telles que les types d’industries ou les segments RTP dans GA et la manière dont ils exécutent et génèrent des pistes en fonction de différentes sources de trafic (social, payant, organique), analysez les taux de clics sur les campagnes et mesurez l’impact des campagnes de personnalisation sur votre site web. Tirez parti de cette fonctionnalité pour tirer le meilleur parti de votre compte RTP

**RTP AUDIENCE ANALYTICS**

Grâce à l’intégration d’, vous disposez d’une nouvelle dimension dans votre compte GA. RTP améliore automatiquement vos tableaux de bord avec :

1. Organisations et secteurs
1. Segments personnalisés dans RTP
1. Listes Account-Based Marketing

Concentrez-vous sur vos prospects B2B clés. Analysez les canaux par secteurs et segments ciblés.

## Rapport de canal {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

Le tableau de bord RTP B2B vous aide à comprendre la répartition de vos visiteurs en fonction des verticaux et de la segmentation RTP. Vous pouvez voir les performances de vos visiteurs en fonction du secteur de la finance et selon différentes campagnes marketing (payantes, organiques, sociales). Le tableau de bord fournit également un aperçu général des performances de vos segments RTP et des analyses vers le bas pour afficher les principales organisations qui visitent votre site.

## Flux comportemental {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

Le rapport Flux de comportement (voir image) visualise le chemin parcouru par les visiteurs et visiteuses d’une page ou d’un événement à l’autre. L’exemple d’image présente le chemin de tous les visiteurs du secteur financier. Ce rapport peut vous aider à découvrir le contenu qui maintient l’engagement des visiteurs et visiteuses sur votre site.

## Performances RTP {#rtp-performance}

Mesurez vos campagnes RTP et corrélez-les avec la moyenne globale de votre site. Découvrez comment ces campagnes affectent les mesures de votre site web et utilisez ces données pour concentrer vos efforts de personnalisation sur les cibles appropriées. Générez des rapports personnalisés pour mieux comprendre les performances de vos campagnes de personnalisation.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Configuration du RTP avec Google Analytics {#setting-up-rtp-with-google-analytics}

1. Ajoutez l’<rtp.ga2@gmail.com> e-mail en tant qu’utilisateur Read &amp; Analyze à votre compte GA. Pour plus d’informations, rendez-vous [ici](https://support.google.com/analytics/answer/2884495?hl=en).

1. Dans votre compte RTP. Accédez à **[!UICONTROL Paramètres du compte]**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Sous **[!UICONTROL Paramètres du compte]**, **[!UICONTROL Domaine]** et **[!UICONTROL Analytics]**.

1. Cliquez sur **Google Analytics**.

1. Activez les **Variables personnalisées** et **Événements** appropriées pour ajouter ces données du RTP au Google Analytics.

1. Saisissez le nombre **Emplacement** pour envoyer des données de variable personnalisées (1,2 par défaut).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

>[!NOTE]
>
>Pour envoyer des données de segment à GA, sous la page [[!UICONTROL Modifier le segment] ](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) de la plateforme RTP, cochez la case **[!UICONTROL Envoyer l’événement à Google Analytics lors de la correspondance de segments]**.

## Configuration de rapports Google Analytics avec des données RTP {#setting-up-google-analytics-reports-with-rtp-data}

Dans Google Analytics, vous pouvez utiliser des tableaux de bord, la segmentation GA et les rapports pour afficher vos données RTP :

* [Tableaux de bord](https://support.google.com/analytics/answer/1068216?hl=en) donnent un aperçu des performances du site web.
* Un segment GA est destiné à filtrer les visiteurs dans l’interface GA et à afficher le trafic par segment. Découvrez comment créer un segment [ici](https://support.google.com/analytics/answer/3124493?hl=en).
* Création de [rapports personnalisés](https://support.google.com/analytics/answer/1033013?hl=en) pour afficher et/ou configurer des e-mails planifiés. Voir sous **[!UICONTROL Personnalisation]** > **[!UICONTROL Nouveau rapport personnalisé]**.
