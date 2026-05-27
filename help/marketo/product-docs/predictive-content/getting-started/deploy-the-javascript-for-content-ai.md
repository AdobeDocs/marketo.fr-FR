---
unique-page-id: 11385053
description: Découvrez comment générer et placer la balise RTP Web Personalization pour le contenu prédictif. Copiez-le dans l’en-tête de votre page, vérifiez la couverture et confirmez que le bouton (bascule) reste activé.
title: Déployer le JavaScript pour l’IA dédiée au contenu
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
TQID: https://experienceleague.adobe.com/LHzl0KuIoJvZ99eFWGFE6RdDW1xRxBS4LG3XU9ujj4U
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 8%

---

# Déployer le JavaScript pour l’IA dédiée au contenu {#deploy-the-javascript-for-content-ai}

Pour utiliser le contenu prédictif, vous devez générer et configurer la balise RTP (Web Personalization).

## Générez un tag {#generate-tag}

1. Connectez-vous à votre compte de contenu prédictif . Accédez à **[!UICONTROL Paramètres du compte]**.

   ![](assets/settings-dropdown-account-hands.png)

1. Dans **[!UICONTROL Configuration du domaine]**, recherchez le domaine approprié et cliquez sur **[!UICONTROL Générer la balise]**.

   ![](assets/generate-tag.png)

1. Copiez et collez la balise Web Personalization dans l’HTML de votre site Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiez la balise Web Personalization JavaScript et collez-la en tant que premier script dans l’en-tête de vos pages, entre les balises `<head> </head>`. Voir les instructions d’implémentation plus détaillées [ici](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Vérifiez que la balise s’affiche sur toutes les pages, y compris les pages de destination et les sous-domaines. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **[!UICONTROL Afficher la page Source]** dans un navigateur web. Recherche : « RTP ».

1. Vérifiez que le bouton (bascule) de la Balise est défini sur **[!UICONTROL ON]**.
