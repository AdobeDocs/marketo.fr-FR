---
unique-page-id: 4720215
description: Mise en oeuvre de la procédure RTP sur Wordpress Enterprise - Documents Marketo - Documentation du produit
title: Mise en oeuvre de la méthode RTP sur Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Mise en oeuvre de la méthode RTP sur Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Accédez à **Paramètres du compte**.

   a. Si vous avez déjà reçu votre balise JavaScript de la part de l’assistance - passez à l’étape 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copiez la balise JavaScript RTP.

1. Connectez-vous à votre compte WordPress en tant qu’utilisateur administrateur.

   a. Sous **Apparence**, accédez à **JavaScript personnalisé**.
b. Collez la balise JavaScript RTP juste après le code existant.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Lorsque vous collez le code, EXCLUEZ les balises suivantes :
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >Insérez le script lui-même UNIQUEMENT.

1. Cliquez sur **Mettre à jour**.
