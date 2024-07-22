---
unique-page-id: 4720149
description: Mise en oeuvre de la méthode RTP sur Wordpress - Documents Marketo - Documentation du produit
title: Mise en oeuvre de RTP sur Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Mise en oeuvre de RTP sur Wordpress {#implementing-rtp-on-wordpress}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Ouvrez le fichier **header.php** de votre **thème WordPress**.

   Vous pouvez utiliser un client FTP pour accéder à votre serveur ou modifier vos fichiers de thème directement à partir du tableau de bord WordPress. Votre éditeur de fichiers se trouve sous l’onglet **Apparence** du menu de la barre latérale.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Dans la liste des fichiers de modèle située à droite de l’éditeur de texte, recherchez **header.php** et ouvrez-le.

1. Accédez à **Paramètres du compte**.

   a. Si vous avez déjà reçu votre balise JavaScript de la part de l’assistance - passez à l’étape 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copiez la balise JavaScript RTP et collez-la dans les modèles de votre site web.

   a. Assurez-vous qu’il s’agit du premier script dans l’en-tête de la page, entre les balises **`<head> </head>`**.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Cliquez sur **Mettre à jour le fichier** pour le fichier header.php.

1. Vérifiez qu’il apparaît sur toutes les pages, y compris les landing pages et les sous-domaines.

   a. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **Afficher le Source de page.** Recherchez **RTP** pour localiser la balise.
