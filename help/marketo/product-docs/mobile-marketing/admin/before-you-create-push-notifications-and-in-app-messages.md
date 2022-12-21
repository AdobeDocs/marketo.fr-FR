---
unique-page-id: 11376159
description: Avant de créer des notifications push et des messages In-App - Documents Marketo - Documentation du produit
title: Avant de créer des notifications push et des messages In-App
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Avant de créer des notifications push et des messages In-App {#before-you-create-push-notifications-and-in-app-messages}

La création de notifications push et de messages in-app n’est pas difficile, mais vous devez tout préparer avant de pouvoir commencer. L’administrateur Marketo et le développeur d’applications mobiles doivent suivre les étapes ci-dessous pour préparer les intégrations nécessaires.

1. Tout d’abord, l’administrateur Marketo [ajoute une application mobile ;](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. L’administrateur Marketo [envoie un fragment de code au développeur.](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. Le développeur télécharge le SDK et inclut des fragments de code et d’autres méthodes pour [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) ou [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. Par défaut, les messages in-app sont déclenchés à l’ouverture de votre application. Si vous souhaitez déclencher des messages pour d’autres événements, par exemple lorsqu’une page spécifique est consultée ou qu’un bouton spécifique est appuyé, le développeur doit ajouter des événements personnalisés au code (voir [Événements personnalisés pour les messages In-App](#CustomEvents) ci-dessous).

1. Le développeur [génère la clé API du serveur et le numéro de projet pour Android.](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) ou [la certification et le mot de passe pour iOS ;](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) et l’envoie à l’administrateur Marketo.

1. L’administrateur Marketo configure l’accès aux notifications push [avec la clé API du serveur (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) ou [avec le certificat (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Il est facile pour un administrateur de Marketo de vérifier si votre configuration push est vérifiée. Allez-y [here](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Événements personnalisés pour les messages In-App {#custom-events-for-in-app-messages}

Pour la messagerie in-app, le déclencheur d’affichage est défini sur **Ouverture d’application** par défaut. Si vous souhaitez utiliser des événements personnalisés pour déclencher l’affichage de messages in-app (par exemple : **Clics Ajouter au panier**, **Page Paramètres des vues**), créez une liste des événements souhaités et donnez-la au développeur de vos applications mobiles. Le développeur ajoute alors les événements personnalisés dans le code. Une fois approuvées, elles apparaissent comme des déclencheurs d’affichage lors de la configuration de votre audience. **Attention**: Le processus d’approbation du codage d’événement personnalisé peut prendre du temps.

Après avoir effectué toute la préparation pour les messages in-app et les notifications push, il est temps de commencer !

>[!MORELIKETHIS]
>
>* [Création d’un message in-app](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Création d’une notification push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

