---
unique-page-id: 2949160
description: Intégration à Adobe Analytics - Marketo Docs - Documentation du produit
title: Intégration à Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# Intégration à Adobe Analytics {#integrate-with-adobe-analytics}

## Introduction {#intro}

Analysez vos analyses web du point de vue B2B en affichant les données de campagne de personnalisation en temps réel de l’organisation, du secteur et de Marketo dans votre compte Adobe Analytics.

Ce document permet l’intégration entre la personnalisation en temps réel de Marketo et Adobe Adobe Analytics. Les données issues de la méthode RTP vous permettent de détecter et d’analyser les tendances de tous les segments du secteur et organisations qui visitent votre site, ainsi que de mesurer l’efficacité de vos campagnes RTP, en fournissant des informations et des analyses afin d’obtenir des résultats optimaux.

Pour ce faire, vous pouvez consulter des mesures telles que le nombre de visiteurs nouveaux par rapport aux visiteurs récurrents dans chaque segment, analyser les taux de clics sur les campagnes et découvrir les secteurs, les segments personnalisés et les campagnes en temps réel qui ont généré les meilleures pistes de conversion. Tirez parti de cette fonctionnalité pour tirer le meilleur parti de votre compte RTP.

## Audience Analytics RTP {#rtp-audience-analytics}

Avec l’intégration RTP - AA, vous disposez d’une nouvelle dimension dans votre interface d’analyse web. La technologie RTP améliore automatiquement vos tableaux de bord Web Analytics avec :

1. Données de l’organisation et du secteur
1. Segments RTP personnalisés
1. Listes de comptes nommés (Account-Based Marketing)

Cela améliore vos données B2B et vous permet de vous concentrer sur les visiteurs pertinents en optimisant :

1. Canaux sortants
1. Contenu
1. Reciblage

## Rapport Canal {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

Le tableau de bord RTP vous aide à comprendre la ventilation de vos visiteurs selon les segments verticaux et RTP. Vous pouvez afficher les performances de vos visiteurs en fonction du secteur et de différentes campagnes marketing (payantes, organiques, sociales) liées à ce secteur. Le tableau de bord fournit également un aperçu général des sections du site que vos visiteurs consultent en fonction de leur type de secteur d’activité.

## Rapport comportemental {#behavioral-report}

Différents rapports de comportement peuvent être créés dans Adobe Analytics en fonction des données de segment d’organisation, de secteur et de HTTP. Ces rapports de flux visualisent le chemin que les visiteurs empruntent d’une page ou d’un événement à l’autre. Ce rapport peut vous aider à découvrir le contenu qui maintient les visiteurs en contact avec votre site.

## Performances RTP {#rtp-performance}

Affichez les impressions et conversions de campagnes RTP sous Liens personnalisés dans Adobe Analytics.

Ce rapport sur les liens personnalisés affiche les impressions et les conversions des campagnes sous le format de dénomination suivant :

* Impression ISegment : [Nom du segment RTP], ICamcampaign : [Nom de la campagne HTTP]
* Conversion ISegment : [Nom du segment RTP], ICamcampaign : [Nom de la campagne HTTP]

![](assets/custom-links-report.png)

## Configuration dans Adobe Analytics {#set-up-in-adobe-analytics}

L’intégration utilise l’API JavaScript proposée par Adobe Analytics. Les variables de conversion personnalisées (eVar), les événements personnalisés (événement) et les variables de trafic sont utilisés dans l’intégration. Tous doivent être activés dans un administrateur AA. Vous devez définir les variables de conversion, les événements personnalisés et les variables de trafic dans AA. Sinon, vous ne pourrez pas afficher les données dans la suite même si vous l’avez activée dans la HTTP.

Procédez comme suit pour configurer ces variables dans AA :

