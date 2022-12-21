---
unique-page-id: 11385053
description: Déploiement de JavaScript pour Content-AI - Documents Marketo - Documentation du produit
title: Déploiement de JavaScript pour Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# Déploiement de JavaScript pour Content-AI {#deploy-the-javascript-for-content-ai}

Pour utiliser le contenu prédictif, vous devez générer et configurer la balise RTP (Web Personalization).

## Générez un tag
 {#generate-tag}

1. Connectez-vous à votre compte de contenu prédictif. Accédez à **Paramètres du compte**.

   ![](assets/settings-dropdown-account-hands.png)

1. Dans **Configuration des domaines**, recherchez le domaine approprié, puis cliquez sur **Générer une balise**.

   ![](assets/generate-tag.png)

1. Copiez et collez la balise de personnalisation Web dans le HTML de votre site Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiez la balise JavaScript de personnalisation Web et collez-la en tant que premier script dans l’en-tête de vos pages, entre le `<head> </head>` balises. Voir plus détaillé [instructions de mise en oeuvre ici](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Vérifiez que la balise s’affiche sur toutes les pages, y compris les landing pages et les sous-domaines. Pour le vérifier, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **Afficher la source de page** dans un navigateur web. Rechercher : &quot;RTP&quot;.

1. Confirmez que le bouton bascule Balise est défini sur **ON**.
