---
unique-page-id: 7504218
description: Rapports RTP personnalisés dans Google Universal Analytics - Documents Marketo - Documentation du produit
title: Rapports RTP personnalisés dans Google Universal Analytics
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 5%

---

# Rapports RTP personnalisés dans Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Intégration de RTP à Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Cet article explique comment configurer des rapports personnalisés RTP pour Google Universal Analytics (GUA).  Les données envoyées de RTP vers GUA peuvent être configurées en tant que deux rapports personnalisés distincts appelés :

* RTP B2B
* Engagement RTP

## Configuration d’un rapport personnalisé {#setting-up-a-custom-report}

1. Connectez-vous aux Google Analytics.

1. Cliquez sur **Personnalisation** dans le menu supérieur.

1. Cliquez sur **+Nouveau rapport personnalisé**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## Rapport RTP B2B {#rtp-b-b-report}

1. Nommer le rapport **Rapport RTP B2B**.

1. Nommer le premier onglet **Secteur industriel**.

>[!NOTE]
>
>Vous aurez **Dupliquer cet onglet** et créer d’autres similaires - étape 5)

1. Sélectionnez la **Explorateur** type de rapport.

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. Dans le **Groupes de mesures** , sélectionnez les mesures pertinentes pour votre entreprise.

   a. Nous vous recommandons ce qui suit :

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. Dupliquez cet onglet 4 fois et nommez-les :

   1. **Secteur**
   1. **Groupe**
   1. **Catégorie**
   1. **ABM**
   1. **Entreprises**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. Dans le **Analyse des Dimensions** définissez les dimensions pertinentes pour chaque onglet, comme ci-dessous.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nom de l'onglet 
    </div></th> 
   <th> 
    <div>
      Analyse des Dimensions
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Secteur</td> 
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
   <td>Entreprises</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Ne définissez aucun filtre et ne définissez pas ce rapport pour qu’il soit disponible. **Toutes les données de site Web** (ou changez si cela est pertinent pour un compte Analytics spécifique).

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## Rapport Engagement RTP {#rtp-engagement-report}

1. Nommer le rapport **Rapport Engagement RTP**.

1. Définissez le nom du 1er onglet sur **Tous les engagements**.

>[!NOTE]
>
>Vous allez dupliquer cet onglet et en créer d’autres similaires - étape 5)

1. Sélectionnez la **Explorateur** type de rapport.

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Dans la section Groupes de mesures , sélectionnez les mesures pertinentes pour votre entreprise. Voici une recommandation :

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Dupliquez cet onglet 4 fois et nommez-les :

   1. **Tous les engagements**
   1. **Engagement du secteur industriel**
   1. **Engagement par groupe**
   1. **Engagement par catégorie**
   1. **Engagement par ABM**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. Dans le **Analyse des Dimensions** définissez les dimensions pertinentes pour chaque onglet, comme ci-dessous :

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nom de l'onglet 
    </div></th> 
   <th> 
    <div>
      Analyse des Dimensions 
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
   <td>Engagement par catégorie</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagement par groupe</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagement du secteur industriel</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Définissez les filtres suivants :

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
   <td><p>Catégorie d’événement</p></td> 
   <td>Regex</td> 
   <td>RTP-Campagnes|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">Filtrez tous les autres événements personnalisés qui ne sont pas liés à la méthode RTP</td> 
  </tr> 
  <tr> 
   <td>Exclure</td> 
   <td>Libellé d’événement</td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">Permet de filtrer de votre campagne de rapports à l’aide de # dans le nom de la campagne.</td> 
  </tr> 
 </tbody> 
</table>

1. Définir ce rapport pour qu’il soit disponible **Toutes les données de site Web** (ou changez si nécessaire).

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Cliquez sur **Enregistrer**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[Intégration de RTP à Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Tableaux de bord RTP personnalisés dans Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
