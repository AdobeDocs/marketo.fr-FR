---
description: Comment empêcher les autovisualisations ? - Documents Marketo - Documentation du produit
title: Comment empêcher les autoévaluations ?
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Comment Empêcher Les Auto-Analyses ? {#how-do-i-prevent-self-views}

L’obtention de faux positifs sur votre suivi des vues peut entraîner des incohérences dans les rapports. Cela se produit souvent lorsque les utilisateurs d’[!DNL Marketo Sales] appellent accidentellement le pixel de tracking de leur client de messagerie (nous appelons cela une auto-visualisation). Vous trouverez ci-dessous quelques conseils pour réduire considérablement, voire éliminer, les auto-évaluations.

## Web ([!DNL Outlook] Web App et Gmail) {#web-outlook-web-app-and-gmail}

[!DNL Marketo Sales] stockera un cookie dans votre navigateur pour empêcher le suivi des vues lors de l&#39;ouverture de vos e-mails à partir de [!DNL Outlook] Web App et de Gmail. Si vous recevez toujours des autoévaluations, nous vous recommandons de procéder comme suit :

* Vérifiez que les cookies sont activés sur votre ordinateur.

* Si vous utilisez un nouvel ordinateur ou un nouvel appareil mobile, vérifiez que vous vous êtes connecté à l’application web. Cela nous permettra de reconnaître votre ordinateur/appareil à partir de maintenant.

## Bureau (Windows) {#desktop-windows}

Les vues sont suivies en téléchargeant un petit pixel d’image invisible dans votre client de messagerie. Vous pouvez réduire considérablement le nombre d’auto-vues dans [!DNL Outlook] en désactivant les images à télécharger automatiquement. Vous trouverez ci-dessous les étapes à suivre.

1. Dans Outlook, cliquez sur **[!UICONTROL Fichier]** dans la barre de menus.

   ![](assets/how-do-i-prevent-self-views-1.png)

1. Cliquez sur **[!UICONTROL Options]**.

   ![](assets/how-do-i-prevent-self-views-2.png)

1. Dans la boîte de dialogue Options de [!DNL Outlook], cliquez sur **[!UICONTROL Centre de gestion de la confidentialité]**.

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Sous Microsoft [!DNL Outlook] Trust Center, cliquez sur **[!UICONTROL Paramètres du Centre de gestion de la confidentialité]**.

   ![](assets/how-do-i-prevent-self-views-4.png)

1. Cliquez sur [!UICONTROL Téléchargement automatique] dans le menu de gauche, puis activez la case à cocher **[!UICONTROL Ne pas télécharger automatiquement les images dans les e-mails ou les éléments RSS d’HTML]**.

   ![](assets/how-do-i-prevent-self-views-5.png)

1. Cliquez sur **[!UICONTROL OK]** dans la boîte de dialogue [!UICONTROL Centre de gestion de la confidentialité].

   ![](assets/how-do-i-prevent-self-views-6.png)

1. Cliquez sur **[!UICONTROL OK]** dans la boîte de dialogue Options de [!DNL Outlook].

   ![](assets/how-do-i-prevent-self-views-7.png)

## Ordinateur de bureau (Mac) {#desktop-mac}

Les vues sont suivies en téléchargeant un petit pixel d’image invisible dans votre client de messagerie. Vous pouvez réduire considérablement le nombre d’auto-vues dans [!DNL Outlook] en désactivant les images à télécharger automatiquement. Vous trouverez ci-dessous les étapes à suivre.

1. Dans [!DNL Outlook], cliquez sur **[!UICONTROL Outlook]** dans la barre de menus et sélectionnez **[!UICONTROL Préférences]**.

   ![](assets/how-do-i-prevent-self-views-8.png)

1. Sous [!UICONTROL E-mail], choisissez **[!UICONTROL Lecture]**.

   ![](assets/how-do-i-prevent-self-views-9.png)

1. Sous [!UICONTROL Sécurité], cliquez sur le bouton radio **[!UICONTROL Jamais]**.

   ![](assets/how-do-i-prevent-self-views-10.png)
