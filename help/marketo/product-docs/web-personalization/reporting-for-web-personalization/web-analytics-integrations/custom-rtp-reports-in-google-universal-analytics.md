---
unique-page-id: 7504218
description: Rapports RTP personnalisés dans Google Universal Analytics - Docs marketing - Documentation sur les produits
title: Rapports RTP personnalisés dans Google Universal Analytics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---


# Rapports RTP personnalisés dans Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Intégration de RTP à Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)

Cette publication explique comment configurer des rapports personnalisés RTP pour Google Universal Analytics (GUA).  Les données envoyées de RTP à GUA peuvent être configurées sous la forme de deux rapports personnalisés distincts appelés :

* RTP B2B
* Engagement RTP

## Configuration d’un rapport personnalisé {#setting-up-a-custom-report}

1. Connectez-vous aux Google Analytics.
1. Cliquez sur **Personnalisation **dans le menu supérieur.
1. Cliquez sur **+Nouveau rapport personnalisé.**

** ![](assets/image2015-3-22-16-3a10-3a48.png)

**

## Rapport RTP B2B {#rtp-b-b-report}

1. Nommez le rapport **RTP B2B Report**.
1. Nommer le 1er onglet **Industrie **

   1. (Remarque : vous allez **Duplicata cet onglet** et en créer d&#39;autres similaires - étape 5)

1. Sélectionnez le type de rapport** Explorer**.\
   ** ![](assets/image2015-3-22-16-3a15-3a25.png)

   **

1. Dans la section **Groupes de mesures**, sélectionnez les mesures pertinentes pour votre activité.

   1. Nous vous recommandons ce qui suit :\
      ** ![](assets/image2015-3-22-16-3a16-3a40.png)

      **

1. Duplicata cet onglet 4 fois et nommez-le :

   1. **Industrie**
   1. **Groupe**
   1. **Catégorie**
   1. **ABM**
   1. **Organisations**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. Dans la section **Zoom sur la Dimension**, définissez les dimensions appropriées pour chaque onglet comme ci-dessous.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nom d’onglet 
    </div></th> 
   <th> 
    <div>
      Zoom sur les Dimensions 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Industrie</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Groupe</td> 
   <td><img src="assets/2.png" data-linked-resource-id="7514674" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Catégorie</td> 
   <td><img src="assets/3.png" data-linked-resource-id="7514673" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Organisations</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Ne définissez aucun filtres et ne configurez pas ce rapport pour qu’il soit disponible pour **Toutes les données du site Web ** (ou modifiez-le s’il est pertinent pour un compte Analytics spécifique).
1. Cliquez sur **Enregistrer**.\
   ![](assets/image2015-3-22-16-3a21-3a23.png)

## Rapport d’engagement RTP {#rtp-engagement-report}

1. Nommez le rapport **Rapport Engagement RTP.**
1. Définissez le premier nom d’onglet sur **Tous les engagements**.

   1. (Remarque : vous allez Duplicata cet onglet et en créer d&#39;autres similaires - étape 5)

1. Sélectionnez le type de rapport **Explorateur**.\
   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Dans la section Groupes de mesures, sélectionnez les mesures pertinentes pour votre activité. Voici une recommandation :\
   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplicata cet onglet 4 fois et nommez-le :

   1. **Tous les engagements**
   1. **Engagement de l&#39;industrie**
   1. **Engagement par groupe**
   1. **Engagement par Catégorie**
   1. **Engagement par ABM**

   ** ![](assets/image2015-3-22-16-3a26-3a21.png)\**

1. Dans la section **Analyses de Dimension**, définissez les dimensions appropriées pour chaque onglet comme suit :

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nom d’onglet 
    </div></th> 
   <th> 
    <div>
      Zoom sur les Dimensions 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Tous les engagements</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagement par ABM</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagement par Catégorie</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagement par groupe</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagement de l'industrie</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Définissez les filtres suivants :
1. 

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      Champ 
    </div></th> 
   <th> 
    <div>
      Type de correspondance 
    </div></th> 
   <th> 
    <div>
      Valeurs 
    </div></th> 
   <th colspan="1"> 
    <div>
      Commentaires 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>Inclure</p></td> 
   <td><p>Catégorie événement</p></td> 
   <td>Regex</td> 
   <td>RTP-Campagnes|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">Filtre tous les autres événements personnalisés qui ne sont pas liés à RTP</td> 
  </tr> 
  <tr> 
   <td>Exclure</td> 
   <td>Étiquette de événement</td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">Permet de filtrer de votre campagne de rapports en utilisant # dans le nom de la campagne.</td> 
  </tr> 
 </tbody> 
</table>

1. Définir ce rapport comme disponible pour **Toutes les données du site Web **(ou le modifier si nécessaire)

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Cliquez sur **Enregistrer**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!NOTE]
>
>**Articles connexes**
>
>[Intégration de RTP à Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)
>
>[Tableaux de bord RTP personnalisés dans Google Universal Analytics](custom-rtp-dashboards-in-google-universal-analytics.md)

