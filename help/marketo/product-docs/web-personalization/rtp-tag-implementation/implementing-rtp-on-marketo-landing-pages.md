---
unique-page-id: 4720151
description: Implémentation de RTP sur les Landings page marketing - Docs marketing - Documentation du produit
title: Implémentation de RTP sur les Landings page marketing
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Implémentation de RTP sur les Landings page marketing {#implementing-rtp-on-marketo-landing-pages}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Rendez-vous au **Design Studio.** Ouvrez l&#39;élément à modifier. Sélectionner des actions **** de modèle, sélectionner **Modifier le brouillon**

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Effectuez les modifications de modèle dans l’onglet Source **** HTML.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Dans votre compte RTP, accédez à Paramètres du compte**.**

1. Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer une balise**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copiez la balise JavaScript RTP et collez-la dans tous vos modèles de landing page entre les **`<head> </head>`** balises.
1. Cliquez sur **Enregistrer** et **Fermer** la fenêtre.
1. De retour dans **Design Studio**, approuvez le landing page des actions **de** modèle, cliquez sur **Approuver**.\
   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Enfin, vous devrez **réapprouver** tout landing page utilisant ce modèle pour que les modifications apportées au modèle soient prises en compte. Vous pouvez les réapprouver tous en même temps à partir de la section Landings page principaux.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Vérifiez qu’il s’affiche sur tous les `pages including` landings page et sous-domaines.

   Pour ce faire, cliquez avec le bouton droit de la souris sur votre `website’s` page. Accédez à la source de la page de **Vue.** Recherchez **RTP** pour localiser la balise.
