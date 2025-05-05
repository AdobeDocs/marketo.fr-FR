---
unique-page-id: 11385053
description: Déploiement de JavaScript for Content-AI - Marketo Docs - Documentation du produit
title: Déploiement de JavaScript pour Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# Déploiement de JavaScript pour Content-AI {#deploy-the-javascript-for-content-ai}

Pour utiliser le contenu prédictif, vous devez générer et configurer la balise RTP (Web Personalization).

## Générez un tag {#generate-tag}

1. Connectez-vous à votre compte de contenu prédictif. Accédez à **Paramètres du compte**.

   ![](assets/settings-dropdown-account-hands.png)

1. Dans **Domain Configuration**, recherchez le domaine approprié et cliquez sur **Generate Tag**.

   ![](assets/generate-tag.png)

1. Copiez et collez la balise Web Personalization dans l’HTML de votre site Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiez la balise Web Personalization JavaScript et collez-la comme premier script dans l’en-tête de vos pages, entre les balises `<head> </head>`. Voir des [instructions de mise en oeuvre plus détaillées ici](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Vérifiez que la balise s’affiche sur toutes les pages, y compris les landing pages et les sous-domaines. Pour le vérifier, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **Afficher le Source de page** dans un navigateur web. Recherche : &quot;RTP&quot;.

1. Confirmez que le bouton bascule Tag est défini sur **ON**.
