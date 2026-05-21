---
description: Détails de notification pour les utilisateurs de Marketo Engage qui ont reçu la notification Impossible d’établir une connexion Websocket
title: Notification - Connexion Websocket
hide: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
TQID: https://experienceleague.adobe.com/NpcRnxQPi03CF8z77Urrfs2P2phkuRbh2pd5J1UquFk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 30%

---

# Notification : connexion Websocket {#notification-websocket-connection}

Ce document est destiné aux utilisateurs de Marketo Engage qui ont reçu la notification suivante dans leur instance de Marketo : `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Si vous ou votre entreprise utilisez des paramètres de pare-feu ou de serveur proxy restrictifs, vous (ou votre administrateur ou administratrice réseau) devrez peut-être placer sur la liste autorisée certains domaines et plages d’adresses IP pour vous assurer que Adobe Marketo Engage fonctionne comme prévu.

La prise en charge de Marketo n’est pas configurée pour vous aider à mettre en œuvre les protocoles ci-dessous. Si vous avez besoin d’aide, veuillez partager ce document avec votre équipe informatique. S’ils restreignent l’accès web à l’aide d’un place sur la liste autorisée, demandez-leur d’ajouter les domaines suivants (y compris l’astérisque) pour autoriser toutes les ressources et tous les sockets web de Marketo :

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
