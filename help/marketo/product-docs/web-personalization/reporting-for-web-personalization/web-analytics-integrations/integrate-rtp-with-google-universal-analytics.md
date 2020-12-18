---
unique-page-id: 4720125
description: Intégration de RTP à Google Universal Analytics - Docs marketing - Documentation du produit
title: Intégration de RTP à Google Universal Analytics
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Intégration de RTP avec Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Intro {#intro}

Tirez parti de Google Universal Analytics (GUA) avec les données de personnalisation et de fidélisation de la personnalisation en temps réel de Marketo pour mieux mesurer et analyser vos efforts de marketing en ligne.

Ce billet explique comment configurer et intégrer la plate-forme de personnalisation en temps réel du marketing (RTP) avec les comptes Google Universal Analytics (GUA). Les données RTP peuvent être ajoutées à votre compte GUA, ce qui vous permet de vue et de voir les performances des organisations, industries, secteurs d’activité et segments RTP qui visitent votre site Web.

**Google Universal Analytics**

Google Universal Analytics avec les données de RTP vous permet de mieux comprendre comment les utilisateurs B2B interagissent avec votre contenu en ligne et de mieux mesurer et obtenir de meilleurs résultats à partir de vos campagnes de personnalisation. [En savoir plus sur Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**`For Google Tag Manager Users Only`**
>
>Aucun codage ou configuration spéciale n&#39;est nécessaire. Assurez-vous de remplir la liste de contrôle suivante :
>
>* `RTP dimensions are created in Google Universal Analytics`
>* [La balise RTP est correctement installée dans Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* `Google Universal Analytics Integration is enabled in the RTP's Account Settings`
>* [La balise Google Universal Analytics est correctement configurée dans Google Tag Manager.](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [La balise Google Tag Manager est correctement installée sur votre site Web](https://developers.google.com/tag-manager/quickstart)

>



## Configurer des Dimensions personnalisées dans GUA {#set-up-custom-dimensions-in-gua}

1. En Google Analytics,

   1. Accédez à **Admin**
   1. Sélectionnez le **compte.**
   1. Sélectionnez la **propriété.**
   1. Sélectionnez **Définitions personnalisées **et **Dimensions personnalisées.**

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Ajoutez une nouvelle dimension personnalisée. Cliquez sur **+Nouvelle Dimension personnalisée**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Ajoutez les **Dimensions personnalisées suivantes :**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Nom de la Dimension personnalisée</strong></p></td> 
   <td><p><strong>Portée</strong></p></td> 
   <td><p><strong>Principal</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Organisation</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">obj</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industrie</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">obj</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>Catégorie RTP</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">obj</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Group</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">obj</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Les** noms de Dimension personnalisés doivent être exactement comme définis dans le tableau ci-dessus (sinon les tableaux de bord RTP personnalisés et les rapports dans GUA ne s’afficheront pas correctement)

1. Ajoutez le **nom. **Sélectionnez l’étendue comme **Session.** Cliquez sur  **Créer.**

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Votre liste de Dimension personnalisée doit ressembler à ceci.

![](assets/image2014-11-29-11-36-50-version-2.png)

Une fois que vous avez activé les Dimensions personnalisées dans GUA, accédez à la plate-forme RTP pour activer ces dimensions dans RTP.

## Activez l&#39;intégration GUA dans votre compte RTP {#activate-the-gua-integration-in-your-rtp-account}

1. Dans la plate-forme RTP, accédez à **Paramètres du compte.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Sous **Paramètres du compte**, cliquez sur **Domaine.**
1. Sous **Analytics, **cliquez sur **Google Universal Analytics**.
1. Activez **** les Dimensions et Événements personnalisés appropriés pour ajouter ces données de RTP à Google Universal Analytics.
1. Saisissez le **numéro d&#39;index** de la dimension alignée sur le numéro d&#39;index dans GUA.
1. Cliquez sur **Enregistrer**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Le numéro d&#39;index de la Dimension personnalisée se trouve dans GUA sous Dimensions personnalisées.
>
>Exemple : Numéro d&#39;index RTP-Industrie = 1, Numéro d&#39;index RTP-Organisation = 2.

## Supprimer les anciens Tableaux de bord en Google Analytics {#remove-old-dashboards-in-google-analytics}

1. En Google Analytics. Accédez au **Rapports.**
1. Cliquez sur **Tableaux de bord.**
1. Sélectionnez un **Tableau de bord **(RTP B2B ou RTP Performance).
1. Cliquez sur **Supprimer le Tableau de bord**.

![](assets/image2014-11-29-11-3a42-3a55.png)

