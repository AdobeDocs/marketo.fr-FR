---
unique-page-id: 1900579
description: Désactiver le suivi d’un lien de courrier électronique - Documents Marketo - Documentation du produit
title: Désactiver le suivi d’un lien de courrier électronique
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Désactiver le suivi d’un lien de courrier électronique {#disable-tracking-for-an-email-link}

Parfois, vous ne souhaitez pas activer la variable **URL de suivi Marketo** sur un lien d’un email. Cela s’avère utile lorsque la page de destination ne prend pas en charge les paramètres d’URL et peut entraîner la rupture du lien.

1. Sélectionnez votre adresse électronique et cliquez sur **Modifier le brouillon**.

   ![](assets/one-7.png)

1. Double-cliquez sur la section modifiable contenant le lien.

   ![](assets/two-6.png)

1. Cliquez sur le lien en question, puis sur le lien **Insérer/Modifier un lien** bouton .

   ![](assets/three-6.png)

1. Dans la fenêtre contextuelle Modifier le lien , désélectionnez la case **Suivi du lien** .

   ![](assets/four-4.png)

1. Vous remarquerez que la variable **Case Inclure mkt_tok** disparaît. Cliquez sur **Appliquer**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Décocher juste **Inclure mkt_tok** permettra toujours le suivi du lien, mais après la redirection, l’URL de destination n’inclura pas le paramètre de chaîne de requête mkt_tok . Ce paramètre est utilisé par les landing pages Marketo et Munchkin pour assurer un suivi correct des activités des personnes (comme lorsqu’une personne se désabonne d’un email). Évitez d’utiliser cette fonctionnalité, sauf si vous constatez un comportement bizarre sur votre site web en raison du paramètre présent.

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Vous souhaitez désactiver le suivi des clics pour un lien dans un email **modèle**? Utilisez ce format :
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >Si vous avez besoin d’aide pour mettre en oeuvre cette méthode, consultez votre développeur web.

Beau ! Vous avez maintenant désactivé le suivi d’un lien.
