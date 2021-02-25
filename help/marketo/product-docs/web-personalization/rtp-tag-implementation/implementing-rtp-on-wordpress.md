---
unique-page-id: 4720149
description: Implémentation de RTP sur Wordpress - Marketo Docs - Documentation du produit
title: Implémentation de RTP sur Wordpress
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---


# Implémentation de RTP sur Wordpress {#implementing-rtp-on-wordpress}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Ouvrez le fichier **header.php** de votre thème **WordPress**.

   Vous pouvez utiliser un client FTP pour accéder à votre serveur ou modifier vos fichiers de thème directement à partir du tableau de bord WordPress. Votre éditeur de fichiers se trouve sous l&#39;onglet **Apparence** du menu de la barre latérale.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Dans la liste des fichiers de modèle à droite de l’éditeur de texte, recherchez **header.php** et ouvrez-le.

1. Accédez à **Paramètres du compte**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copiez la balise JavaScript RTP et collez-la dans vos modèles de site Web.

   a. Assurez-vous qu’il s’agit du premier script dans l’en-tête de la page, entre les balises **`<head> </head>`**.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Cliquez sur **Mettre à jour le fichier** pour le fichier header.php.

1. Vérifiez qu’il s’affiche sur toutes les pages, y compris les landings page et sous-domaines.

   a. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site Web. Accédez à **Source de la page de Vue.** Recherchez  **** RTP pour localiser la balise.
