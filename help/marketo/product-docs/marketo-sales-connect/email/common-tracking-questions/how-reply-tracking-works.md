---
unique-page-id: 14352482
description: Fonctionnement du suivi des réponses - Documents marketing - Documentation du produit
title: Fonctionnement du suivi des réponses
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---


# Fonctionnement du suivi des réponses {#how-reply-tracking-works}

Le suivi des réponses s’effectue en recherchant un identifiant de message figurant dans chaque courrier électronique que vous envoyez. Chaque courrier électronique contient un identifiant de message unique qui nous permet de disposer du meilleur suivi des réponses.

>[!NOTE]
>
>**Conditions préalables**
>
>**Connexion au serveur de messagerie :** Sales Connect doit être connecté à votre boîte de réception pour que nous sachions quand une nouvelle réponse est arrivée. Vous devez avoir votre compte Sales Connect [connecté à Gmail](http://docs.marketo.com/x/kYMOAQ). Si vous utilisez Outlook, nous devrons intégrer votre serveur [](http://toutapp.com/next#settings/exchange_settings)Exchange.

Si Sales Connect ne peut pas suivre la réponse de votre prospect à votre courriel, il ne pourra pas arrêter une campagne en fonction de la détection des réponses ou consigner cette réponse à Salesforce.  Qu&#39;est-ce qu&#39;on veut dire que toute adresse électronique peut répondre ?

Cela signifie que si vous envoyez un courriel [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) et qu&#39;il répond [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad), nous pouvons suivre la réponse. De plus, si vous envoyez un courrier électronique [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) et un CC [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153)et qu’Alan vous répond, il détectera également la réponse et mettra fin à la campagne.
