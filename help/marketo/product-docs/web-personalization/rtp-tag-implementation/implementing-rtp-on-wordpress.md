---
unique-page-id: 4720149
description: Découvrez l’implémentation du rtp sur wordpress dans Marketo Engage, y compris l’implémentation du rtp sur dnl wordpress. Utilisez ce guide pour passer à l’étape suivante.
title: Mise en œuvre de RTP sur Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
TQID: https://experienceleague.adobe.com/5V3CEgasEJi4zrYoezh8Tt340VGHNNHaliF2wdbBLwY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 202
ht-degree: 1%

---

# Mise en œuvre du RTP sur [!DNL Wordpress] {#implementing-rtp-on-wordpress}

Pour implémenter votre balise [!UICONTROL RTP] suivez les instructions d’installation ci-dessous :

1. Ouvrez le fichier **header.php** de votre **[!DNL WordPress]thème**.

   Vous pouvez utiliser un client FTP pour accéder à votre serveur ou modifier vos fichiers de thème directement à partir du tableau de bord [!DNL WordPress]. L’éditeur de fichiers se trouve sous l’onglet **[!UICONTROL Apparence]** dans le menu de la barre latérale.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Dans la liste des fichiers modèles à droite de l&#39;éditeur de texte, trouvez **header.php** et ouvrez-le.

1. Accédez à **[!UICONTROL Paramètres du compte]**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Sous [!UICONTROL Domaine], recherchez le domaine approprié et cliquez sur **[!UICONTROL Générer la balise]**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copiez la balise RTP JavaScript et collez-la dans les modèles de votre site web.

   a. Assurez-vous qu’il s’agit du premier script situé en-tête de la page, entre les balises **`<head> </head>`**.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Cliquez sur **[!UICONTROL Mettre à jour le fichier]** pour le fichier header.php.

1. Vérifiez qu’il apparaît sur toutes les pages, y compris les pages de destination et les sous-domaines.

   a. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **[!UICONTROL Afficher la page Source].** Recherchez **RTP** pour localiser la balise.
