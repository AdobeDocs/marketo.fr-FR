---
description: Comment empêcher les auto-vues - Documents Marketo - Documentation du produit
title: Comment empêcher les auto-vues
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Comment Empêcher Les Auto-Vues ? {#how-do-i-prevent-self-views}

L’obtention de faux positifs sur votre suivi des vues peut entraîner des incohérences dans les rapports. Cela se produit souvent lorsque les utilisateurs de Marketo Sales invoquent accidentellement le pixel de suivi à partir de leur client de messagerie (nous appelons cela une auto-visualisation). Vous trouverez ci-dessous quelques conseils pour réduire et même éliminer de manière significative les auto-visions.

## Web (Outlook Web App et Gmail) {#web-outlook-web-app-and-gmail}

Marketo Sales stockera un cookie dans votre navigateur afin d’empêcher le suivi des vues lors de l’ouverture de vos emails à partir d’Outlook Web App et de Gmail. Si vous recevez toujours des vues d’ensemble, nous vous recommandons de procéder comme suit :

* Vérifiez que les cookies sont activés sur votre ordinateur.

* Si vous utilisez un nouvel ordinateur ou un nouvel appareil mobile, vérifiez que vous êtes connecté à l’application web. Cela nous permettra de reconnaître votre ordinateur/appareil à l’avenir.

## Bureau (Windows) {#desktop-windows}

Les vues sont suivies en téléchargeant un petit pixel d’image invisible dans votre client de messagerie. Vous pouvez réduire de manière significative le nombre d’auto-vues dans Outlook en désactivant les images à télécharger automatiquement. Vous trouverez ci-dessous les étapes à suivre.

1. Dans Outlook, cliquez sur **Fichier** dans la barre de menus.

   ![](assets/how-do-i-prevent-self-views-1.png)

1. Cliquez sur **Options**.

   ![](assets/how-do-i-prevent-self-views-2.png)

1. Dans la boîte de dialogue Options Outlook, cliquez sur **Centre de gestion**.

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Sous Microsoft Outlook Trust Center, cliquez sur **Paramètres du Centre de gestion de la confidentialité**.

   ![](assets/how-do-i-prevent-self-views-4.png)

1. Cliquez sur Téléchargement automatique dans le menu de gauche, puis sélectionnez l’option **Ne téléchargez pas automatiquement des images dans un email de HTML ou des éléments RSS** .

   ![](assets/how-do-i-prevent-self-views-5.png)

1. Cliquez sur **OK** dans la boîte de dialogue Centre de gestion de la confidentialité.

   ![](assets/how-do-i-prevent-self-views-6.png)

1. Cliquez sur **OK** dans la boîte de dialogue Options Outlook.

   ![](assets/how-do-i-prevent-self-views-7.png)

## Bureau (Mac) {#desktop-mac}

Les vues sont suivies en téléchargeant un petit pixel d’image invisible dans votre client de messagerie. Vous pouvez réduire de manière significative le nombre d’auto-vues dans Outlook en désactivant les images à télécharger automatiquement. Vous trouverez ci-dessous les étapes à suivre.

1. Dans Outlook, cliquez sur **Outlook** dans la barre de menus, puis sélectionnez **Préférences**.

   ![](assets/how-do-i-prevent-self-views-8.png)

1. Sous Courrier électronique, choisissez **Lire**.

   ![](assets/how-do-i-prevent-self-views-9.png)

1. Sous Sécurité, cliquez sur le **Jamais** bouton radio.

   ![](assets/how-do-i-prevent-self-views-10.png)
