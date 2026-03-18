---
unique-page-id: 14352482
description: Découvrez comment fonctionne le suivi des réponses dans Sales Connect. Découvrez comment les réponses sont détectées et consignées dans Salesforce ou Marketo.
title: Fonctionnement du suivi des réponses
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 4%

---

# Fonctionnement du suivi des réponses {#how-reply-tracking-works}

Le suivi des réponses est effectué en examinant un identifiant de message qui se trouve dans chaque e-mail que vous envoyez. Chaque e-mail contient un identifiant de message unique qui nous permet d’effectuer l’un des meilleurs suivis de réponse.

>[!PREREQUISITES]
>
>**Connexion au serveur de messagerie :** [!DNL Sales Connect] devez être connecté à votre boîte de réception afin que nous sachions quand une nouvelle réponse est arrivée. Votre compte [!DNL Sales Connect] doit être [connecté à Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Si vous utilisez [!DNL Outlook], nous devrons procéder à l’intégration à votre [serveur Exchange](https://toutapp.com/next#settings/exchange_settings).

Si [!DNL Sales Connect] ne parvient pas à suivre la réponse de votre prospect à votre e-mail, il ne sera pas en mesure d’arrêter une campagne basée sur la détection de réponse ou de consigner cette réponse à [!DNL Salesforce].  Que signifie une adresse e-mail à laquelle une personne peut répondre ?

Cela signifie que si vous envoyez un e-mail à <flynn@flynnsarcade.com> et qu’il répond avec <kevinf@flynnsarcade.com>, nous sommes en mesure de suivre la réponse. De plus, si vous envoyez un e-mail à <flynn@flynnsarcade.com> et à CC <alan@encom.com> et qu’Alan vous réécrit, la réponse sera également détectée et la campagne sera terminée.
