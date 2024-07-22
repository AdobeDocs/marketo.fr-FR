---
description: Présentation du suivi des emails - Documentation Marketo - Documentation du produit
title: Présentation du suivi des emails
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Présentation du suivi des emails {#email-tracking-overview}

## Fonctionnement du suivi des réponses {#how-reply-tracking-works}

Le suivi des réponses s’effectue en examinant un identifiant de message qui se trouve dans chaque email que vous envoyez. Chaque email contient un identifiant de message unique qui nous permet d’avoir le meilleur suivi de réponse possible.

>[!PREREQUISITES]
>
>Connexion avec le serveur de messagerie : Sales Connect doit être connecté à votre boîte de réception afin que nous sachions quand une nouvelle réponse est arrivée. Votre compte Sales Connect doit être connecté à Gmail. Si vous utilisez Outlook, nous devrons intégrer votre serveur exchange.

Si Sales Connect ne peut pas suivre la réponse de votre prospect à votre email, il ne pourra pas arrêter une campagne basée sur la détection des réponses ni consigner cette réponse à Salesforce. Que signifie toute adresse email à laquelle on peut répondre ?

Cela signifie que si vous envoyez un email à flynn@flynnsarcade.com et qu’il répond avec kevinf@flynnsarcade.com, nous pouvons suivre la réponse. De plus, si vous envoyez des courriels à flynn@flynnsarcade.com et CC alan@encom.com, et qu&#39;Alan vous répond, il détectera également la réponse et mettra fin à la campagne.

## Comment effectuer le suivi de vos pièces jointes aux emails {#how-to-track-your-email-attachments}

Sales Connect offre un suivi sur vos pièces jointes (.doc, .ppt, .pdf) afin que vous puissiez déterminer quand elles ont été ouvertes/téléchargées et voir les pages que votre destinataire consulte. Nous vous autoriserons à utiliser notre fonctionnalité de pièces jointes pouvant faire l’objet d’un suivi à partir de l’ [application web](https://toutapp.com/login) et de Gmail (ou des applications Google).

>[!NOTE]
>
>Le suivi des pièces jointes est uniquement disponible pour nos plans d’équipe (à partir de notre plan de démarrage g3).

**Comment envoyer votre première pièce jointe pouvant faire l’objet d’un suivi**

1. Composez un email ou modifiez un modèle, puis cliquez sur le bouton **Contenu** .

1. Téléchargez votre pièce jointe et envoyez-la. Nous prenons en charge les PDF, les documents Word et les présentations PowerPoint.

1. Sélectionnez **Ajouter au courrier électronique**.

1. Cliquez sur **Envoyer** et déclenchez votre flux en direct. Vous verrez vos destinataires pendant qu’ils s’ouvrent et parcourent vos pièces jointes.

>[!TIP]
>
>Si vous ne souhaitez pas effectuer le suivi d’une pièce jointe, cliquez simplement sur Joindre des fichiers et cette pièce jointe ne sera pas suivie.

## Fonctionnement du suivi des vues {#how-view-tracking-works}

Nous effectuons le suivi des ouvertures d’email en plaçant une image invisible dans les emails que vous envoyez.

Si quelqu’un répond à votre email mais que Sales Connect indique qu’il n’a pas été visualisé, il y a des chances que le destinataire n’ait pas activé les images dans son client de messagerie (c’est-à-dire, cliquez sur le message &quot;cliquez ici pour télécharger les images&quot; dans l’email).

Quelques conseils pour obtenir de meilleurs statistiques de tracking sur vos emails :

* Incluez une image dans vos emails (comme un logo) afin que le destinataire soit invité à activer les images pour voir votre message.
* Incluez un lien comme appel à l’action dans le courrier électronique.

## Test de l’e-mail non affiché comme affiché {#test-email-not-showed-as-viewed}

Même si vous avez envoyé votre message à une autre adresse électronique, nous ne vous consignerons pas l’affichage des courriers électroniques que vous vous êtes envoyés dans le flux en direct. Notre suivi est basé sur les appareils. Tant que vous utilisez un ordinateur sur lequel vous êtes connecté à Sales Connect, nous allons filtrer cette activité.

La raison ? Sales Connect est dynamique et nos utilisateurs actifs ne nous pardonneraient jamais si leurs propres informations s’affichaient dans l’activité Flux en direct chaque fois qu’ils regardaient un email qu’ils envoyaient.
