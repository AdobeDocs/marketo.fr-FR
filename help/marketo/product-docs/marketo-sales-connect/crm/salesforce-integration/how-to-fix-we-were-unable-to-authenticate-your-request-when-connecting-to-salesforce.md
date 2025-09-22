---
unique-page-id: 14352484
description: Comment corriger « Nous n’avons pas pu authentifier votre demande » lors de la connexion à Salesforce - Documents Marketo - Documentation du produit
title: Comment corriger l’erreur « Nous n’avons pas pu authentifier votre demande » lors de la connexion à Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 8%

---

# Comment corriger « Nous n’avons pas pu authentifier votre demande » lors de la connexion à [!DNL Salesforce] {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si vous recevez le message d’erreur « Nous n’avons pas pu authentifier votre requête » lors de la tentative de connexion de [!DNL Sales Connect] à [!DNL Salesforce], il se peut qu’il y ait une restriction sur votre accès à l’API de [!DNL Salesforce]. Vérifiez auprès de votre administrateur [!DNL Salesforce] que les éléments suivants sont en place.

## Activer l’API dans les autorisations utilisateur {#enable-api-in-user-permissions}

1. Demandez à un administrateur [!DNL Salesforce] de se connecter à SFDC.
1. Sélectionnez **[!UICONTROL Configuration]**.
1. Sélectionnez **[!UICONTROL Gérer les utilisateurs]**.
1. Sélectionnez **[!UICONTROL Profils]**.
1. Recherchez le profil sous lequel se trouvent les utilisateurs de ToutApp et cliquez sur **[!UICONTROL Modifier]**.
1. Faites défiler jusqu’à **[!UICONTROL Autorisations d’administration]** et assurez-vous que **[!UICONTROL API activée]** est coché.

## Vérifier si [!DNL Salesforce] bloque la [!DNL Sales Connect] de la connexion {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Demandez à un administrateur [!DNL Salesforce] de se connecter à SFDC.
1. Sélectionnez **[!UICONTROL Configuration]**.
1. Sélectionnez **[!UICONTROL Gérer Les Applications]**.
1. Sélectionnez **[!UICONTROL Utilisation d’OAuth pour les applications connectées]**.
1. Assurez-vous que [!DNL Sales Connect] indique « [!UICONTROL Block] » en regard de celui-ci. Si vous voyez « [!UICONTROL Débloquer] », cliquez sur le bouton pour débloquer l’accès de [!DNL Sales Connect] à [!DNL Salesforce].
