---
unique-page-id: 9437340
description: Implémentation de la procédure à main levée à l’aide du gestionnaire de balises Tealium - Docs marketing - Documentation du produit
title: Implémentation de RTP à l’aide de Tealium Tag Manager
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Implémentation de RTP à l’aide de Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d&#39;installation ci-dessous.

1. Connectez-vous à votre compte Tealium Tag Manager.
1. Accédez à l’onglet Balises et ajoutez la balise de Conteneur personnalisée Tealium, située sous l’onglet Divers du marché Balises.
1. Dans le champ Titre, saisissez **Marketo RTP** et cliquez sur **Terminer**.
1. Enregistrez vos modifications.

   >[!NOTE]
   >
   >Il n&#39;est pas encore nécessaire de publier le nouveau conteneur.

1. Une fois le profil enregistré, cliquez sur votre nom/adresse électronique dans le coin supérieur droit de la console iQ Tealium.
1. Dans le menu Admin, cliquez sur **Gérer les modèles** sous Administration de comptes.
1. Sélectionnez **Conteneur personnalisé Tealium : Marketo RTP** à partir de la liste déroulante pour ouvrir le modèle de balise.
1. Connectez-vous à votre compte RTP.
1. Accédez à Paramètres du compte.

   >[!NOTE]
   >
   >Si vous avez déjà reçu votre balise JavaScript de l’assistance, passez à l’étape 11.

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.
1. Copiez la balise JavaScript RTP et collez-la entre le code de la bibliothèque de balises de Début et le code de la bibliothèque de balises de fin dans votre modèle de Profil Tealium.

   >[!NOTE]
   >
   >**Etapes importantes**
   >
   >Supprimez les balises `<!-- RTP tag -->` et `<!-- End of RTP tag -->` du code que vous placez dans ce fichier.
   >
   >Supprimez toutes les balises `<script type='text/javascript'>` et `</script>` du code que vous placez dans ce fichier.

1. **Cliquez sur Enregistrer le** modèle de Profil et publiez votre nouveau profil.

