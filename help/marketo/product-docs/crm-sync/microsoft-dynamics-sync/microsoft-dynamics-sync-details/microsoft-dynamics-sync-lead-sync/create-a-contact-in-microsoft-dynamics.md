---
unique-page-id: 10095389
description: Découvrez comment créer un contact dans Microsoft Dynamics depuis Marketo. Utilisez l’action de flux Synchroniser la personne avec Microsoft dans une campagne de déclenchement pour la création de contacts en temps réel.
title: Créer un contact dans Microsoft Dynamics
exl-id: 66cb26c0-f383-4d1e-be22-e7f8c6b266fb
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/5q84B57P88MNhaYHluCKKCYLwOonW2xj7hAUNDOmXl8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 4%
---
# Créer un contact dans [!DNL Microsoft Dynamics] {#create-a-contact-in-microsoft-dynamics}

1. Sélectionnez la personne en mode Marketo Engage uniquement (le type de Microsoft est vide) que vous souhaitez créer en tant que contact dans Dynamics.

   ![](assets/one.png)

1. Cliquez sur **[!UICONTROL Actions de personne]** et **[!DNL Microsoft]**, puis sélectionnez **[!UICONTROL Synchroniser la personne avec Microsoft]**.

   ![](assets/two.png)

1. Cliquez sur **[!UICONTROL Synchroniser avec]** et sélectionnez **[!UICONTROL Contact]**. Cliquez sur **[!UICONTROL Exécuter maintenant]**.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Lors de l’utilisation de l’action de flux « [!UICONTROL Synchroniser la personne avec Microsoft] » (dans une campagne Trigger uniquement), le prospect/contact est créé en temps réel dans Dynamics.

1. Marketo qualifie cet enregistrement de lead dans [!DNL Dynamics] en contact qui n’est associé à aucun compte dans [!DNL Dynamics].

   ![](assets/image2015-10-23-9-3a43-3a33.png)

1. Vous pouvez désormais sélectionner **[!UICONTROL Contact]** lorsque vous utilisez la contrainte Synchroniser en tant que dans un filtre de campagne dynamique.

   ![](assets/five.png)
