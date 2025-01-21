---
unique-page-id: 7504238
description: Tableaux de bord RTP personnalisés dans Google Universal Analytics - Documents Marketo - Documentation du produit
title: Tableaux de bord RTP personnalisés dans Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 89995b2cd6fdc2f2e4ea43906304bdf16d367de1
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Tableaux de bord RTP personnalisés dans Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Intégration du RTP à Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Cette publication explique comment configurer des tableaux de bord RTP dans Google Universal Analytics (GUA). Les données envoyées de RTP vers GUA peuvent être configurées sous la forme de deux tableaux de bord personnalisés distincts appelés :

* RTP B2B
* Engagement RTP

## Configuration d’un tableau de bord personnalisé {#setting-up-a-custom-dashboard}

1. Connectez-vous aux Google Analytics . Cliquez sur **Reporting** dans le menu supérieur. Cliquez sur **Tableaux de bord** puis sur **+Nouveau tableau de bord personnalisé**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Sélectionnez **Zone de travail vierge**, ajoutez un **Nom du tableau de bord** et cliquez sur **Créer un tableau de bord**.

1. Cliquez sur **Ajouter un widget** pour créer un widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Tableau de bord RTP B2B {#rtp-b-b-dashboard}

Ce tableau de bord permet aux utilisateurs d’analyser les performances de leur site web du point de vue B2B.

Il fournit des informations telles que le comportement de la source de visite et sur site par secteur, chiffre d’affaires, taille, listes basées sur les comptes et segments cibles.

Le tableau de bord se compose de 3 colonnes

* Traffic source
* Segmentation
* Analyse micrographique

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
    <div> <strong>Colonne 3 - Zoom micrographique</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : sessions par segments et canaux</li> 
     <li>Type de widget : Barre<br></li> 
     <li>Créez un graphique à barres affichant : Session</li> 
     <li>Regroupé par : libellé de l'événement</li> 
     <li>Pivoter par : regroupement de canaux par défaut</li> 
     <li>Filtre : <br>Afficher uniquement | Catégorie d’événement (contenant) RTP-Segments</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : nombre d’utilisateurs segmentés RTP</li> 
     <li>Type : 2.1 Mesure</li> 
     <li>Afficher la mesure suivante : Utilisateurs<br></li> 
     <li>Filtre : <br>Afficher uniquement | Catégorie d’événement (contenant) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : Sessions par secteur</li> 
     <li>Type : circulaire<br></li> 
     <li>Créez un graphique en secteurs qui affiche : Sessions</li> 
     <li>Regroupé par : RTP-Industry</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nom : Sessions par secteur et canaux</strong></li> 
     <li><strong>Type de widget : Barre</strong></li> 
     <li><strong>Créez un graphique à barres affichant : Session</strong></li> 
     <li><strong>Regroupé par : RTP-Industry</strong></li> 
     <li><strong>Pivoter par : regroupement de canaux par défaut</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nom : sessions segmentées par pays</strong></li> 
     <li><strong>Type : Geomap</strong></li> 
     <li><strong>Tracer la mesure sélectionnée : Pays | Sessions</strong></li> 
     <li><strong>Sélectionner une région : Le Monde</strong></li> 
     <li><strong>Filtre : Afficher uniquement | Catégorie d’événement (contenant) RTP-Segments</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nom : Sessions par catégorie RTP</strong></li> 
     <li><strong>Type : circulaire</strong></li> 
     <li><strong>Créez un graphique en secteurs qui affiche : Sessions</strong></li> 
     <li><strong>Regroupé par : RTP-Category</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nom : Segments Cibles Principaux</li> 
     <li>Type : Barre</li> 
     <li>Créez un graphique à barres affichant les éléments suivants : Utilisateurs</li> 
     <li>Regroupé par : Action d’événement</li> 
     <li>Filtre : Afficher uniquement | Catégorie d’événement (contenant) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nom : Sessions by RTP-Groups</li> 
     <li>Type : Barre<br></li> 
     <li>Créez un graphique à barres affichant : Sessions</li> 
     <li>Regroupé par : RTP-Group</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nom : sessions et objectifs par principaux segments</li> 
     <li>Type : Tableau<br></li> 
     <li>Afficher les colonnes suivantes : <br>Libellé de l'événement | Sessions | Taux de conversion de l’objectif</li> 
     <li>Filtre : <br>Afficher uniquement | Catégorie d’événement (contenant) RTP-Segments</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Tableau de bord d’engagement RTP {#rtp-engagement-dashboard}

Ce tableau de bord permet aux utilisateurs d’analyser les performances de leur campagne RTP et les engagements du moteur de recommandations. Il permet de comparer la moyenne. durée de la session et pages par session entre :

* Inactif
* Engagé (impressions et clics sur une campagne personnalisée)
* Clics sur le moteur de recommandation et contenu le plus recommandé

Créez un tableau de bord appelé **Tableau de bord d’engagement RTP** et définissez les widgets suivants :

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Colonne 1 Exposition des campagnes</strong> 
    </div></th> 
   <th> 
    <div> <strong>Colonne 2 - Clickthrough des campagnes</strong> 
    </div></th> 
   <th> 
    <div> <strong>Colonne 3 Moteur de recommandation</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : <strong>Total CTA (Engagement)</strong></li> 
     <li>Type : <strong>2.1 </strong> métrique</li> 
     <li>Afficher la mesure suivante : <strong>Total des événements</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événement (contient) : RTP-Campagnes</strong><br><strong>[afficher uniquement] Action d’événement (correspondant exactement) : Impression</strong>[ne pas afficher] Libellé d’événement (contenant) : #</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>Total CTA (Clickthrough)</strong></li> 
     <li>Type : <strong>2.1 </strong> métrique</li> 
     <li>Afficher la mesure suivante : <strong>Total des événements</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événement (contient) : RTP-Campagnes</strong><br><strong>[afficher uniquement] Action d’événement (correspondant exactement) : Clics</strong><strong>[ne pas afficher] Libellé d’événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>CRE - Nombre total de clics</strong></li> 
     <li>Type : Mesure <strong>2.1</strong><br></li> 
     <li>Afficher la mesure suivante : <strong>Pages vues</strong></li> 
     <li>Filtre : <strong>[afficher uniquement] Page (contenant) : rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nom : <strong>Moy. Durée de la session (engagement)</strong></li> 
     <li>Type : <strong>2.1 </strong> métrique</li> 
     <li>Afficher la mesure suivante : <strong>Moy. Durée de la session </strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événement (correspondant exactement) : RTP-Campagnes</strong><br><strong>[afficher uniquement] Action d’événement (correspondant exactement) : impression</strong><strong>[ne pas afficher] Libellé d’événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nom : <strong>Moy. Durée de la session (clics publicitaires)</strong></li> 
     <li>Type : <strong>2.1 </strong> métrique</li> 
     <li>Afficher la mesure suivante : <strong>Moy. Durée de la session </strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événement (correspondance exacte) : RTP-Campagnes</strong><br><strong>[afficher uniquement] Action d’événement (correspondance exacte) : clics</strong><strong>[ne pas afficher] Libellé d’événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nom : <strong>CRE - Top Recommended Content</strong></li> 
     <li>Type : <strong>Table</strong><br></li> 
     <li>Afficher les colonnes suivantes : <br><strong>Titre de la page | Pages vues </strong><br></li> 
     <li>Filtres :<br>Filtre : <strong>[afficher uniquement] Page (contenant) : rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : <strong>Pages / Session (Engagement)</strong></li> 
     <li>Type : <strong>2.1 </strong> métrique</li> 
     <li>Afficher la mesure suivante : <strong>Pages/session</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événement (correspondant exactement) : RTP-Campagnes</strong></li> 
     <li><strong>[show uniquement] Action d'événement (correspondant exactement) : impression</strong></li> 
     <li><strong>[ne pas afficher] Libellé de l'événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>Pages / Session (Clickthrough)</strong></li> 
     <li>Type : <strong>2.1 </strong> métrique</li> 
     <li>Afficher la mesure suivante : <strong>Pages/session</strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événement (correspondant exactement) : RTP-Campagnes</strong></li> 
     <li><strong>[afficher uniquement] Action d’événement (correspondant exactement) : clics</strong></li> 
     <li><strong>[ne pas afficher] Libellé de l'événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nom : <strong>Impressions par CTA</strong></li> 
     <li>Type : <strong>Table</strong></li> 
     <li>Afficher les colonnes suivantes : <strong>Libellé de l'événement | Total des événements | Utilisateurs </strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événement (correspondant exactement) : RTP-Campagnes</strong><br><strong>[afficher uniquement] Action d’événement (correspondant exactement) : impression</strong><strong>[ne pas afficher] Libellé d’événement (contenant) : #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nom : <strong>Clickthrough by CTA</strong></li> 
     <li>Type : <strong>Table</strong></li> 
     <li>Afficher les colonnes suivantes : <strong>Libellé de l'événement | Total des événements | Utilisateurs </strong></li> 
     <li>Filtres :<br><strong>[afficher uniquement] Catégorie d’événement (correspondant exactement) : RTP-Campagnes</strong><br><strong>[afficher uniquement] Action d’événement (correspondant exactement) : clics</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Intégration du RTP à Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Rapports RTP personnalisés dans Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
