---
unique-page-id: 4720151
description: Mise en oeuvre de la procédure RTP sur les pages d’entrée Marketo - Documents Marketo - Documentation du produit
title: Implémentation de la méthode RTP sur les pages d’entrée Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Implémentation de la méthode RTP sur les pages d’entrée Marketo {#implementing-rtp-on-marketo-landing-pages}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Accédez à **Design Studio.** Ouvrez l’élément que vous souhaitez modifier. Sélectionnez **Actions de modèle**, sélectionnez **Modifier le brouillon**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Apportez vos modifications de modèle dans l’onglet **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Dans votre compte RTP, accédez à **Paramètres du compte**.

   a. Si vous avez déjà reçu votre balise JavaScript de la part de l’assistance - passez à l’étape 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copiez la balise JavaScript RTP et collez-la dans tous vos modèles de landing page entre les balises **`<head> </head>`**.

1. Cliquez sur **Enregistrer** et **Fermer** dans la fenêtre.

1. De retour dans **Design Studio**, approuvez la page d’entrée à partir des **actions de modèle**, cliquez sur **Approve** (Approuver).

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Enfin, vous devrez **réapprouver** toutes les landing pages utilisant ce modèle pour que les modifications du modèle soient prises en compte. Vous pouvez tous les réapprouver en même temps à partir de la section Pages d’entrée principale.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Vérifiez qu’il apparaît sur toutes les pages, y compris les landing pages et les sous-domaines.

   Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **Afficher le Source de page.** Recherchez **RTP** pour localiser la balise.
