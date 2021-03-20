---
unique-page-id: 14352482
description: Fonctionnement du suivi des réponses - Documents marketing - Documentation du produit
title: Fonctionnement du suivi des réponses
translation-type: tm+mt
source-git-commit: 073b73255d49f859c32c8b4793e6798f02f7a5c4
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Fonctionnement du suivi des réponses {#how-reply-tracking-works}

Le suivi des réponses s’effectue en recherchant un identifiant de message figurant dans chaque courrier électronique que vous envoyez. Chaque courrier électronique contient un identifiant de message unique qui nous permet de disposer du meilleur suivi des réponses.

>[!PREREQUISITES]
>
>**Connexion avec le serveur de messagerie :** Sales Connect doit être connecté à votre boîte de réception pour que nous sachions quand une nouvelle réponse est arrivée. Vous devez disposer de votre compte Sales Connect [connecté à Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Si vous utilisez Outlook, nous devrons intégrer votre [serveur d&#39;échange](https://toutapp.com/next#settings/exchange_settings).

Si Sales Connect ne peut pas suivre la réponse de votre prospect à votre courriel, il ne pourra pas arrêter une campagne en fonction de la détection des réponses ou consigner cette réponse à Salesforce.  Qu&#39;est-ce qu&#39;on veut dire que toute adresse électronique peut répondre ?

Cela signifie que si vous envoyez un courriel à flynn@flynnsarcade.com et qu&#39;il répond par kevinf@flynnsarcade.com, nous pouvons suivre la réponse. De plus, si vous envoyez un courrier électronique à flynn@flynnsarcade.com et CC alan@encom.com et qu’Alan vous répond, il détectera également la réponse et mettra fin à la campagne.
