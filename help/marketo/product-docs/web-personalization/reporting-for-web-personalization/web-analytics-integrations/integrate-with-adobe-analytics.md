---
unique-page-id: 2949160
description: Intégration à Adobe Analytics - Docs marketing - Documentation sur les produits
title: Intégration avec Adobe Analytics
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---


# Intégration avec Adobe Analytics {#integrate-with-adobe-analytics}

## Intro {#intro}

Analysez vos analyses Web du point de vue B2B en affichant les données de campagne de personnalisation en temps réel de votre entreprise, industrie et marketing dans votre compte Adobe Analytics.

Ce document permet l’intégration entre la personnalisation en temps réel du marketing (RTP) et l’Adobe Adobe Analytics. Les données de RTP vous permettent de détecter et d&#39;analyser les tendances de tous les segments et organisations du secteur qui visitent votre site et de mesurer l&#39;efficacité de vos campagnes RTP, en fournissant les informations et l&#39;analyse pour obtenir des résultats optimaux.

Pour ce faire, vous pouvez consulter des mesures telles que le nombre de nouveaux visiteurs par rapport au nombre de  de retour dans chaque segment, analyser les taux de clics sur les campagnes et découvrir les secteurs, les segments personnalisés et les campagnes en temps réel qui ont généré le plus de pistes de conversion. Tirez parti de cette capacité pour tirer le meilleur parti de votre compte RTP.

## Audience Analytics RTP {#rtp-audience-analytics}

Avec l’intégration RTP - AA, vous disposez d’une nouvelle dimension dans votre interface d’analyses Web. RTP améliore automatiquement vos tableaux de bord d&#39;analyses Web avec :

1. Données sur l’organisation et le secteur
1. Segments RTP personnalisés
1. Listes de compte nommées (marketing basé sur le compte)

Cela améliore vos données B2B et vous permet de vous concentrer sur les visiteurs pertinents en optimisant :

1. Canaux sortants
1. Contenu
1. Reciblage

## Rapport canal {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

Le tableau de bord RTP vous aide à comprendre la ventilation de vos visiteurs selon les secteurs verticaux et les segments RTP. Vous pouvez voir les performances de vos visiteurs en fonction de l’industrie et des différentes campagnes marketing (payantes, organiques, sociales) liées à cette industrie. Le tableau de bord fournit également un aperçu général des sections du site que vos visiteurs consultent en fonction de leur secteur d&#39;activité.

## Rapport comportemental {#behavioral-report}

Différents rapports de comportement peuvent être créés en Adobe Analytics en fonction des données des segments d’entreprise, d’industrie et de RTP. Ces rapports de flux visualisent le chemin suivi par les visiteurs d’une page ou d’un Événement à l’autre. Ce rapport peut vous aider à découvrir quel contenu maintient les visiteurs en contact avec votre site.

## Performances RTP {#rtp-performance}

Vue des impressions et conversions de campagne RTP sous Liens personnalisés dans Adobe Analytics.

Ce rapport sur les liens personnalisés montre les impressions et les conversions des campagnes sous le format de dénomination suivant :

* Impression ISegment : [Nom]de segment RTP, ICamcampaign : [Nom Campaign RTP]
* Segment de conversion : [Nom]de segment RTP, ICamcampaign : [Nom Campaign RTP]

![](assets/custom-links-report.png)

## Configuration en Adobe Analytics {#set-up-in-adobe-analytics}

L’intégration utilise l’API JavaScript que Adobe Analytics offre. Les variables de conversion personnalisées (eVar), les événements personnalisés (événement) et les variables de trafic sont utilisés dans l’intégration. Tous doivent être activés à partir d’un administrateur AA. Vous devez définir les variables de conversion, les événements personnalisés et les variables de trafic dans AAou vous ne pourrez pas afficher les données dans la suite même si vous les avez activées dans RTP.

Pour configurer ces variables dans AA, procédez comme suit :

