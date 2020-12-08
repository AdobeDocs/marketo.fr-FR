---
unique-page-id: 4720149
description: Implémentation de RTP sur Wordpress - Marketo Docs - Documentation du produit
title: Implémentation de RTP sur Wordpress
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# Implémentation de RTP sur Wordpress {#implementing-rtp-on-wordpress}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Ouvrez le fichier **header.php** de votre thème **** WordPress.

   Vous pouvez utiliser un client FTP pour accéder à votre serveur ou modifier vos fichiers de thème directement à partir du tableau de bord WordPress. L’éditeur de fichiers se trouve sous l’onglet **Aspect** du menu de la barre latérale.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Dans la liste des fichiers de modèle à droite de l’éditeur de texte, recherchez **header.php** et ouvrez-le.
1. Accédez à Paramètres du **compte.**

   Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer une balise**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copiez la balise JavaScript RTP et collez-la dans vos modèles de site Web.

   Assurez-vous qu’il s’agit du premier script dans l’en-tête de la page, entre les **`<head> </head>`** balises.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Cliquez sur **Mettre à jour le fichier** pour le fichier header.php.
1. Vérifiez qu’il s’affiche sur tous les `pages including` landings page et sous-domaines.

   Pour ce faire, cliquez avec le bouton droit de la souris sur votre `website’s` page. Accédez à la source de la page de **Vue.** Recherchez **RTP** pour localiser la balise.
