---
unique-page-id: 2949160
description: Intégration à Adobe Analytics - Documentation de Marketo - Documentation du produit
title: Intégrer à Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 1%

---

# Intégrer à Adobe Analytics {#integrate-with-adobe-analytics}

## Introduction {#intro}

Analysez vos analyses web du point de vue B2B en affichant les données des campagnes d’organisation, de secteur et de [!DNL Marketo Real-Time Personalization] (RTP) dans votre compte Adobe Analytics.

Ce document permet l’intégration entre [!DNL Marketo Real-Time Personalization] (RTP) et Adobe Adobe Analytics. Les données de RTP vous permettront de détecter et d&#39;analyser les tendances dans tous les segments de l&#39;industrie et les organisations visitant votre site et de mesurer l&#39;efficacité de vos campagnes RTP, fournissant les informations et l&#39;analyse pour obtenir des résultats optimaux.

Pour ce faire, vous pouvez examiner des mesures telles que le nombre de visiteurs nouveaux par rapport au nombre de visiteurs récurrents dans chaque segment, analyser les taux de clics sur les campagnes et découvrir quels secteurs d’activité, segments personnalisés et campagnes en temps réel ont généré les meilleures pistes de conversion. Tirez parti de cette fonctionnalité pour tirer le meilleur parti de votre compte RTP.

## AUDIENCE ANALYTICS RTP {#rtp-audience-analytics}

Avec l’intégration RTP - AA, vous disposez d’une nouvelle dimension dans votre interface Web Analytics. RTP améliore automatiquement vos tableaux de bord Web Analytics avec :

1. Données sur l’organisation et le secteur
1. Segments RTP personnalisés
1. Listes des comptes nommés (Account-Based Marketing)

Cela améliore vos données B2B et vous permet de vous concentrer sur les visiteurs appropriés en optimisant :

1. Canaux sortants
1. Contenu
1. Reciblage

## Rapport de canal {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

Le tableau de bord RTP vous aide à comprendre la répartition de vos visiteurs en fonction des verticaux et des segments RTP. Vous pouvez afficher les performances de vos visiteurs et visiteuses en fonction du secteur et des différentes campagnes marketing (payantes, organiques, sociales) liées à ce secteur. Le tableau de bord fournit également une vue d’ensemble des sections du site que vos visiteurs consultent en fonction de leur type de secteur d’activité.

## Rapport comportemental {#behavioral-report}

Différents rapports de comportement peuvent être créés dans Adobe Analytics en fonction des données de segment de l’organisation, du secteur et du RTP. Ces rapports de flux visualisent le chemin que les visiteurs empruntent d’une page ou d’un événement à l’autre. Ce rapport peut vous aider à découvrir le contenu qui maintient l’engagement des visiteurs et visiteuses sur votre site.

## Performances RTP {#rtp-performance}

Affichez les impressions et les conversions de campagnes RTP sous Liens personnalisés dans Adobe Analytics.

Ce rapport Lien personnalisé affiche les impressions et les conversions des campagnes sous le format de dénomination suivant :

* Impression ISegment : [Nom du segment RTP], ICampaign : [Nom de la campagne RTP]
* Conversion ISegment : [Nom du segment RTP], ICampaign : [Nom de la campagne RTP]

![](assets/custom-links-report.png)

## Configuration dans Adobe Analytics {#set-up-in-adobe-analytics}

L’intégration utilise l’API JavaScript proposée par Adobe Analytics. Les variables de conversion personnalisées (eVar), les événements personnalisés (événement) et les variables de trafic sont utilisés dans l’intégration. Tous doivent être activés à partir de l’administrateur AA. Vous devez définir les variables de conversion, les événements personnalisés et les variables de trafic dans AA. Sinon, vous ne pourrez pas voir les données de la suite même si vous l’avez activée dans RTP.

Pour configurer ces variables dans AA, procédez comme suit :

