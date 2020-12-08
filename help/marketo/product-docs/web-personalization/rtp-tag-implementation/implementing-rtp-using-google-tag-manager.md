---
unique-page-id: 4720145
description: Implémentation de la procédure RTP à l’aide du gestionnaire de balises Google - Marketo Docs - Documentation du produit
title: Implémentation de RTP à l’aide de Google Tag Manager
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 0%

---


# Implémentation de RTP à l’aide de Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Pour mettre en oeuvre votre RTP, `tag please` suivez les instructions d&#39;installation ci-dessous.

1. Connectez-vous à votre compte Google Tag Manager.

1. Ajoutez une nouvelle balise > Configurations des balises > Balise HTML personnalisée**.** Appelez-le **RTP**.

1. Connectez-vous à votre compte RTP**.**

1. Accédez à Paramètres du compte**.**

   1. Si vous avez déjà reçu votre balise JavaScript de l’assistance, passez à l’étape 6.

      ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer une balise**.

   ** ![](assets/image2014-11-30-15-3a20-3a17.png)

   **

1. Copiez la balise JavaScript RTP et collez-la dans la nouvelle balise **HTML** personnalisée que vous avez créée (étape 1).

1. Cliquez sur **+Ajouter la règle pour déclencher la balise**. Sélectionnez **Toutes les pages**.

1. Cliquez sur **Enregistrer **et [publiez la nouvelle version](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Vérifiez qu’il s’affiche sur tous les `pages, including` landings page et sous-domaines.

   1. Pour ce faire, cliquez avec le bouton droit de la souris sur votre `website’s` page. Accédez à l’élément **Inspect. **Recherchez **RTP **pour localiser la balise.

