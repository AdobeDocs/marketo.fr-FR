---
unique-page-id: 4720145
description: Découvrez l’implémentation de rtp à l’aide de Google Tag Manager dans Marketo Engage, y compris l’implémentation de rtp à l’aide de dnl google. Utilisez ce guide pour passer à l’étape suivante.
title: Mise en œuvre de RTP à l’aide de Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XesXGBf2aDsnsbS2Ro1RLdd1EVrj-mBdCiv8C0dj8NU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 173
ht-degree: 3%

---

# Mise en œuvre du RTP à l’aide de [!DNL Google Tag Manager] {#implementing-rtp-using-google-tag-manager}

Pour implémenter votre balise RTP, suivez les instructions d’installation ci-dessous.

1. Connectez-vous à votre compte [!DNL Google Tag Manager].

1. Ajoutez une nouvelle **[!UICONTROL Balise]** > **[!UICONTROL Configurations des balises]** > **[!UICONTROL Balise HTML personnalisée].** Appelez-le **RTP**.

1. Connectez-vous à votre **compte RTP**.

1. Accédez à **[!UICONTROL Paramètres du compte]**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance, passez à l’étape 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Sous [!UICONTROL Domaine], recherchez le domaine approprié et cliquez sur **[!UICONTROL Générer la balise]**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copiez la balise JavaScript RTP et collez-la dans la nouvelle **balise HTML personnalisée** créée (étape 1).

1. Cliquez sur **[!UICONTROL Ajouter une règle à la balise Fire]**. Sélectionnez **[!UICONTROL Toutes les pages]**.

1. Cliquez sur **[!UICONTROL Enregistrer]** et [publier la nouvelle version](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Vérifiez qu’il apparaît sur toutes les pages, y compris les pages de destination et les sous-domaines.

   a. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **[!UICONTROL Inspecter l’élément]**, recherchez **RTP** pour localiser la balise.
