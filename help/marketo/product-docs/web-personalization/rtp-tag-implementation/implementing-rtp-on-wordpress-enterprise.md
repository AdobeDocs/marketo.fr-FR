---
unique-page-id: 4720215
description: Mise en oeuvre de RTP sur Wordpress Enterprise - Marketo Docs - Documentation sur les produits
title: Implémentation de RTP sur Wordpress Enterprise
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# Implémentation de RTP sur Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Accédez à **Paramètres du compte**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copiez la balise JavaScript RTP.

1. Connectez-vous à votre compte WordPress en tant qu’utilisateur administrateur.

   a. Sous **Apparence**, accédez à **JavaScript personnalisé**.
b. Collez la balise Javascript RTP juste après le code existant.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Lorsque vous collez le code EXCLURE les balises suivantes :
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >
   >Insérez le script lui-même SEULEMENT.

1. Cliquez sur **Mettre à jour**.
