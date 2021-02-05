---
unique-page-id: 7504238
description: Tableaux de bord RTP personnalisés dans Google Universal Analytics - Docs marketing - Documentation sur les produits
title: Tableaux de bord RTP personnalisés dans Google Universal Analytics
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 0%

---


# Tableaux de bord RTP personnalisés dans Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Intégration de RTP à Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)

Ce billet explique comment configurer des tableaux de bord RTP dans Google Universal Analytics (GUA).  Les données envoyées de RTP à GUA peuvent être configurées sous la forme de deux tableaux de bord personnalisés distincts appelés :

* RTP B2B
* Engagement RTP

## Configuration d’un Tableau de bord personnalisé {#setting-up-a-custom-dashboard}

1. Connectez-vous aux Google Analytics. Cliquez sur **Rapports **dans le menu supérieur. Cliquez sur **Tableaux de bord **et **+Nouveau Tableau de bord personnalisé.**

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Sélectionnez **Canevas vierge**, ajoutez un **nom du Tableau de bord** et cliquez sur **Créer un Tableau de bord**.

1. Cliquez sur **Ajouter le widget** pour créer un widget.\
   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Tableau de bord RTP B2B {#rtp-b-b-dashboard}

Ce tableau de bord permet aux utilisateurs d&#39;analyser les performances de leur site Web du point de vue B2B.

Il fournit des informations telles que la source des visites et le comportement sur site par secteur d’activité, les recettes, la taille, les listes basées sur le compte et les segments de cible.

Le tableau de bord se compose de 3 colonnes.

* Source du trafic
* Segmentation
* Zoom avant sur les microrégraphies

1. Créez un nouveau tableau de bord appelé **RTP B2B Tableau de bord **et définissez les widgets suivants :

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Colonne 1 - Sources de trafic 
    </div></th> 
   <th> 
    <div> <strong>Colonne 2 - Segmentation</strong> 
    </div></th> 
   <th> 
    <div> <strong>Colonne 3 - Analyse micrographique</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : Sessions par segment et Canal</li> 
     <li>Type de widget : Barre<br></li> 
     <li>Créez un graphique à barres présentant les éléments suivants : Session</li> 
     <li>Regroupé par : Libellé du événement</li> 
     <li>Pivot par : Regroupement de Canaux par défaut</li> 
     <li>Filtre : <br>Afficher uniquement | Catégorie de Événement (contenant) RTP-Segments</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : Nombre d'utilisateurs segmentés RTP</li> 
     <li>Type : 2.1 Mesure</li> 
     <li>Afficher la mesure suivante : Utilisateurs<br></li> 
     <li>Filtre : <br>Afficher uniquement | Catégorie de Événement (contenant) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : Sessions par secteur</li> 
     <li>Type : Diagramme<br></li> 
     <li>Créez un graphique circulaire présentant : Sessions</li> 
     <li>Regroupé par : RTP-Industrie</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nom : Sessions par secteur et Canaux</strong></li> 
     <li><strong>Type de widget : Barre</strong></li> 
     <li><strong>Créez un graphique à barres présentant les éléments suivants : Session</strong></li> 
     <li><strong>Regroupé par : RTP-Industrie</strong></li> 
     <li><strong>Pivot par : Regroupement de Canaux par défaut</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nom : Sessions segmentées par pays</strong></li> 
     <li><strong>Type : Geomap</strong></li> 
     <li><strong>Traiter la mesure sélectionnée : Pays | Sessions</strong></li> 
     <li><strong>Sélectionnez une région : Le monde</strong></li> 
     <li><strong>Filtre : Afficher uniquement | Catégorie de Événement (contenant) RTP-Segments</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nom : Sessions par Catégorie RTP</strong></li> 
     <li><strong>Type : Diagramme</strong></li> 
     <li><strong>Créez un graphique circulaire présentant : Sessions</strong></li> 
     <li><strong>Regroupé par : Catégorie RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nom : Principaux segments de Cible</li> 
     <li>Type : Barre</li> 
     <li>Créez un graphique à barres présentant les éléments suivants : Utilisateurs</li> 
     <li>Regroupé par : Action événement</li> 
     <li>Filtre : Afficher uniquement | Catégorie de Événement (contenant) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nom : Sessions par groupes RTP</li> 
     <li>Type : Barre<br></li> 
     <li>Créez un graphique à barres présentant les éléments suivants : Sessions</li> 
     <li>Regroupé par : RTP-Group</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nom : Sessions et objectifs par principaux segments</li> 
     <li>Type : Tableau<br></li> 
     <li>Affichez les colonnes suivantes : <br>Étiquette de Événement | Sessions | Taux de conversion d'objectif</li> 
     <li>Filtre : <br>Afficher uniquement | Catégorie de Événement (contenant) RTP-Segments</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Tableau de bord d’engagement RTP {#rtp-engagement-dashboard}

Ce tableau de bord permet aux utilisateurs d’analyser les performances de leurs campagnes RTP et les engagements de leurs moteurs de recommandation. Il fournit une comparaison de la moyenne. durée de la session et pages par session entre :

* 

   * Non engagé
   * Engagé (impressions et clics sur une campagne personnalisée)
   * Clics sur le moteur de recommandation et le contenu recommandé le plus élevé

Créez un nouveau tableau de bord appelé **Tableau de bord d’engagement RTP** et définissez les widgets suivants :

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Colonne 1 Exposition des campagnes</strong> 
    </div></th> 
   <th> 
    <div> <strong>Colonne 2 Campagnes Clics publicitaires</strong> 
    </div></th> 
   <th> 
    <div> <strong>Moteur de recommandation de colonne 3</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : <strong>CTA total (engagement)</strong></li> 
     <li>Type : <strong>Mesure 2.1 </strong></li> 
     <li>Afficher la mesure suivante : <strong>Événements totaux</strong></li> 
     <li>Filtres : <br><strong>[afficher uniquement] Catégorie de Événement (contient) : RTP-Campaigns</strong><br><strong>[afficher uniquement] l’action du Événement (correspondance exacte) : Impression</strong><strong>[n’affiche pas] Étiquette de Événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>Total CTA (Clics publicitaires)</strong></li> 
     <li>Type : <strong>Mesure 2.1 </strong></li> 
     <li>Afficher la mesure suivante : <strong>Événements totaux</strong></li> 
     <li>Filtres : <br><strong>[afficher uniquement] Catégorie de Événement (contient) : RTP-Campaigns</strong><br><strong>[afficher uniquement] l’action du Événement (correspondance exacte) : Cliquez sur </strong><strong>[n'affiche pas] Étiquette de Événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>CRE - Nombre total de clics</strong></li> 
     <li>Type : <strong>2.1 Mesure</strong><br></li> 
     <li>Afficher la mesure suivante : <strong>Pages vues</strong></li> 
     <li>Filtre : <strong>[afficher uniquement] Page (contenant) : rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nom : <strong>Moy. Durée de la session (engagement)</strong></li> 
     <li>Type : <strong>Mesure 2.1 </strong></li> 
     <li>Afficher la mesure suivante : <strong>Moy. Durée de session</strong></li> 
     <li>Filtres : <br><strong>[afficher uniquement] Catégorie de Événement (correspondant exactement à) : RTP-Campaigns</strong><br><strong>[afficher uniquement] l’action du Événement (correspondance exacte) : impression</strong><strong>[ne pas afficher] Étiquette de Événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nom : <strong>Moy. Durée de la session (clic publicitaire)</strong></li> 
     <li>Type : <strong>Mesure 2.1 </strong></li> 
     <li>Afficher la mesure suivante : <strong>Moy. Durée de session</strong></li> 
     <li>Filtres : <br><strong>[afficher uniquement] Catégorie de Événement (correspondant exactement à) : RTP-Campaigns</strong><br><strong>[afficher uniquement] l’action du Événement (correspondance exacte) : clics</strong><strong>[ne pas afficher] Étiquette de Événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nom : <strong>CRE - Principaux contenus recommandés</strong></li> 
     <li>Type : <strong>Tableau</strong><br></li> 
     <li>Affichez les colonnes suivantes : <br><strong>Titre de la page | Pages vues</strong><br></li> 
     <li>Filtres : <br>Filtre : <strong>[afficher uniquement] Page (contenant) : rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : <strong>Pages / Session (Engagement)</strong></li> 
     <li>Type : <strong>Mesure 2.1 </strong></li> 
     <li>Afficher la mesure suivante : <strong>Pages / Session</strong></li> 
     <li>Filtres : <br><strong>[afficher uniquement] Catégorie de Événement (correspondant exactement à) : RTP-Campaigns</strong></li> 
     <li><strong>[afficher uniquement] Action de Événement (correspondance exacte) : impression</strong></li> 
     <li><strong>[ne pas afficher] Étiquette de Événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>Pages / Session (Clics publicitaires)</strong></li> 
     <li>Type : <strong>Mesure 2.1 </strong></li> 
     <li>Afficher la mesure suivante : <strong>Pages / Session</strong></li> 
     <li>Filtres : <br><strong>[afficher uniquement] Catégorie de Événement (correspondant exactement à) : RTP-Campaigns</strong></li> 
     <li><strong>[afficher uniquement] Action de Événement (correspondance exacte) : clics</strong></li> 
     <li><strong>[ne pas afficher] Étiquette de Événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : <strong>Impressions par CTA</strong></li> 
     <li>Type : <strong>Tableau</strong></li> 
     <li>Affichez les colonnes suivantes : <strong>Étiquette de Événement | Total des Événements | Utilisateurs</strong></li> 
     <li>Filtres : <br><strong>[afficher uniquement] Catégorie de Événement (correspondant exactement à) : RTP-Campaigns</strong><br><strong>[afficher uniquement] l’action du Événement (correspondance exacte) : impression</strong><strong>[ne pas afficher] Étiquette de Événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>Clics publicitaires par CTA</strong></li> 
     <li>Type : <strong>Tableau</strong></li> 
     <li>Affichez les colonnes suivantes : <strong>Étiquette de Événement | Total des Événements | Utilisateurs</strong></li> 
     <li>Filtres : <br><strong>[afficher uniquement] Catégorie de Événement (correspondant exactement à) : RTP-Campaigns</strong><br><strong>[afficher uniquement] l’action du Événement (correspondance exacte) : clics</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Intégration de RTP à Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)
>
>[Rapports RTP personnalisés dans Google Universal Analytics](custom-rtp-reports-in-google-universal-analytics.md)

