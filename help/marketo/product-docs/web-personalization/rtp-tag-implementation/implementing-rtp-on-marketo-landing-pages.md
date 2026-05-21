---
unique-page-id: 4720151
description: Découvrez l’implémentation du rtp sur les pages de destination marketo dans Marketo Engage, y compris l’implémentation du rtp sur marketo. Utilisez ce guide pour passer à l’étape suivante.
title: Mise en œuvre de RTP sur les pages de destination Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
TQID: https://experienceleague.adobe.com/scyZfbFBloPu8JRfJiMjm62AFCHM7WCxaats3qssq2A
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 213
ht-degree: 5%

---

# Mise en œuvre de RTP sur les pages de destination Marketo {#implementing-rtp-on-marketo-landing-pages}

Pour implémenter votre balise [!UICONTROL RTP] suivez les instructions d’installation ci-dessous :

1. Accédez au **[!UICONTROL Design Studio].** Ouvrez l’élément que vous souhaitez modifier. Sélectionnez **[!UICONTROL Actions de modèle]**, puis **[!UICONTROL Modifier le brouillon]**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Apportez vos modifications de modèle dans l’onglet **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Dans votre compte RTP, accédez à **[!UICONTROL Paramètres du compte]**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Sous [!UICONTROL Domaine], recherchez le domaine approprié et cliquez sur **[!UICONTROL Générer la balise]**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copiez la balise JavaScript RTP et collez-la dans tous les modèles de page de destination compris entre les balises **`<head> </head>`**.

1. Cliquez sur **[!UICONTROL Enregistrer]** et **[!UICONTROL Fermer]** dans la fenêtre.

1. De retour dans **[!UICONTROL Design Studio]**, approuvez la page de destination à partir de **[!UICONTROL Actions de modèle]**, puis cliquez sur **[!UICONTROL Approuver]**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Enfin, vous devrez **réapprouver** toutes les pages de destination utilisant ce modèle pour que les modifications du modèle prennent effet. Vous pouvez toutes les approuver de nouveau en même temps à partir de la section principale [!UICONTROL Pages de destination].

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Vérifiez qu’il apparaît sur toutes les pages, y compris les pages de destination et les sous-domaines.

   Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **[!UICONTROL Afficher la page Source].** Recherchez **[!UICONTROL RTP]** pour localiser la balise.