1. Accédez à **Outils d’administration** dans votre compte AA.
1. Sélectionnez la **Suite de rapports** à utiliser avec l’intégration.
1. Sous **Modifier les paramètres**, accédez à **Conversion** et sélectionnez **[Variables de conversion](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Sélectionnez la [Variable de conversion](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) number (nous recommandons) :

   1. Evar n° 20 pour les conversions personnalisées du secteur
   1. Evar n° 21 pour les conversions personnalisées de l’organisation

   >[!NOTE]
   >
   >Si ces # sont utilisés, sélectionnez un autre nombre disponible. Alignez ce nombre sur le numéro d’emplacement dans les paramètres du compte RTP.

   1. Modifier l’état en _Activé_.

      1. Modifier le nom en **Secteur industriel** et **Organisation**. (C’est ainsi qu’il apparaîtra dans la suite de rapports.)

      1. Remplacez le champ Expire après par **Visite**.

1. Sous **Modifier les paramètres** accéder à **Conversion** et sélectionnez **[Événements de succès](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Sélectionnez le numéro Événement d’événement de succès personnalisé (nous vous recommandons) :

      1. event20 pour les campagnes RTP
      1. event21 pour les segments RTP

      >[!NOTE]
      >
      >Si ces # sont utilisés, sélectionnez un autre nombre disponible. Alignez ce nombre sur le numéro d’emplacement dans les paramètres du compte RTP.

      1. Remplacez les deux noms d’événements par **Campagnes RTP** et **Segments RTP**. Il s’agit du nom qui apparaîtra dans la suite de rapports.

   1. Sélectionnez le champ Type à définir **Compteur (sans sous-relations)**

1. Sous **Modifier les paramètres** accéder à **[Trafic](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** et sélectionnez **[Variables de trafic](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Sélectionnez le numéro de propriété de la variable de trafic (nous vous recommandons de le faire) :

      1. Propriété n° 20 - Nom : Organisation du segment RTP
      1. Propriété n° 21 - Nom : Secteur du segment RTP
      1. Propriété n° 25 - Nom : Organisation de campagne
      1. Propriété n° 26 - Nom : Secteur des campagnes RTP

      >[!NOTE]
      >
      >Si ces # sont utilisés, sélectionnez un autre nombre disponible. Aligner ce nombre avec le numéro d’emplacement dans les paramètres du compte RTP)

      1. Modifiez les quatre noms de propriétés. Il s’agit du nom qui apparaîtra dans la suite de rapports.

   1. Sélectionnez Champ activé pour **Activé**.

   1. Sélectionnez le champ Rapports de chemins pour **Activé**.

## Configuration dans la personnalisation en temps réel de Marketo (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. Dans la plateforme RTP, accédez à **Paramètres du compte**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Sous **Paramètres du compte**, cliquez sur **Domaine**.
1. Sous **Analytics, cliquez sur** **Adobe Analytics**.
1. Tourner **Activé** Les bascules des variables Conversion, Personnalisé et Trafic .
1. Attribution des variables de conversion, d’événement et de trafic **numéros d’emplacements** pour correspondre aux numéros d’emplacements créés dans AA
1. Cliquez sur **Enregistrer**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Nos paramètres d’emplacement recommandés sont les suivants :
>
>**Variables de conversion**
>
>* Conversions personnalisées du secteur - Emplacement 20
>* Conversions personnalisées de l’organisation - Emplacement 21
>
>**Événements personnalisés**
>
>* Événement personnalisé de campagne - Emplacement 20
>* Événement personnalisé de segment - Emplacement 21
>
>**Variables de trafic**
>
>* Variable de trafic de l’organisation de segments - Emplacement 20
>* Variable de trafic du secteur des segments - Emplacement 21
>* Variable de trafic de l’organisation Campaign - Emplacement 22
>* Variable de trafic du secteur Campaign - Emplacement 23
>
>**Assurez-vous que ces numéros d’emplacements correspondent aux numéros de variables et d’événements créés dans AA.**

## Rapports   {#reports}

Créez des rapports SiteAdobe Analytics améliorés en fonction des noms d’organisation, des secteurs et des segments de HTTP et des données de campagnes en temps réel.

Voici quelques exemples de rapports et de tableaux de bord personnalisés dans AA :

* Performances par secteur ou segment défini (listes nommées basées sur un compte)
* Répartition du secteur par IPC
* Pages vues par organisation
* Performances du canal marketing en fonction de l’organisation, du secteur industriel et des segments

**-Exemples de rapports-**

**Rapport Principaux secteurs**

![](assets/top-industries-report.png)

**Rapport d’entreprise**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Création du tableau de bord RTP**

Créez un [nouveau tableau de bord](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), appelé **Tableau de bord RTP**. Ce tableau de bord vous aidera à comprendre la ventilation de vos visiteurs en fonction des segments verticaux et RTP.

1. Cliquez sur **Tableau de bord,** click **Ajouter un tableau de bord**.

1. Nommer le tableau de bord **Tableau de bord RTP**.

1. Sélectionnez la **taille du tableau de bord** 3 x 2, 2 x 2.

1. Créez le [petit rapport](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) et ajouter [contenu du tableau de bord](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Ajout du mini-rapport Industries au tableau de bord

1. Accédez à **Conversions personnalisées**, cliquez sur **Secteur industriel**.

1. Configuration d’un graphique sur **Graphique circulaire**.

1. Cliquez sur **Tableau de bord**, ajoutez **Petit rapport**.

1. Nommer le rapport **Principaux secteurs**.

1. Placer sur le tableau de bord **Tableau de bord RTP**.

1. Créer **Nouveau**.

Ajout du mini-rapport Segments au tableau de bord

1. Accédez à **Mesures du site**. Cliquez sur **Événements personnalisés**, **Segments**.

1. Configuration d’un graphique sur **Barre verticale**.

1. Cliquez sur **Tableau de bord**, ajoutez **Petit rapport**.

1. Nommer le rapport **Principaux segments**.

1. Placer sur le tableau de bord **Tableau de bord RTP**.

1. Créer **Nouveau**.

Vos mini-rapports s’affichent dans le tableau de bord.

## Affichage des impressions et des clics (conversions) dans Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Cliquez sur **Liens personnalisés**.

   ![](assets/sitecatalyst1-1.png)

1. Recherchez Impressions pour afficher les noms des segments et des campagnes représentant le nombre d’impressions de la campagne.\
   ![](assets/sitecatalyst1.png)

1. Recherchez Conversion pour afficher les noms des segments et des campagnes représentant le nombre de clics pour la campagne.

   ![](assets/sitecatalyst2.png)
