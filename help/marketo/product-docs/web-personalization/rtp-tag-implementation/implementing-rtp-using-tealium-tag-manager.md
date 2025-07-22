---
unique-page-id: 9437340
description: Mise en œuvre du RTP à l’aide de Tealium Tag Manager - Documents Marketo - Documentation du produit
title: Mise en œuvre du RTP à l’aide de Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 1%

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

1. Accédez à [!UICONTROL  Paramètres du compte ].

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
