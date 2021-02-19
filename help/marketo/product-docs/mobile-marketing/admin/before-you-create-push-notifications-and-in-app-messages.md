---
unique-page-id: 11376159
description: Avant de créer des notifications Push et des messages in-app - Documents marketing - Documentation du produit
title: Avant de créer des notifications Push et des messages in-app
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# Avant de créer des notifications Push et des messages in-app {#before-you-create-push-notifications-and-in-app-messages}

La création de notifications Push et de messages in-app n’est pas difficile, mais vous devez disposer de tous les éléments nécessaires pour pouvoir début. L’administrateur du marketing et le développeur d’applications mobiles doivent suivre les étapes ci-dessous pour préparer les intégrations nécessaires.

1. Tout d’abord, l’administrateur marketing [ajoute une application mobile](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. L’administrateur du marketing envoie alors [un fragment de code au développeur](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. Le développeur télécharge le SDK et inclut un extrait de code et d’autres méthodes pour [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) ou [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. Par défaut, les messages in-app sont déclenchés à l’ouverture de votre application. Si vous souhaitez déclencher des messages pour d’autres événements, par exemple lorsqu’une page spécifique est consultée ou qu’un bouton spécifique est appuyé, le développeur doit ajouter des événements personnalisés au code (voir [Événements personnalisés pour les messages in-app](#CustomEvents) ci-dessous).

1. Le développeur [génère la clé d&#39;API du serveur et le numéro de projet pour Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) ou [la certification et le mot de passe pour iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) et l&#39;envoie à l&#39;administrateur du marketing.

1. L’administrateur du marketing configure l’accès aux notifications Push [avec la clé d’API du serveur (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) ou [avec le certificat (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Il est facile pour un administrateur de marketing de vérifier si votre configuration Push est vérifiée. Allez [ici](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Événements personnalisés pour les messages in-app {#custom-events-for-in-app-messages}

Pour la messagerie in-app, le déclencheur d’affichage est défini sur **App Open** par défaut. Si vous souhaitez utiliser des événements personnalisés pour déclencher l’affichage de messages in-app (par exemple, **Les clics Ajoutent au panier**, **Page des paramètres de Vues**), créez une liste de événements et donnez-la au développeur d’applications mobiles. Le développeur ajoute alors les événements personnalisés dans le code. Une fois approuvées, elles apparaissent comme des déclencheurs d’affichage lors de la configuration de votre audience. **Attention** : Le processus d’approbation du codage de événement personnalisé peut prendre un certain temps.

Après avoir effectué toute la préparation des messages in-app et des notifications Push, il est temps de commencer !

>[!MORELIKETHIS]
>
>* [Création d’un message intégré à l’application](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
   >
   >
* [Créer une notification Push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

