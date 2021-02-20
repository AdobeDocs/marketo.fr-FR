---
unique-page-id: 11385053
description: Déploiement de JavaScript pour Content-AI - Documentation sur le marketing - Documentation du produit
title: Déploiement de JavaScript pour Content-AI
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# Déploiement du code JavaScript pour Content-AI {#deploy-the-javascript-for-content-ai}

Pour utiliser le contenu prédictif, vous devez générer et configurer la balise RTP (Personnalisation Web).

## Générer la balise {#generate-tag}

1. Connectez-vous à votre compte Contenu prédictif. Accédez à **Paramètres du compte**.

   ![](assets/settings-dropdown-account-hands.png)

1. Dans **Configuration du domaine**, recherchez le domaine approprié et cliquez sur **Générer la balise**.

   ![](assets/generate-tag.png)

1. Copiez et collez la balise Personnalisation Web dans le code HTML de votre site Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiez la balise JavaScript de personnalisation Web et collez-la en tant que premier script dans l’en-tête de vos pages, entre les balises `<head> </head>`. Voir les [instructions d&#39;implémentation plus détaillées ici](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Vérifiez que la balise s’affiche sur toutes les pages, y compris les landings page et sous-domaines. Pour vérifier cette information, cliquez avec le bouton droit de la souris sur la page de votre site Web. Accédez à **Vue Page Source** dans un navigateur Web. Rechercher : &quot;RTP&quot;.

1. Vérifiez que la bascule Balise est définie sur **ON**.
