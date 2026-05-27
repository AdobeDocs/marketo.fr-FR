---
unique-page-id: 4720215
description: Découvrez l’implémentation du rtp sur Wordpress Enterprise dans Marketo Engage, y compris l’implémentation du rtp sur Wordpress. Utilisez ce guide pour passer à l’étape suivante.
title: Mise en œuvre de RTP sur Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
TQID: https://experienceleague.adobe.com/S0LvRrD1V6hkWN5L5TlnoaIqcDvXLjfm5do2-1WQTNw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 120
ht-degree: 10%

---

# Mise en œuvre de RTP sur Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

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
