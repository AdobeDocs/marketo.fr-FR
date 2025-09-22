---
unique-page-id: 4720149
description: Mise en œuvre du RTP sur Wordpress - Documents Marketo - Documentation du produit
title: Mise en œuvre de RTP sur Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 2%

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

   a. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **[!UICONTROL Afficher la page Source].** Rechercher **RTP** pour localiser la balise.
