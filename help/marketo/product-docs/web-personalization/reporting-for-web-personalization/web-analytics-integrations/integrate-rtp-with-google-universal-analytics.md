---
unique-page-id: 4720125
description: Intégration de RTP à Google Universal Analytics - Documents Marketo - Documentation du produit
title: Intégration de RTP à Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 2%

---

# Intégration de RTP à Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Introduction {#intro}

Tirez parti de Google Universal Analytics (GUA) avec les données de personnalisation et de prévisualisation en temps réel (RTP) de Marketo pour mieux mesurer et analyser vos efforts de marketing en ligne.

Cette publication explique comment configurer et intégrer la plateforme de personnalisation en temps réel de Marketo (RTP) à des comptes Google Universal Analytics (GUA). Les données RTP peuvent être ajoutées à votre compte GOUA, ce qui vous permet d’afficher et de visualiser les performances des organisations, des secteurs, des entreprises et des segments RTP qui visitent votre site web.

**Google Universal Analytics**

Google Universal Analytics avec les données de RTP vous permet de mieux comprendre comment les utilisateurs B2B interagissent avec votre contenu en ligne et vous aide à mesurer et à obtenir de meilleurs résultats de vos campagnes de personnalisation. [En savoir plus sur Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**Pour les utilisateurs du Gestionnaire de balises de Google uniquement**
>
>Aucun codage ni configuration spéciale ne doit être effectué. Assurez-vous de remplir la liste de contrôle suivante :
>
>* Les dimensions RTP sont créées dans Google Universal Analytics
>* [La balise RTP est correctement installée dans Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* L’intégration de Google Universal Analytics est activée dans les paramètres du compte RTP
>* [La balise Google Universal Analytics est correctement configurée dans Google Tag Manager.](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [La balise Gestionnaire de balises de Google est correctement installée sur votre site web.](https://developers.google.com/tag-manager/quickstart)

## Configuration de Dimensions personnalisées dans GUA {#set-up-custom-dimensions-in-gua}

1. En Google Analytics,

   1. Accédez à **Administration**
   1. Sélectionnez la **Compte.**
   1. Sélectionnez la **Propriété.**
   1. Sélectionner **Définitions personnalisées** et **Dimensions personnalisées**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Ajoutez une nouvelle dimension personnalisée. Cliquez sur **+Nouvelle Dimension personnalisée**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Ajoutez ce qui suit : **Dimensions personnalisées :**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Nom de Dimension personnalisé</strong></p></td> 
   <td><p><strong>Portée</strong></p></td> 
   <td><p><strong>Actif</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>Organisation RTP</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industry</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Category</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Group</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Noms de Dimension personnalisés** doit être exactement tel que défini dans le tableau ci-dessus (sinon les tableaux de bord et les rapports RTP personnalisés dans le GUA ne s’afficheront pas correctement).

1. Ajoutez la variable **Nom**. Sélectionnez la portée comme **Session**. Cliquez sur **Créer**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Votre liste de Dimensions personnalisées doit ressembler à ceci.

![](assets/image2014-11-29-11-36-50-version-2.png)

Une fois que vous avez activé les Dimensions personnalisées dans la méthode GUA, accédez à la plateforme RTP pour activer ces dimensions dans la méthode RTP.

## Activation de l’intégration GUA dans votre compte RTP {#activate-the-gua-integration-in-your-rtp-account}

1. Dans la plateforme RTP, accédez à **Paramètres du compte.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Sous **Paramètres du compte**, cliquez sur **Domaine**.
1. Sous **Analytics**, cliquez sur **Google Universal Analytics**.
1. Tourner **Activé** les Dimensions et événements personnalisés appropriés pour ajouter ces données de RTP à Google Universal Analytics.
1. Saisissez le **Numéro d’index** de la dimension alignée sur le numéro d’index en GUA.
1. Cliquez sur **Enregistrer**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Vous trouverez le numéro d’index de la Dimension personnalisée dans la section Dimensions personnalisées.
>
>Exemple : Numéro d’index RTP-Secteur = 1, Numéro d’index RTP-Organisation = 2.

## Suppression des anciens tableaux de bord en Google Analytics {#remove-old-dashboards-in-google-analytics}

1. En Google Analytics. Accédez à **Création de rapports.**
1. Cliquez sur **Tableaux de bord.**
1. Sélectionnez une **Tableau de bord** (Performance RTP B2B ou RTP)
1. Cliquez sur **Supprimer le tableau de bord**.

![](assets/image2014-11-29-11-3a42-3a55.png)
