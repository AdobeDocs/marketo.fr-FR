---
description: Notification - Connexion au socket web - Documents Marketo - Documentation du produit
title: Notification - Connexion au web
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 94afeacfdecf71e6985daccc31dd67e3d19953ac
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Notification : connexion au web {#notification-websocket-connection}

Cet article est destiné aux utilisateurs Marketo Engage qui ont reçu la notification suivante dans leur instance Marketo : `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are connected to now on March 3, 2024. Please work with your IT team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Si vous ou votre entreprise utilisez des paramètres de pare-feu ou de serveur proxy restrictifs, vous ou votre administrateur réseau devrez peut-être placer sur la liste autorisée certains domaines et plages d’adresses IP pour vous assurer que Adobe Marketo Engage fonctionne comme prévu.

La prise en charge de Marketo n’est pas configurée pour faciliter la mise en oeuvre des protocoles ci-dessous. Si vous avez besoin d’aide, partagez cet article avec votre équipe informatique. S’ils limitent l’accès web à l’aide d’une liste autorisée, demandez-leur d’ajouter les domaines suivants (y compris l’astérisque) pour autoriser toutes les ressources et tous les websockets Marketo :

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
