---
description: Notification - Connexion Websocket - Documents Marketo - Documentation Du Produit
title: Notification - Connexion Websocket
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 2%

---

# Notification : connexion Websocket {#notification-websocket-connection}

Ce document est destiné aux utilisateurs de Marketo Engage qui ont reçu la notification suivante dans leur instance de Marketo : `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Si vous ou votre entreprise utilisez des paramètres de pare-feu ou de serveur proxy restrictifs, vous ou votre administrateur réseau devrez peut-être placer sur la liste autorisée certains domaines et plages d’adresses IP pour vous assurer que Adobe Marketo Engage fonctionne comme prévu.

La prise en charge de Marketo n’est pas configurée pour vous aider à mettre en œuvre les protocoles ci-dessous. Si vous avez besoin d’aide, veuillez partager ce document avec votre équipe informatique. S’ils restreignent l’accès web à l’aide d’un place sur la liste autorisée, demandez-leur d’ajouter les domaines suivants (y compris l’astérisque) pour autoriser toutes les ressources et tous les sockets web de Marketo :

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
