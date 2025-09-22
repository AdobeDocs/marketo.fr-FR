---
description: Présentation Du Suivi Des E-Mails - Documents Marketo - Documentation Du Produit
title: Vue d’ensemble du suivi des e-mails
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 5%

---

# Vue d’ensemble du suivi des e-mails {#email-tracking-overview}

## Fonctionnement du suivi des réponses {#how-reply-tracking-works}

Le suivi des réponses est effectué en examinant l’identifiant du message qui se trouve dans chaque e-mail que vous envoyez. Chaque e-mail contient un identifiant de message unique qui nous permet d’effectuer l’un des meilleurs suivis de réponse.

>[!PREREQUISITES]
>
>Connexion au serveur de messagerie : [!DNL Sales Connect] doit être connecté à votre boîte de réception afin que nous sachions quand une nouvelle réponse est arrivée. Votre compte [!DNL Sales Connect] doit être connecté à Gmail. Si vous utilisez Outlook, nous devrons l&#39;intégrer à votre serveur Exchange.

Si [!DNL Sales Connect] ne parvient pas à suivre la réponse de votre prospect à votre e-mail, il ne sera pas en mesure d’arrêter une campagne basée sur la détection de réponse ou de consigner cette réponse dans Salesforce. Que signifie une adresse e-mail à laquelle une personne peut répondre ?

Cela signifie que si vous envoyez un e-mail à <flynn@flynnsarcade.com> et qu’il répond avec <kevinf@flynnsarcade.com>, nous pouvons suivre la réponse. De plus, si vous envoyez un e-mail à <flynn@flynnsarcade.com> et à CC <alan@encom.com> et qu’Alan vous réécrit, la réponse sera également détectée et la campagne sera terminée.

## Comment effectuer le suivi des pièces jointes de vos e-mails {#how-to-track-your-email-attachments}

[!DNL Sales Connect] offre un suivi sur vos pièces jointes (.doc, .ppt, .pdf) afin que vous puissiez voir quand elles ont été ouvertes/téléchargées et quelles pages votre destinataire consulte. Nous vous permettrons d’utiliser notre fonctionnalité de suivi des pièces jointes à partir de l’[application web](https://toutapp.com/login) et de Gmail (ou des applications Google).

>[!NOTE]
>
>Le tracking des pièces jointes n&#39;est disponible que pour nos plans d&#39;équipe (à partir de notre plan g3startup).

**Comment envoyer votre première pièce jointe traçable**

1. Composez un e-mail ou modifiez un modèle, puis cliquez sur le bouton **[!UICONTROL Contenu]**.

1. Chargez la pièce jointe et envoyez-la. Nous prenons en charge les PDF, les documents [!DNL Word] et les présentations [!DNL Powerpoint].

1. Sélectionnez **[!UICONTROL Ajouter à l’e-mail]**.

1. Cliquez sur **[!UICONTROL Envoyer]** et lancez votre flux en direct. Vos destinataires s’afficheront à l’ouverture et lors du parcours de page de vos pièces jointes.

>[!TIP]
>
>Si vous ne souhaitez pas suivre une pièce jointe, cliquez simplement sur Joindre des fichiers et cette pièce jointe ne sera pas suivie.

## Fonctionnement du suivi des vues {#how-view-tracking-works}

Nous suivons les ouvertures d’e-mails en plaçant une image invisible dans les e-mails que vous envoyez.

Si quelqu’un répond à votre e-mail mais que [!DNL Sales Connect] indique qu’il n’a pas été consulté, il est probable que le destinataire n’ait pas activé les images dans son client de messagerie (c’est-à-dire, qu’il ait cliqué sur le message « cliquez ici pour télécharger des images » dans l’e-mail).

Quelques conseils pour obtenir de meilleures statistiques de tracking sur vos emails :

* Insérez une image dans vos e-mails (comme un logo) afin que le destinataire soit encouragé à activer les images pour voir votre message.
* Incluez un lien en tant que call to action dans l’e-mail.

## L’e-mail de test ne s’est pas affiché comme sur la prévisualisation. {#test-email-not-showed-as-viewed}

Même si vous avez envoyé votre message à une autre adresse e-mail, nous ne vous enregistrerons pas en consultant les e-mails que vous vous êtes envoyés dans le flux en direct. Notre suivi est basé sur les appareils ; tant que vous utilisez un ordinateur avec lequel vous vous êtes connecté, nous [!DNL Sales Connect] cette activité.

La raison ? [!DNL Sales Connect] est intelligent, et nos utilisateurs actifs ne nous pardonneraient jamais si leurs propres informations s’affichaient dans l’activité Flux en direct chaque fois qu’ils consultent un e-mail qu’ils envoient.
