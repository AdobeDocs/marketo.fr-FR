---
unique-page-id: 7504218
description: Rapports RTP personnalisés dans Google Universal Analytics - Documents Marketo - Documentation du produit
title: Rapports RTP personnalisés dans Google Universal Analytics
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 8%

---

# Rapports RTP personnalisés dans Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Intégration du RTP à Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Cet article explique comment configurer des rapports personnalisés RTP pour Google Universal Analytics (GUA).  Les données envoyées de RTP vers GUA peuvent être configurées sous la forme de deux rapports personnalisés distincts appelés :

* RTP B2B
* Engagement RTP

## Configuration d’un [!UICONTROL rapport personnalisé] {#setting-up-a-custom-report}

1. Connectez-vous à Google Analytics.

1. Cliquez sur **[!UICONTROL Personnalisation]** dans le menu supérieur.

1. Cliquez sur **[!UICONTROL Nouveau rapport personnalisé]**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## Rapport RTP B2B {#rtp-b-b-report}

1. Nommez le rapport **RTP B2B Report**.

1. Nommez le 1er onglet **[!UICONTROL Secteur]**.

>[!NOTE]
>
>Vous allez **Dupliquer cet onglet** et créer d’autres onglets similaires - étape 5)

1. Sélectionnez le type de rapport **[!UICONTROL Explorateur]**.

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. Dans la section **[!UICONTROL Groupes de mesures]**, sélectionnez les mesures pertinentes pour votre entreprise.

   a. Nous recommandons ce qui suit :

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. Dupliquez cet onglet 4 fois et nommez-les :

   1. **Industrie**
   1. **Groupe**
   1. **Catégorie**
   1. **ABM**
   1. **Organisations**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. Dans la section **Analyses Dimension** définissez les dimensions pertinentes pour chaque onglet comme ci-dessous.

<table>
 <thead>
  <tr>
   <th>
    <div>
      Nom de l'onglet
    </div></th>
   <th>
    <div>
      Analyses Dimension détaillées
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>Secteur industriel</td>
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

1. Ne définissez aucun filtre et définissez ce rapport de sorte qu’il soit disponible pour **[!UICONTROL Toutes les données du site web]** (ou modifiez-le si cela concerne un compte Analytics spécifique).

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## Rapport d’engagement RTP {#rtp-engagement-report}

1. Nommez le rapport **RTP Engagement Report**.

1. Définissez le nom du 1er onglet sur **[!UICONTROL Tous les engagements]**.

>[!NOTE]
>
>Vous allez dupliquer cet onglet et en créer d’autres similaires (étape 5)

1. Sélectionnez le type de rapport **[!UICONTROL Explorateur]**.

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Dans la section [!UICONTROL Groupes de mesures], sélectionnez les mesures pertinentes pour votre entreprise. Voici une recommandation :

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Dupliquez cet onglet 4 fois et nommez-les :

   1. **Tous les engagements**
   1. **Engagement du secteur**
   1. **Engagement par groupe**
   1. **Engagement par catégorie**
   1. **Engagement par ABM**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. Dans la section **Analyses Dimension** définissez les dimensions pertinentes pour chaque onglet comme ci-dessous :

<table>
 <thead>
  <tr>
   <th>
    <div>
      Nom de l'onglet
    </div></th>
   <th>
    <div>
      Analyses Dimension détaillées
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
   <td>Engagement de l'industrie</td>
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
   <td><p><span class="uicontrol">Catégorie d’événement</span></p></td>
   <td>Regex</td>
   <td>RTP-Campagnes|RTP-Recommendations|RTP-Segments</td>
   <td colspan="1">Filtre tous les autres événements personnalisés qui ne sont pas liés au RTP.</td>
  </tr>
  <tr>
   <td>Exclure</td>
   <td><span class="uicontrol">Libellé de l’événement</span></td>
   <td>Regex</td>
   <td>#</td>
   <td colspan="1">Permet de filtrer à partir de la campagne de rapports à l’aide de # dans le nom de la campagne</td>
  </tr>
 </tbody>
</table>

1. Définir ce rapport comme étant disponible pour **[!UICONTROL Toutes les données du site Web]** (ou le modifier si nécessaire).

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[Intégration du RTP à Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Tableaux de bord RTP personnalisés dans Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
