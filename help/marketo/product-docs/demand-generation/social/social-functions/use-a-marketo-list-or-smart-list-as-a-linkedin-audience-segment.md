---
unique-page-id: 7504180
description: Découvrez comment utiliser une liste Marketo ou une liste dynamique en tant que segment d’audience LinkedIn. Envoi de listes à LinkedIn pour le ciblage publicitaire via Ad Bridge.
title: Utiliser une liste Marketo ou une liste intelligente comme segment ciblé LinkedIn
exl-id: 9a7943fe-b2e7-443a-87e0-da01001682de
feature: Social
TQID: 'https://experienceleague.adobe.com/n7Z4AKx6Hiu6f9cxXPpfSTJJdOLakTwy7ejQ-6LK4Bo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: e9b7b90f-6f8a-4637-a2ca-00239808918c
    internal-label: Social
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 14%
---
# Utiliser une liste Marketo ou une liste intelligente comme segment ciblé LinkedIn {#use-a-marketo-list-or-smart-list-as-a-linkedin-audience-segment}

Intégrez vos utilisateurs Marketo Engage à vos audiences LinkedIn.

>[!PREREQUISITES]
>
>[Ajout d’audiences correspondantes LinkedIn en tant que service LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}

1. Accédez à la **[!UICONTROL Base de données]**.

   ![](assets/list-as-a-linkedin-audience-segment-1.png)

1. Sélectionnez une liste dynamique.

   ![](assets/list-as-a-linkedin-audience-segment-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Personnes]**.

   ![](assets/list-as-a-linkedin-audience-segment-3.png)

1. Cliquez sur l’icône **[!UICONTROL Envoyer via Ad Bridge]** ![, &#x200B;](assets/icon-ad-bridge.png) au bas de la liste.

   ![](assets/list-as-a-linkedin-audience-segment-4.png)

   >[!NOTE]
   >
   >Lors de l’utilisation d’intégrations de réseau publicitaire pour envoyer une audience à LinkedIn, Marketo envoie uniquement l’adresse e-mail.

1. Sélectionnez **[!UICONTROL LinkedIn]** et cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/list-as-a-linkedin-audience-segment-5.png)

1. Sélectionnez une **[!UICONTROL audience LinkedIn]**.

   >[!NOTE]
   >
   >Cliquez sur **[!UICONTROL +Nouvelle audience]** pour créer une audience dans LinkedIn Campaign Manager.

   ![](assets/list-as-a-linkedin-audience-segment-6.png)

   >[!NOTE]
   >
   >LinkedIn a abandonné les API utilisées pour le type de notification push « Effacer l’audience et ajouter des prospects » en mars 2018. Cette option n’est plus disponible à compter de la version de Marketo du 1er trimestre 2018.

1. Sélectionnez un **[!UICONTROL type push]**. Cliquez sur **[!UICONTROL Mettre à jour]**.

   ![](assets/list-as-a-linkedin-audience-segment-7.png)

   >[!NOTE]
   >
   >Patientez 15 minutes pour que la synchronisation se termine.

Vos données vont maintenant être synchronisées avec les audiences de LinkedIn. Pour plus d’informations sur le téléchargement de listes vers LinkedIn pour le ciblage des comptes et des contacts, consultez [Centre d’aide des solutions marketing de LinkedIn](https://www.linkedin.com/help/lms/answer/73938?query=ad%20segment){target="_blank"}.
