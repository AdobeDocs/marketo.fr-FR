---
unique-page-id: 4720215
description: Mise en œuvre du RTP sur Wordpress Enterprise - Documents Marketo - Documentation du produit
title: Mise en œuvre du RTP sur Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 1%

---

# Mise en œuvre du RTP sur Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Pour implémenter votre balise [!UICONTROL RTP] suivez les instructions d’installation ci-dessous :

1. Accédez à **[!UICONTROL Paramètres du compte]**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Sous [!UICONTROL Domaine], recherchez le domaine approprié et cliquez sur **[!UICONTROL Générer la balise]**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copiez la balise RTP JavaScript.

1. Connectez-vous à votre compte [!DNL WordPress] en tant qu’utilisateur administrateur

   a. Sous **[!UICONTROL Apparence]**, accédez à **[!UICONTROL Custom JavaScript]**.
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

1. Cliquez sur **[!UICONTROL Mettre à jour]**.
