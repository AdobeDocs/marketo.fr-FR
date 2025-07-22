---
unique-page-id: 11385053
description: Déploiement de JavaScript for Content-AI - Documents Marketo - Documentation du produit
title: Déploiement de JavaScript for Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# Déploiement de JavaScript for Content-AI {#deploy-the-javascript-for-content-ai}

Pour utiliser le contenu prédictif, vous devez générer et configurer la balise RTP (Web Personalization).

## Générez un tag
 {#generate-tag}

1. Connectez-vous à votre compte de contenu prédictif . Accédez à **[!UICONTROL Paramètres du compte]**.

   ![](assets/settings-dropdown-account-hands.png)

1. Dans **[!UICONTROL Configuration du domaine]**, recherchez le domaine approprié et cliquez sur **[!UICONTROL Générer la balise]**.

   ![](assets/generate-tag.png)

1. Copiez et collez la balise Web Personalization dans l’HTML de votre site Web.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copiez la balise Web Personalization JavaScript et collez-la en tant que premier script dans l’en-tête de vos pages, entre les balises `<head> </head>`. Voir les instructions d’implémentation plus détaillées [ici](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Vérifiez que la balise s’affiche sur toutes les pages, y compris les pages de destination et les sous-domaines. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **[!UICONTROL Afficher la page Source]** dans un navigateur web. Recherche : « RTP ».

1. Vérifiez que le bouton (bascule) de la Balise est défini sur **[!UICONTROL ON]**.
