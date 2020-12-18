---
unique-page-id: 11385053
description: Déploiement de JavaScript pour Content-AI - Documentation sur le marketing - Documentation du produit
title: Déploiement de JavaScript pour Content-AI
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Déploiement du code JavaScript pour Content-AI {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>Selon la date d’achat, votre abonnement Marketo peut inclure soit du contenu prédictif ou du contenu `<sup>AI</sup>`. Pour les utilisateurs de contenu prédictif, Marketo active les fonctionnalités Content`<sup>AI</sup>` Analytics jusqu’au 30 avril 2018. Pour conserver ces fonctionnalités au-delà de cette date, contactez votre responsable de succès client Marketo pour effectuer la mise à niveau vers Marketo Content`<sup>AI</sup>`.

Pour utiliser le contenu prédictif, vous devez générer et configurer votre RTP (Personnalisation Web) `tag.`

## Générer la balise {#generate-tag}

1. Connectez-vous à votre compte Contenu prédictif. Accédez à **Paramètres du compte**.

   ![](assets/settings-dropdown-account-hands.png)

1. Dans **Configuration du domaine**, recherchez le domaine approprié et cliquez sur **Générer la balise.**

   ![](assets/generate-tag.png)

1. Copiez et collez la balise Personnalisation Web dans le code HTML de votre site Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiez la balise JavaScript de personnalisation Web et collez-la en tant que premier script dans l’en-tête de vos pages, entre les balises `<head> </head>`. Voir les [instructions d&#39;implémentation plus détaillées ici](http://docs.marketo.com/display/docs/rtp+tag+implementation) [.](http://pages2.marketo.com/rtp-implementation.html)

1. Vérifiez que la balise s’affiche sur toutes les pages, y compris les landings page et sous-domaines. Pour vérifier cette valeur, cliquez avec le bouton droit de la souris sur votre `website’s` page. Accédez à **Vue Page Source** dans un navigateur Web. Rechercher : &quot;RTP&quot;.
1. Vérifiez que la bascule Balise est définie sur **ON**.