1. Accédez à **[!UICONTROL Outils d’administration]** dans votre compte AA.
1. Sélectionnez la **[!UICONTROL Suite de rapports]** à utiliser avec l’intégration.
1. Sous **[!UICONTROL Modifier les paramètres]**, accédez à **[!UICONTROL Conversion]** et sélectionnez **[[!UICONTROL Variables de conversion]](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.
Sélectionnez le nombre [Variable de conversion](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) (recommandé) :

   1. Evar # 20 pour les conversions personnalisées du secteur
   1. Evar # 21 pour les conversions personnalisées d’organisation

   >[!NOTE]
   >
   >Si ces # sont pris, sélectionnez un autre numéro disponible. Alignez ce numéro sur le numéro de slot dans les paramètres du compte RTP.

   1. Modifiez le statut en _[!UICONTROL Enabled_].

      1. Remplacez le nom par **Secteur** et **Organisation**. (Tel est son aspect dans la suite de rapports.)

      1. Remplacez le champ Expire après par **[!UICONTROL Visite]**.

1. Sous **[!UICONTROL Modifier les paramètres]** accédez à **[!UICONTROL Conversion]** et sélectionnez **[[!UICONTROL Événements de succès]](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Sélectionnez le numéro d’événement de succès personnalisé (nous vous recommandons) :

      1. event20 pour les campagnes RTP
      1. event21 pour les segments RTP ;

      >[!NOTE]
      >
      >Si ces # sont pris, sélectionnez un autre numéro disponible. Alignez ce numéro sur le numéro de slot dans les paramètres du compte RTP.

      1. Remplacez les noms des deux événements par **Campagnes RTP** et **Segments RTP**. Il s’agit du nom qui apparaîtra dans la suite de rapports.

   1. Sélectionnez le champ Type à **Compteur (pas de sous-relations)**

1. Sous **[!UICONTROL Modifier les paramètres]** accédez à **[Trafic](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** et sélectionnez **[Variables de trafic](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Sélectionnez la propriété de variable de trafic # (nous vous recommandons) :

      1. Propriété # 20 - Nom : Organisation du segment RTP
      1. Propriété # 21 - Nom : RTP Segment Industry
      1. Propriété # 25 - Nom : Campaign Organization
      1. Propriété # 26 - Nom : RTP Campaign Industry

      >[!NOTE]
      >
      >Si ces # sont pris, sélectionnez un autre numéro disponible. Aligner ce nombre sur le numéro de slot dans les paramètres du compte RTP)

      1. Modifiez les 4 noms de propriété. Il s’agit du nom qui apparaîtra dans la suite de rapports.

   1. Sélectionnez [!UICONTROL Activé] pour **[!UICONTROL Activé]**.

   1. Sélectionnez le champ [!UICONTROL Rapports de chemin] pour **[!UICONTROL Activé]**.

## Configuration dans [!DNL Marketo Real-Time Personalization] (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. Dans la plateforme RTP, accédez à **[!UICONTROL Paramètres du compte]**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Sous **[!UICONTROL Paramètres du compte]**, cliquez sur **[!UICONTROL Domaine]**.
1. Sous **[!UICONTROL Analytics]**, cliquez sur **Adobe Analytics**.
1. Activez **[!UICONTROL Activer]** le bouton (bascule) des variables Conversion, Personnalisé et Trafic .
1. Attribuez les variables de conversion, d’événement et de trafic **numéros de slot** pour correspondre aux numéros de slot créés dans AA
1. Cliquez sur **[!UICONTROL Enregistrer]**

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Nos paramètres d&#39;emplacement recommandés sont les suivants :
>
>**Variables de conversion**
>
>* [!UICONTROL Conversions personnalisées du secteur] - Emplacement 20
>* [!UICONTROL Conversions personnalisées d’organisation] - Emplacement 21
>
>**Événements personnalisés**
>
>* [!UICONTROL Événement personnalisé de campagne] - Emplacement 20
>* [!UICONTROL Événement personnalisé de segment] - Emplacement 21
>
>**Variables de trafic**
>
>* [!UICONTROL Variable de trafic d’organisation de segment] - Emplacement 20
>* [!UICONTROL Variable de trafic du secteur des segments] - Emplacement 21
>* [!UICONTROL Variable De Trafic De L’Organisation De Campagne] - Emplacement 22
>* [!UICONTROL Variable De Trafic Du Secteur Campaign] - Emplacement 23
>
>**Assurez-vous que ces numéros d’emplacement correspondent aux variables et aux numéros d’événements créés dans AA.**

## Rapports {#reports}

Créez des rapports SiteAdobe Analytics améliorés en fonction des noms d’organisation, des secteurs d’activité, des segments RTP et des données de campagnes en temps réel.

Voici quelques exemples de rapports et de tableaux de bord personnalisés dans AA :

* Performances par secteur ou par segment défini (listes nommées basées sur les comptes)
* Répartition du secteur par performance des KPI
* Pages vues par organisation
* Performances du canal marketing selon l’organisation, le secteur et les segments

**-Report Examples-**

**Rapport Principaux secteurs**

![](assets/top-industries-report.png)

**Rapport sur les organisations**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Création du tableau de bord RTP**

Créez un [tableau de bord](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html) appelé **tableau de bord RTP**. Ce tableau de bord vous aidera à comprendre la répartition de vos visiteurs en fonction des secteurs verticaux et des segments RTP.

1. Cliquez sur **[!UICONTROL Tableau de bord],** sur **[!UICONTROL Ajouter un tableau de bord]**.

1. Nommez le tableau de bord **RTP Dashboard**.

1. Sélectionnez la **taille du tableau de bord** 3 x 2, 2 x 2.

1. Créez le [petit rapport](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) et ajoutez le [contenu au tableau de bord](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Ajout du rapport Industries au tableau de bord

1. Accédez à **[!UICONTROL Conversions personnalisées]**, cliquez sur **[!UICONTROL Secteur]**.

1. Configurez le graphique en **graphique en secteurs**.

1. Cliquez sur **[!UICONTROL Tableau de bord]**, ajoutez **[!UICONTROL Petit rapport]**.

1. Nommez le rapport **Principaux secteurs**.

1. Placer dans le tableau de bord **tableau de bord RTP**.

1. Créer **Nouveau**.

Ajout du petit rapport Segments au tableau de bord

1. Accédez à **[!UICONTROL Mesures du site]**. Cliquez sur **[!UICONTROL Événements personnalisés]**, **[!UICONTROL Segments]**.

1. Configurez le graphique en **Barre verticale**.

1. Cliquez sur **[!UICONTROL Tableau de bord]**, ajoutez **[!UICONTROL Petit rapport]**.

1. Nommez le rapport **Segments principaux**.

1. Placer dans le tableau de bord **tableau de bord RTP**.

1. Créer **Nouveau**.

Vos petits rapports s’affichent dans le tableau de bord.

## Affichage des impressions et des clics (conversions) dans Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Cliquez sur **[!UICONTROL Personnaliser] Liens**.

   ![](assets/sitecatalyst1-1.png)

1. Recherchez Impressions pour afficher les noms de segment et de campagne représentant le nombre d’impressions de la campagne.
   ![](assets/sitecatalyst1.png)

1. Recherchez Conversion pour afficher les noms de segment et de campagne représentant le nombre de clics pour la campagne.

   ![](assets/sitecatalyst2.png)
