---
unique-page-id: 1900579
description: Désactiver le suivi d'un lien de courriel - Documents marketing - Documentation du produit
title: Désactiver le suivi d’un lien de courriel
translation-type: tm+mt
source-git-commit: 29eb4c833c128c37849260f0c554144c237ab28e
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Désactiver le suivi d’un lien de courriel {#disable-tracking-for-an-email-link}

Il arrive que vous ne souhaitiez pas activer l’URL **de suivi du** marketing sur un lien d’un courrier électronique. Cela s’avère utile lorsque la page de destination ne prend pas en charge les paramètres d’URL et peut entraîner la rupture d’un lien.

1. Sélectionnez votre adresse électronique et cliquez sur **Modifier** **le brouillon**.

   ![](assets/one-7.png)

1. Cliquez avec le doublon sur la section modifiable qui contient le lien.

   ![](assets/two-6.png)

1. Cliquez sur le lien en question, puis sur le bouton **Insérer/Modifier le lien** .

   ![](assets/three-6.png)

1. Dans la fenêtre contextuelle Modifier le lien, décochez la case **Suivi du lien** .

   ![](assets/four-4.png)

1. Vous remarquerez que la zone **** Inclure mkt_tok disparaît. Cliquez sur **Appliquer**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Si vous désactivez la case à cocher **Inclure uniquement mkt_tok** , le lien sera toujours suivi, mais après la redirection, l’URL de destination n’inclura pas le paramètre de chaîne de requête mkt_tok. Ce paramètre est utilisé par les Landings page Marketo et Munchkin pour assurer un suivi correct des activités de personne (comme lorsqu&#39;une personne se désabonne d&#39;un courrier électronique). Evitez d’utiliser cette fonctionnalité à moins que vous ne voyiez un comportement bizarre sur votre site Web en raison de la présence du paramètre.

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Voulez-vous désactiver le suivi des clics pour un lien dans un **modèle**de courrier électronique ? Utilisez ce format :
   >`<a class="mktNoTrack" href="http://www.mywebsite.com">This link does not have tracking</a>`\
   >Si vous avez besoin d’aide pour implémenter cette méthode, contactez votre développeur Web.

Sympa ! Vous avez maintenant désactivé le suivi pour un lien.
