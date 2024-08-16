---
description: Notification - Connexion au socket web - Documents Marketo - Documentation du produit
title: Notification - Connexion au web
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: eb3e7983f7521d025dff1f5d79b8caeaeb0f622c
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Notification : connexion au web {#notification-websocket-connection}

Ce document est destiné aux utilisateurs Marketo Engage qui ont reçu la notification suivante dans leur instance Marketo : `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Si vous ou votre entreprise utilisez des paramètres de pare-feu ou de serveur proxy restrictifs, vous ou votre administrateur réseau devrez peut-être placer sur la liste autorisée certains domaines et plages d’adresses IP pour vous assurer que Adobe Marketo Engage fonctionne comme prévu.

La prise en charge de Marketo n’est pas configurée pour faciliter la mise en oeuvre des protocoles ci-dessous. Si vous avez besoin d’aide, partagez ce document avec votre équipe informatique. S’ils limitent l’accès web à l’aide d’une liste autorisée, demandez-leur d’ajouter les domaines suivants (y compris l’astérisque) pour autoriser toutes les ressources et tous les websockets Marketo :

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
