---
unique-page-id: 4720145
description: Mise en oeuvre de la procédure RTP à l’aide de Google Tag Manager - Documents Marketo - Documentation du produit
title: Mise en oeuvre de la méthode RTP à l’aide de Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Mise en oeuvre de la méthode RTP à l’aide de Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous.

1. Connectez-vous à votre compte Gestionnaire de balises Google.

1. Ajoutez une nouvelle balise > Configurations de balises > Balise d’HTML personnalisée&#x200B;**.** Appelez-le **RTP**.

1. Connectez-vous à votre compte RTP&#x200B;**.**

1. Accédez à **Paramètres du compte**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance, passez à l’étape 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copiez la balise JavaScript RTP et collez-la dans la nouvelle balise **HTML personnalisé** que vous avez créée (étape 1).

1. Cliquez sur **+Ajouter une règle pour déclencher la balise**. Sélectionnez **Toutes les pages**.

1. Cliquez sur **Enregistrer** et [publier la nouvelle version](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Vérifiez qu’il apparaît sur toutes les pages, y compris les landing pages et les sous-domaines.

   a. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **Inspect Element**, recherchez **RTP** pour localiser la balise.
