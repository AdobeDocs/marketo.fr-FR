---
unique-page-id: 4720125
description: Intégration du RTP à Google Universal Analytics - Documentation de Marketo - Documentation du produit
title: Intégration du RTP à Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 3%

---

# Intégrer le RTP à [!DNL Google Universal Analytics] {#integrate-rtp-with-google-universal-analytics}

## Introduction {#intro}

Tirez parti de [!DNL Google Universal Analytics] (GUA) avec les données firmographiques et de personnalisation de [!DNL Marketo Real-Time Personalization] (RTP) pour mieux mesurer et analyser vos efforts de marketing en ligne.

Cette publication explique comment configurer et intégrer la plateforme [!DNL Marketo Real-Time Personalization] (RTP) aux comptes [!DNL Google Universal Analytics] (GUA). Les données RTP peuvent être ajoutées à votre compte GUA, ce qui vous permet d’afficher et de voir les performances des organisations, des secteurs d’activité, des graphiques et des segments RTP qui visitent votre site web.

**[!DNL Google Universal Analytics]**

[!DNL Google Universal Analytics] avec les données de RTP vous permet de mieux comprendre comment les utilisateurs B2B interagissent avec votre contenu en ligne et de mesurer et d’obtenir de meilleurs résultats de vos campagnes de personnalisation. [En savoir plus sur  [!DNL Google Universal Analytics]](https://support.google.com/analytics/answer/2790010/?hl=en&authuser=1).

>[!NOTE]
>
>**Pour Les Utilisateurs Du Gestionnaire De Balises De Google Uniquement**
>
>Aucun codage ou configuration spéciale ne doit être effectué. Veillez à compléter la liste de contrôle suivante :
>
>* Les dimensions RTP sont créées dans [!DNL Google Universal Analytics]
>* [La balise RTP est correctement installée dans le Gestionnaire de balises Google](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* L&#39;intégration [!DNL Google Universal Analytics] est activée dans les paramètres du compte RTP
>* [[!DNL Google Universal Analytics] la balise est correctement configurée dans le Gestionnaire de balises Google](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [La balise du Gestionnaire de balises Google est correctement installée sur votre site web](https://developers.google.com/tag-manager/quickstart)

## Configurer des dimensions personnalisées dans GUA {#set-up-custom-dimensions-in-gua}

1. Dans Google Analytics,

   1. Accédez à **[!UICONTROL Admin]**
   1. Sélectionnez le **[!UICONTROL Compte].**
   1. Sélectionnez la **[!UICONTROL Propriété].**
   1. Sélectionnez **[!UICONTROL Définitions personnalisées]** et **[!UICONTROL Dimensions personnalisées]**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Ajoutez une nouvelle dimension personnalisée. Cliquez sur **[!UICONTROL +Nouveau Dimension personnalisé]**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Ajoutez les **[!UICONTROL dimensions personnalisées] suivantes :**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Nom de Dimension personnalisé</strong></p></td> 
   <td><p><strong>Portée</strong></p></td> 
   <td><p><strong>Actif</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Organisation</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industrie</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Category</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>Groupe RTP</strong></p></td> 
   <td><p>Session</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Les **Noms de Dimension personnalisés** doivent être exactement comme définis dans le tableau ci-dessus (sinon les tableaux de bord et rapports RTP personnalisés dans GUA ne s’afficheront pas correctement)

1. Ajoutez le **[!UICONTROL Nom]**. Sélectionnez la Portée **[!UICONTROL Session]**. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Votre liste de Dimension personnalisée doit se présenter comme suit :

![](assets/image2014-11-29-11-36-50-version-2.png)

Une fois que vous avez activé les dimensions personnalisées dans GUA, accédez à la plateforme RTP pour activer ces dimensions dans RTP.

## Activer l’intégration de la GUA dans votre compte RTP {#activate-the-gua-integration-in-your-rtp-account}

1. Dans la plateforme RTP, accédez à **[!UICONTROL Paramètres du compte].**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Sous **[!UICONTROL Paramètres du compte]**, cliquez sur **[!UICONTROL Domaine]**.
1. Sous **[!UICONTROL Analytics]**, cliquez sur **[!UICONTROL Google Universal Analytics]**.
1. Activez **[!UICONTROL Activez]** les dimensions et événements personnalisés appropriés pour ajouter ces données du RTP au [!DNL Google Universal Analytics].
1. Saisissez le **[!UICONTROL Numéro d’index]** de la dimension alignée sur le numéro d’index dans GUA.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>Le numéro d’index du Dimension personnalisé se trouve dans GUA sous Dimensions personnalisées.
>
>Exemple : le numéro d&#39;index RTP-Industry est égal à 1, le numéro d&#39;index RTP-Organization est égal à 2.

## Supprimer les anciens tableaux de bord dans Google Analytics {#remove-old-dashboards-in-google-analytics}

1. Dans Google Analytics. Accédez à **[!UICONTROL Reporting].**
1. Cliquez sur **[!UICONTROL Tableaux de bord ].**.
1. Sélectionnez un **[!UICONTROL Tableau de bord]** (RTP B2B ou Performances RTP)
1. Cliquez sur **[!UICONTROL Supprimer le tableau de bord]**.

![](assets/image2014-11-29-11-3a42-3a55.png)
