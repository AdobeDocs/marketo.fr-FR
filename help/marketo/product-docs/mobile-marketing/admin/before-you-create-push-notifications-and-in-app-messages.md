---
unique-page-id: 11376159
description: Avant de créer des notifications push et des messages In-App - Documents Marketo - Documentation du produit
title: Avant de créer des notifications push et des messages In-App
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Avant de créer des notifications push et des messages In-App {#before-you-create-push-notifications-and-in-app-messages}

La création de notifications push et de messages in-app n’est pas difficile, mais vous devez tout avoir prêt avant de pouvoir commencer. L’administrateur Marketo et le développeur d’applications mobiles doivent suivre les étapes ci-dessous pour préparer les intégrations nécessaires.

1. Tout d’abord, l’administrateur Marketo [ajoute une application mobile](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. L’administrateur Marketo [envoie ensuite un fragment de code au développeur](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. Le développeur télécharge le SDK, ainsi qu’un extrait de code et d’autres méthodes, pour [Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) ou [iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios).

1. Par défaut, les messages in-app sont déclenchés à l’ouverture de votre application. Si vous souhaitez déclencher des messages pour d’autres événements, par exemple lorsqu’une page particulière est consultée ou qu’un bouton spécifique est enfoncé, le développeur doit ajouter des événements personnalisés au code (voir [Événements personnalisés pour les messages In-App](#CustomEvents) ci-dessous).

1. Le développeur [génère la clé API du serveur et le numéro de projet pour Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) ou [ la certification et le mot de passe pour iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios) et l’envoie à l’administrateur Marketo.

1. L’administrateur Marketo configure l’accès aux notifications push [avec la clé API du serveur (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) ou [avec le certificat (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Il est facile pour un administrateur Marketo de vérifier si votre configuration push est vérifiée. Allez [ici](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Événements personnalisés pour les messages In-App {#custom-events-for-in-app-messages}

Pour la messagerie in-app, le déclencheur d’affichage est défini sur **[!UICONTROL App Open]** par défaut. Si vous souhaitez utiliser des événements personnalisés pour déclencher l’affichage de messages in-app (par exemple, **Clics ajouter au panier**, **Page des paramètres d’affichage**), créez une liste d’événements souhaités et remettez-la à votre développeur ou développeuse d’applications mobiles. Le développeur ajoute ensuite les événements personnalisés dans le code. Une fois approuvés, ils apparaissent comme des déclencheurs d’affichage lors de la configuration de votre audience. **Attention** : le processus d’approbation du codage d’événement personnalisé peut prendre un certain temps.

Une fois toute votre préparation aux messages in-app et aux notifications push terminée, il est temps de commencer.

>[!MORELIKETHIS]
>
>* [Créer un message In-App](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Créer une notification push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
