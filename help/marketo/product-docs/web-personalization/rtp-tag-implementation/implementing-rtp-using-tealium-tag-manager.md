---
unique-page-id: 9437340
description: Découvrez l’implémentation de rtp à l’aide de tealium tag manager dans Marketo Engage, y compris l’implémentation de rtp à l’aide de dnl. Utilisez ce guide pour passer à l’étape suivante.
title: Mise en œuvre de RTP à l’aide de Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
TQID: https://experienceleague.adobe.com/zMs2Dii5RERdH8tKb86a6EhxXUx2IpbZkDOCklUvvY4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 233
ht-degree: 3%

---

# Implémentation du RTP à l’aide du gestionnaire de balises [!DNL Tealium] {#implementing-rtp-using-tealium-tag-manager}

Pour implémenter votre balise RTP, suivez les instructions d’installation ci-dessous.

1. Connectez-vous à votre compte [!DNL Tealium] Tag Manager.

1. Accédez à l’onglet [!UICONTROL Balises] et ajoutez la balise de conteneur personnalisé [!UICONTROL Tealium], située sous l’onglet [!UICONTROL Divers] de la marketplace Balises.

1. Dans le champ [!UICONTROL Titre], saisissez **Marketo RTP** puis cliquez sur **[!UICONTROL Terminer]**.

1. Enregistrez vos modifications.

   >[!NOTE]
   >
   >Il n’est pas encore nécessaire de publier le nouveau conteneur.

1. Une fois le profil enregistré, cliquez sur votre nom/adresse e-mail dans le coin supérieur droit de la console Tealium iQ.

1. Dans le menu [!UICONTROL Admin], cliquez sur **[!UICONTROL Gérer les modèles]** sous [!UICONTROL Administrateur de compte].

1. Sélectionnez **[!UICONTROL Conteneur personnalisé Tealium] : Marketo RTP** dans la liste déroulante pour ouvrir le modèle de balise.

1. Connectez-vous à votre compte RTP.

1. Accédez à [!UICONTROL &#x200B; Paramètres du compte &#x200B;].

   >[!NOTE]
   >
   >Si vous avez déjà reçu votre balise JavaScript de l’assistance, passez à l’étape 11.

1. Sous Domain, recherchez le domaine approprié et cliquez sur **[!UICONTROL Generate Tag]**.

1. Copiez la balise RTP JavaScript et collez-la entre [!UICONTROL Code de la bibliothèque de balises de début] et [!UICONTROL Code de la bibliothèque de balises de fin] dans votre modèle de profil Tealium.

   >[!NOTE]
   >
   >**Étapes importantes**
   >
   >Supprimez les balises `<!-- RTP tag -->` et `<!-- End of RTP tag -->` du code que vous placez dans ce fichier.
   >
   >Supprimez toutes les balises `<script type='text/javascript'>` et `</script>` du code que vous placez dans ce fichier.

1. Cliquez sur **[!UICONTROL Enregistrer le modèle de profil]** et publiez votre nouveau profil.
