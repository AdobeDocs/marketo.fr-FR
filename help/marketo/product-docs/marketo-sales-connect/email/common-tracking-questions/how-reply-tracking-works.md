---
unique-page-id: 14352482
description: Fonctionnement du suivi des réponses - Documents Marketo - Documentation du produit
title: Fonctionnement du suivi des réponses
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Fonctionnement du suivi des réponses {#how-reply-tracking-works}

Le suivi des réponses s’effectue en examinant un identifiant de message qui se trouve dans chaque email que vous envoyez. Chaque email contient un identifiant de message unique qui nous permet d’avoir le meilleur suivi de réponse possible.

>[!PREREQUISITES]
>
>**Connexion avec le serveur de messagerie :** Sales Connect (Connexion aux ventes) doit être connecté à votre boîte de réception pour que nous sachions quand une nouvelle réponse est arrivée. Votre compte [Sales Connect doit être connecté à Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Si vous utilisez Outlook, nous devrons intégrer votre [serveur d’exchange](https://toutapp.com/next#settings/exchange_settings).

Si Sales Connect ne peut pas suivre la réponse de votre prospect à votre email, il ne pourra pas arrêter une campagne en fonction de la détection des réponses ou consigner cette réponse à Salesforce.  Que signifie toute adresse email à laquelle on peut répondre ?

Cela signifie que si vous envoyez un email à flynn@flynnsarcade.com et qu&#39;il répond avec kevinf@flynnsarcade.com, nous pouvons suivre la réponse. De plus, si vous envoyez des courriels à flynn@flynnsarcade.com et CC alan@encom.com, et qu&#39;Alan vous répond, il détectera également la réponse et mettra fin à la campagne.
