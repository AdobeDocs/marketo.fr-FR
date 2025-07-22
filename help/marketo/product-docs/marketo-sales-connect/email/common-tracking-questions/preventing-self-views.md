---
unique-page-id: 14352540
description: Empêcher les autovisualisations - Documents Marketo - Documentation du produit
title: Empêcher les autovisualisations
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Empêcher les autovisualisations {#preventing-self-views}

## Vue d’ensemble {#overview}

L’obtention de faux positifs sur votre suivi des vues peut entraîner des incohérences dans les rapports. Cela se produit souvent lorsque les utilisateurs de MSC appellent accidentellement le pixel de tracking de leur client de messagerie (nous appelons cela une auto-visualisation). Vous trouverez ci-dessous quelques conseils pour réduire considérablement, voire éliminer, les auto-évaluations.

## Web ([!DNL Outlook Web App] et Gmail) {#web-outlook-web-app-and-gmail}

[!DNL Sales Connect] conservera un cookie dans votre navigateur pour empêcher le suivi des vues lors de l&#39;ouverture de vos e-mails à partir d&#39;Outlook Web App et de Gmail. Si vous recevez toujours des autoévaluations, nous vous recommandons de procéder comme suit :

* Vérifiez que les cookies sont activés sur votre ordinateur.

* Si vous utilisez un nouvel ordinateur ou un nouvel appareil mobile, vérifiez que vous vous êtes connecté à l’application web. Cela nous permettra de reconnaître votre ordinateur/appareil à partir de maintenant.

## Bureau (Windows) {#desktop-windows}

Les vues sont suivies en téléchargeant un petit pixel d’image invisible dans votre client de messagerie. Vous pouvez réduire considérablement le nombre d’auto-vues dans [!DNL Outlook] en désactivant les images à télécharger automatiquement. Vous trouverez ci-dessous les étapes à suivre.

1. Dans [!DNL Outlook], cliquez sur **[!UICONTROL Fichier]** dans la barre de menus.

   ![](assets/win-1.png)

1. Cliquez sur **[!UICONTROL Options]**.

   ![](assets/win-2.png)

1. Dans la boîte de dialogue Options de [!DNL Outlook], cliquez sur **[!UICONTROL Centre de gestion de la confidentialité]**.

   ![](assets/win-3.png)

1. Sous [!UICONTROL Centre de gestion de la confidentialité Microsoft Outlook], cliquez sur **[!UICONTROL Paramètres du Centre de gestion de la confidentialité]**.

   ![](assets/win-4.png)

1. Cliquez sur [!UICONTROL Téléchargement automatique] dans le menu de gauche, puis activez la case à cocher **[!UICONTROL Ne pas télécharger automatiquement les images dans les e-mails ou les éléments RSS d’HTML]**.

   ![](assets/win-5.png)

1. Cliquez sur **[!UICONTROL OK]** dans la boîte de dialogue [!UICONTROL Centre de gestion de la confidentialité].

   ![](assets/win-6.png)

1. Cliquez sur **[!UICONTROL OK]** dans la boîte de dialogue Options de [!DNL Outlook].

   ![](assets/win-6.png)

## Ordinateur de bureau (Mac) {#desktop-mac}

Les vues sont suivies en téléchargeant un petit pixel d’image invisible dans votre client de messagerie. Vous pouvez réduire considérablement le nombre d’auto-vues dans [!DNL Outlook] en désactivant les images à télécharger automatiquement. Vous trouverez ci-dessous les étapes à suivre.

1. Dans [!DNL Outlook], cliquez sur **[!UICONTROL Outlook]** dans la barre de menus et sélectionnez **[!UICONTROL Préférences]**.

   ![](assets/mac-1.png)

1. Sous [!UICONTROL E-mail], choisissez **[!UICONTROL Lecture]**.

   ![](assets/mac-2.png)

1. Sous [!UICONTROL Sécurité], cliquez sur le bouton radio **[!UICONTROL Jamais]**.

   ![](assets/mac-3.png)
