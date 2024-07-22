---
unique-page-id: 7504238
description: Tableaux de bord RTP personnalisés dans Google Universal Analytics - Documents Marketo - Documentation du produit
title: Tableaux de bord RTP personnalisés dans Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Tableaux de bord RTP personnalisés dans Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Intégration de RTP à Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Cette publication explique comment configurer des tableaux de bord RTP dans Google Universal Analytics (GUA). Les données envoyées de la méthode RTP à la méthode GUA peuvent être configurées en tant que deux tableaux de bord personnalisés distincts appelés :

* RTP B2B
* Engagement RTP

## Configuration d’un tableau de bord personnalisé {#setting-up-a-custom-dashboard}

1. Connectez-vous aux Google Analytics. Cliquez sur **Reporting** dans le menu supérieur. Cliquez sur **Tableaux de bord** et **+Nouveau tableau de bord personnalisé**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Sélectionnez **Canevas vierge**, ajoutez un **nom du tableau de bord** et cliquez sur **Créer un tableau de bord**.

1. Cliquez sur **Ajouter un widget** pour créer un widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Tableau de bord RTP B2B {#rtp-b-b-dashboard}

Ce tableau de bord permet aux utilisateurs d’analyser les performances de leur site web du point de vue B2B.

Il fournit des informations telles que le comportement de la source des visites et du site par secteur, recettes, taille, listes basées sur les comptes et segments cibles.

Le tableau de bord se compose de 3 colonnes.

* Source du trafic
* Segmentation
* Exploration de la technologie

1. Créez un tableau de bord appelé **Tableau de bord B2B RTP** et définissez les widgets suivants :

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
    <div> <strong>Colonne 3 - Zoom avant sur la micrographie</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : sessions par segments et canaux</li> 
     <li>Type de widget : Barre<br></li> 
     <li>Création d’un graphique à barres présentant : Session</li> 
     <li>Regroupement par : libellé de l'événement</li> 
     <li>Pivoter par : Regroupement de canaux par défaut</li> 
     <li>Filtre : <br> Afficher uniquement | Catégorie d’événements (contenant) RTP-Segments</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : nombre d’utilisateurs segmentés par HTTP</li> 
     <li>Type : mesure 2.1</li> 
     <li>Afficher la mesure suivante : Utilisateurs<br></li> 
     <li>Filtre : <br> Afficher uniquement | Catégorie d’événements (contenant) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : Sessions par secteur industriel</li> 
     <li>Type : secteurs<br></li> 
     <li>Créez un graphique circulaire présentant : Sessions</li> 
     <li>Regroupé par : RTP-Industry</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nom : Sessions par secteur et canaux</strong></li> 
     <li><strong>Type de widget : Barre</strong></li> 
     <li><strong>Création d’un graphique à barres présentant : Session</strong></li> 
     <li><strong>Regroupé par : RTP-Industry</strong></li> 
     <li><strong>Pivoter par : Regroupement de canaux par défaut</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nom : Sessions segmentées par pays</strong></li> 
     <li><strong>Type : Geomap</strong></li> 
     <li><strong>Traiter la mesure sélectionnée : Pays | Sessions</strong></li> 
     <li><strong>Choisissez une région : le monde</strong></li> 
     <li><strong>Filtre : Afficher uniquement | Catégorie d’événements (contenant) RTP-Segments</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nom : Sessions par catégorie de HTTP</strong></li> 
     <li><strong>Type : secteurs</strong></li> 
     <li><strong>Créez un graphique circulaire présentant : Sessions</strong></li> 
     <li><strong>Regroupé par : catégorie-RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nom : Segments cibles principaux</li> 
     <li>Type : Barre</li> 
     <li>Créez un graphique à barres affichant : Utilisateurs</li> 
     <li>Groupé par : Action de l’événement</li> 
     <li>Filtre : Afficher uniquement | Catégorie d’événements (contenant) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nom : Sessions par groupes RTP</li> 
     <li>Type : Barre<br></li> 
     <li>Créez un graphique à barres affichant : Sessions</li> 
     <li>Regroupé par : Groupe-RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nom : Sessions et objectifs par principaux segments</li> 
     <li>Type : Tableau<br></li> 
     <li>Afficher les colonnes suivantes : <br>Libellé de l'événement | Sessions | Taux de conversion de l’objectif</li> 
     <li>Filtre : <br> Afficher uniquement | Catégorie d’événements (contenant) RTP-Segments</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Tableau de bord de l’engagement RTP {#rtp-engagement-dashboard}

Ce tableau de bord permet aux utilisateurs d’analyser les performances de leur campagne RTP et les engagements de leur moteur de recommandations. Il fournit une comparaison de la moyenne. durée de session et pages par session entre :

* Non engagé
* Engagé (impressions et clics sur une campagne personnalisée)
* Clics sur le moteur de recommandation et le contenu recommandé supérieur

Créez un tableau de bord appelé **Tableau de bord de l’engagement RTP** et définissez les widgets suivants :

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Exposition des campagnes sur la colonne 1</strong> 
    </div></th> 
   <th> 
    <div> <strong>Clics sur les campagnes de colonne 2</strong> 
    </div></th> 
   <th> 
    <div> <strong>Moteur de recommandation Colonne 3</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : <strong>Total CTA (engagement)</strong></li> 
     <li>Type : <strong>2.1 Metric </strong></li> 
     <li>Afficher la mesure suivante : <strong>Total des événements</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événements (contient) : RTP-Campaigns</strong><br><strong>[afficher uniquement] Action d’événement (correspondance exacte) : Impression</strong><strong>[n’afficher pas] Étiquette d’événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>Total CTA (clic publicitaire)</strong></li> 
     <li>Type : <strong>2.1 Metric </strong></li> 
     <li>Afficher la mesure suivante : <strong>Total des événements</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événements (contient) : RTP-Campaigns</strong><br><strong>[afficher uniquement] Action d’événement (correspondance exacte) : Clics</strong><strong>[n’afficher pas] Étiquette d’événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>CRE - Nombre total de clics</strong></li> 
     <li>Type : <strong>2.1 Metric</strong><br></li> 
     <li>Afficher la mesure suivante : <strong>Pageviews</strong></li> 
     <li>Filtre : <strong>[afficher uniquement] Page (contenant) : rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nom : <strong>Durée Durée de la session (engagement)</strong></li> 
     <li>Type : <strong>2.1 Metric </strong></li> 
     <li>Afficher la mesure suivante : <strong>Durée Durée de la session</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événements (correspondance exacte) : RTP-Campagnes</strong><br><strong>[afficher uniquement] Action d’événement (correspondance exacte) : impression</strong><strong>[n’afficher pas] Étiquette d’événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nom : <strong>Durée Durée de la session (clic publicitaire)</strong></li> 
     <li>Type : <strong>2.1 Metric </strong></li> 
     <li>Afficher la mesure suivante : <strong>Durée Durée de la session</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événements (correspondance exacte) : RTP-Campagnes</strong><br><strong>[afficher uniquement] Action d’événement (correspondance exacte) : clics</strong><strong>[n’afficher pas] Étiquette d’événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nom : <strong>CRE - Top Recommandé Content</strong></li> 
     <li>Type : <strong>Table</strong><br></li> 
     <li>Afficher les colonnes suivantes : <br><strong>Titre de page | Pageviews</strong><br></li> 
     <li>Filtres :<br>Filtre : <strong>[afficher uniquement] Page (contenant) : rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : <strong> Pages / Session (engagement)</strong></li> 
     <li>Type : <strong>2.1 Metric </strong></li> 
     <li>Afficher la mesure suivante : <strong>Pages / Session</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événements (correspondance exacte) : RTP-Campagnes</strong></li> 
     <li><strong>[afficher uniquement] Action de l’événement (correspondance exacte) : impression</strong></li> 
     <li><strong>[ne pas afficher] Libellé de l’événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong> Pages / Session (clic publicitaire)</strong></li> 
     <li>Type : <strong>2.1 Metric </strong></li> 
     <li>Afficher la mesure suivante : <strong>Pages / Session</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événements (correspondance exacte) : RTP-Campagnes</strong></li> 
     <li><strong>[afficher uniquement] Action de l’événement (correspondance exacte) : clics</strong></li> 
     <li><strong>[ne pas afficher] Libellé de l’événement (contenant) : #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : <strong>Impressions par CTA</strong></li> 
     <li>Type : <strong>Table</strong></li> 
     <li>Afficher les colonnes suivantes : <strong>Libellé de l'événement | Nombre total d’événements | Utilisateurs</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événements (correspondance exacte) : RTP-Campagnes</strong><br><strong>[afficher uniquement] Action d’événement (correspondance exacte) : impression</strong><strong>[n’afficher pas] Étiquette d’événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>Clickthrough by CTA</strong></li> 
     <li>Type : <strong>Table</strong></li> 
     <li>Afficher les colonnes suivantes : <strong>Libellé de l'événement | Nombre total d’événements | Utilisateurs</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événements (correspondance exacte) : RTP-Campaigns</strong><br><strong>[afficher uniquement] Action d’événement (correspondance exacte) : clics</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Intégration de RTP à Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Rapports RTP personnalisés dans Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
