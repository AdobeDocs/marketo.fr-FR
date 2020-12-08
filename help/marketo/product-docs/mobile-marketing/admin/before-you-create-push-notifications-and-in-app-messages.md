---
unique-page-id: 11376159
description: Avant de créer des notifications Push et des messages in-app - Documents marketing - Documentation du produit
title: Avant de créer des notifications Push et des messages in-app
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Avant de créer des notifications Push et des messages in-app {#before-you-create-push-notifications-and-in-app-messages}

La création de notifications Push et de messages in-app n’est pas difficile, mais vous devez disposer de tous les éléments nécessaires pour pouvoir début. L’administrateur du marketing et le développeur d’applications mobiles doivent suivre les étapes ci-dessous pour préparer les intégrations nécessaires.

1. Tout d’abord, l’administrateur du marketing [ajoute une application mobile.](add-a-mobile-app.md)
1. L’administrateur du marketing [envoie ensuite un fragment de code au développeur.](send-sdk-code-to-a-developer.md)
1. Le développeur télécharge le SDK et inclut des extraits de code et d’autres méthodes pour [Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) ou [iOS.](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)
1. Par défaut, les messages in-app sont déclenchés à l’ouverture de votre application. Si vous souhaitez déclencher des messages pour d’autres événements, par exemple lorsqu’une page spécifique est consultée ou qu’un bouton spécifique est appuyé, le développeur doit ajouter des événements personnalisés au code (voir Événements [personnalisés pour les messages](#CustomEvents) in-app ci-dessous).
1. Le développeur [génère la clé d’API du serveur et le numéro de projet pour Android](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) ou [la certification et le mot de passe pour iOS](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) et l’envoie à l’administrateur du marketing.
1. L’administrateur du marketing configure l’accès aux notifications Push [avec la clé d’API du serveur (Android)](configure-mobile-app-android-push-access.md) ou [avec le certificat (iOS).](configure-mobile-app-ios-push-access.md)

>[!TIP]
>
>Il est facile pour un administrateur de marketing de vérifier si votre configuration Push est vérifiée. Allez [ici](verify-push-configuration.md).

## Événements personnalisés pour les messages in-app {#custom-events-for-in-app-messages}

Pour les messages in-app, le déclencheur d’affichage est défini par défaut sur **App Open** (Ouvrir l’application). Si vous souhaitez utiliser des événements personnalisés pour déclencher l’affichage de messages in-app (par exemple, **Clics Ajoutés au panier**, Page **Paramètres des** Vues), créez une liste de événements et donnez-la au développeur d’applications mobiles. Le développeur ajoute alors les événements personnalisés dans le code. Une fois approuvées, elles apparaissent comme des déclencheurs d’affichage lors de la configuration de votre audience. **Attention**: Le processus d’approbation du codage de événement personnalisé peut prendre un certain temps.

Après avoir effectué toute la préparation des messages in-app et des notifications Push, il est temps de commencer !

>[!NOTE]
>
>**Articles connexes**
>
>* [Création d’un message intégré à l’application](http://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [Créer une notification Push](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



