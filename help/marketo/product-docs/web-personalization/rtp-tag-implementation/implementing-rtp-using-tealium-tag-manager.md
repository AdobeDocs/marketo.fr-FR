---
unique-page-id: 9437340
description: Mise en oeuvre de la procédure RTP à l’aide de Tealium Tag Manager - Documents Marketo - Documentation du produit
title: Mise en oeuvre de la méthode RTP à l’aide de Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Mise en oeuvre de la méthode RTP à l’aide de Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous.

1. Connectez-vous à votre compte Tealium Tag Manager.

1. Accédez à l’onglet Balises et ajoutez la balise Tealium Custom Container située sous l’onglet Divers du marketplace de la marque Balises.

1. Dans le champ Titre, saisissez **Marketo RTP** et cliquez sur **Terminer**.

1. Enregistrez vos modifications.

   >[!NOTE]
   >
   >Il n’est pas encore nécessaire de publier le nouveau conteneur.

1. Une fois le profil enregistré, cliquez sur votre nom/adresse électronique dans le coin supérieur droit de la console Tealium iQ.

1. Dans le menu Admin, cliquez sur **Gérer les modèles** sous Administration de compte.

1. Sélectionnez **Tealium Custom Container : Marketo RTP** dans la liste déroulante pour ouvrir le modèle de balise.

1. Connectez-vous à votre compte RTP.

1. Accédez à Paramètres du compte.

   >[!NOTE]
   >
   >Si vous avez déjà reçu votre balise JavaScript de l’assistance, passez à l’étape 11.

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.

1. Copiez la balise JavaScript RTP et collez-la entre le code de bibliothèque de balises de début et le code de bibliothèque de balises de fin dans votre modèle de profil Tealium.

   >[!NOTE]
   >
   >**Étapes importantes**
   >
   >Supprimez les balises `<!-- RTP tag -->` et `<!-- End of RTP tag -->` du code que vous placez dans ce fichier.
   >
   >Supprimez toutes les balises `<script type='text/javascript'>` et `</script>` du code que vous placez dans ce fichier.

1. **Cliquez sur Enregistrer le modèle de profil** et publiez votre nouveau profil.