1. Accédez aux outils **** d’administration dans votre compte AA.
1. Sélectionnez la suite **de** rapports à utiliser avec l’intégration.
1. Sous **Modifier les paramètres,** accédez à **Conversion** et sélectionnez ** Variables [de](http://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)conversion**.\
   Sélectionnez le numéro de la variable [de](http://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) conversion (nous vous recommandons de le faire) :

   1. 

      1. eVar n° 20 pour les conversions personnalisées du secteur
      1. eVar n° 21 pour les conversions personnalisées d&#39;organisation

         >[!NOTE]
         >
         >Si ces # sont pris, sélectionnez un autre nombre disponible. Alignez ce numéro avec le numéro d&#39;emplacement dans Paramètres du compte RTP.

      1. Modifier l&#39;état en * Activé*

         1. Remplacez Nom par **Secteur** et **Organisation**. (Voici comment il apparaîtra dans la suite de rapports.)

         1. Modifiez le champ Expire après en **Visite.**

1. Sous **Modifier les paramètres, **accédez à** Conversion **et sélectionnez ** [Événements](http://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)** de réussite.

1. Sélectionnez le numéro de Événement des Événements de réussite personnalisés (nous vous recommandons de le faire) :

   1. événement20 pour les campagnes RTP
   1. événement21 pour les segments RTP

      >[!NOTE]
      >
      >Si ces # sont pris, sélectionnez un autre nombre disponible. Alignez ce numéro avec le numéro d&#39;emplacement dans Paramètres du compte RTP.

   1. Modifiez les noms des deux événements en Campagnes **** RTP et Segments **** RTP. Il s’agit du nom qui apparaîtra dans la suite de rapports.

1. Sélectionnez le champ Type* *à **Compteur (sans sous-relations).**

1. Sous **Modifier les paramètres** , accédez à ** [Trafic](http://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable) **et sélectionnez ** Variables [de](http://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)** trafic.

   1. Sélectionnez la propriété # de la variable de trafic (nous vous recommandons) :

      1. Propriété n° 20 - Nom : Organisation des segments RTP
      1. Propriété n° 21 - Nom : Secteur des segments RTP
      1. Propriété n° 25 - Nom : Organisation Campaign
      1. Propriété n° 26 - Nom : Industrie Campaign RTP

         >[!NOTE]
         >
         >Si ces # sont pris, sélectionnez un autre nombre disponible. Aligner ce nombre avec le numéro d&#39;emplacement dans Paramètres du compte RTP)

      1. Modifiez les 4 noms de propriétés. Il s’agit du nom qui apparaîtra dans la suite de rapports.
   1. Sélectionner le champ activé à **activer**
   1. Sélectionner le champ Rapports Chemin à **activer**


## Configuration dans la personnalisation en temps réel de Marketo {#set-up-in-marketo-real-time-personalization-rtp}

1. Dans la plate-forme RTP, accédez à Paramètres **du** compte.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Sous Paramètres **du** compte, cliquez sur **Domaine**.
1. Sous **Analytics, cliquez sur** **Adobe Analytics**.
1. Activez **l&#39;option **les variables Conversion, Personnalisé et Trafic bascule.
1. Affectez les numéros **** d&#39;emplacement des variables de conversion, de Événement et de trafic pour qu&#39;ils correspondent aux numéros d&#39;emplacement créés dans AA.
1. Cliquez sur **ENREGISTRER**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Nos paramètres d&#39;emplacement recommandés sont
>
>**Variables de conversion**
>
>* Conversions personnalisées du secteur - Emplacement 20
>* Conversions personnalisées de l&#39;organisation - Emplacement 21

>
>
**Événements personnalisés**
>
>* Événement personnalisé Campaign - Emplacement 20
>* Événement personnalisé de segment - Emplacement 21

>
>
**Variables de trafic**
>
>* Variable de trafic d&#39;organisation de segment - Emplacement 20
>* Variable de trafic du secteur des segments - Emplacement 21
>* Variable de trafic d&#39;organisation Campaign - Emplacement 22
>* Variable de trafic du secteur Campaign - Emplacement 23

>
>
**Assurez-vous que ces numéros d’emplacements correspondent aux numéros de variables et de événements créés dans AA.**

## Rapports {#reports}

Créez des rapports SiteAdobe Analytics améliorés en fonction des noms d’entreprise, des secteurs et des segments RTP et des données des campagnes en temps réel.

Voici quelques exemples de rapports et de tableaux de bord personnalisés dans AA :

* Performances par secteur ou segment défini (listes nommées basées sur un compte)
* Ventilation par secteur et performance par IPC
* Pages vues par organisation
* Performances du canal marketing en fonction de l’organisation, du secteur, des segments

**Exemples de rapports**

**Rapport Principales industries**

** ![](assets/top-industries-report.png)

**

**Rapport Organisations**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Création du Tableau de bord RTP**

Créez un [nouveau tableau de bord](http://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), appelé Tableau de bord **** RTP. Ce tableau de bord vous aidera à comprendre la ventilation de vos visiteurs en fonction des secteurs verticaux et des segments RTP.

1. Cliquez sur **Tableau de bord,** cliquez sur** Ajouter Tableau de bord**

1. Nommer le Tableau de bord **RTP du Tableau de bord**
1. Sélectionner la taille **du** tableau de bord 3 x 2, 2 x 2
1. Créez le [petit rapport](http://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) et ajoutez du [contenu au tableau de bord.](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard)

Ajouter le petit rapport Industries au Tableau de bord

1. Accédez à Conversions **** personnalisées, cliquez sur **Secteur**

1. Configuration d&#39;un graphique en **secteurs**
1. Cliquez sur le **Tableau de bord**, ajoutez le **petit rapport.**

1. Nommer les **principales industries du rapport**
1. Placer dans le Tableau de bord **RTP Tableau de bord**
1. Créer **nouveau**.

Ajouter le petit rapport Segments au Tableau de bord

1. Accédez à **Mesures du site, **Cliquez sur Événements **personnalisés, Segments.**

1. Configuration d’un graphique sur une barre **verticale**
1. Cliquez sur le **Tableau de bord**, ajoutez le **petit rapport.**

1. Nommer les **principaux segments du rapport**
1. Placer dans le Tableau de bord **RTP Tableau de bord**
1. Créer **nouveau.**

Vos petits rapports s’afficheront dans le tableau de bord.

## Impressions de vue et clics (conversions) dans Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Cliquez sur Liens personnalisés.

   ![](assets/sitecatalyst1-1.png)

1. Recherchez Impressions sur le segment de vue et Noms Campaign représentant le nombre d’impressions de la campagne.\
   ![](assets/sitecatalyst1.png)

1. Recherchez Conversion en segment de vue et noms Campaign représentant le nombre de clics pour la campagne.

   ![](assets/sitecatalyst2.png)

