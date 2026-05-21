---
unique-page-id: 4719332
description: Découvrez comment déployer le code JavaScript rtp dans Marketo Engage, notamment comment déployer le code JavaScript rtp. Utilisez ce guide pour passer à l’étape suivante.
title: Déployer le JavaScript RTP
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XUylNa8clUib-aMhpAR8fjeu4pHRA8KSQydSH1AVxF8
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
source-wordcount: 184
ht-degree: 4%

---

# Déployer le JavaScript RTP {#deploy-the-rtp-javascript}

Pour générer et configurer votre balise RTP, suivez les instructions d’installation ci-dessous

## [!UICONTROL Générer la balise] {#generate-tag}

1. Connectez-vous à votre compte RTP. Accédez à **[!UICONTROL Paramètres du compte]**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. Dans **[!UICONTROL Domain]** et **[!UICONTROL Domain Configuration]**, recherchez le domaine approprié et cliquez sur **[!UICONTROL Generate Tag]**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Copiez et collez la balise Web Personalization (RTP) dans votre site Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiez la balise JavaScript RTP et collez-la en tant que premier script dans l’en-tête de vos pages, entre les balises `<head> </head>`.

   Assurez-vous que la balise s’affiche sur toutes les pages, y compris les pages de destination et les sous-domaines. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à Afficher la page Source dans un navigateur web. Recherche : « RTP ».

1. [!UICONTROL Balise] activer/désactiver **[!UICONTROL ON]**.

   Vérifiez que le bouton bascule [!UICONTROL Balise] est défini sur [!UICONTROL ON]. Vous devriez commencer à voir le flux de données dans l’onglet de l’organisation.

   Vous êtes maintenant configuré avec la balise RTP et prêt à commencer la [création de segments](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) et de campagnes en temps réel !

1. Vérifiez que la balise se trouve sur toutes les pages.
