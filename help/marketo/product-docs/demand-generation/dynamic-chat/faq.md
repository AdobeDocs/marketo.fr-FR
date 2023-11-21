---
description: FAQ sur le Dynamic Chat - Documents Marketo - Documentation du produit
title: FAQ sur Dynamic Chat
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: a7404dc5c3f2014f53d49fd033f7e4002b9b2203
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 0%

---

# FAQ sur Dynamic Chat {#dynamic-chat-faq}

Consultez ci-dessous pour obtenir des réponses à certaines questions fréquentes sur Dynamic Chat.

**Puis-je installer Dynamic Chat n’importe où sur le site web de ma société ou est-ce que cela ne fonctionne que sur les landing pages Marketo ?**

Le fragment de code JavaScript du Dynamic Chat peut être installé sur n’importe quel site web ainsi que sur les landing pages Marketo.

**Quelle est la durée de stockage des données pour la création de rapports ?**

90 jours. Pour obtenir la liste complète des limites/paramètres, veuillez consulter le Marketo Engage [Page Description du produit](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

**Le Dynamic Chat prend-il en charge d’autres langues que l’anglais ?**

Oui. Le Dynamic Chat prend en charge les langues suivantes : allemand, français, espagnol, japonais, néerlandais, italien, portugais brésilien, coréen, chinois simplifié et chinois traditionnel. En savoir plus dans [Modification de la langue](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"}.

**Prenez-vous en charge la fonctionnalité AI/NLP ?**

La fonctionnalité AI/NLP n’est pas prise en charge.

**Comment cibler les personnes anonymes ?**

Dans votre boîte de dialogue, vous devez utiliser la variable _L’adresse électronique de personne est vide_ attribut.

**Qu&#39;est-ce qu&#39;une conversation engagée ?**

Une conversation engagée survient dès qu’un visiteur répond au robot dans un flux de dialogue ou de conversation. Si le visiteur ouvre le chatterbot mais ne répond pas au robot (par exemple, il sélectionne une réponse ou envoie des informations), il ne compte pas comme un engagement.

**Que se passe-t-il si j&#39;atteint ma limite mensuelle de conversation active ?**

Lorsque vous atteignez la limite mensuelle des conversations actives, tous les dialogues et flux de conversation publiés cesseront de se déclencher jusqu’à ce que vous ayez augmenté votre limite ou que votre limite soit réinitialisée au début du mois suivant.

**Comment le saurai-je lorsque je me rapproche de ma limite de conversation engagée ?**

Lorsque vous avez atteint 90 % de la limite de vos conversations actives, les administrateurs de Dynamic Chat reçoivent une notification par e-mail et tous les utilisateurs reçoivent une notification de bannière dans Dynamic Chat.

**Si un visiteur interagit avec un dialogue, puis se connecte ensuite à un agent en direct, est-ce que cela compte comme un ou deux engagements ?**

Pour les clients du module Sélectionner, cela compte comme deux engagements distincts : l’un pour l’engagement Dialogue et l’autre pour l’engagement chat en direct. Pour les clients du module Prime, les engagements de conversation en direct ne sont pas comptabilisés séparément, ce qui ne compte qu’comme un seul engagement.

**À quelle fréquence la limite de conversation engagée est-elle réinitialisée ?**

La limite de conversation en cours est réinitialisée le premier de chaque mois calendaire.

**Pourquoi le chatterbot ne revient-il pas après avoir terminé une conversation ?**

Les boîtes de dialogue sont conçues pour être présentées une seule fois à un visiteur. Ainsi, dès qu’un visiteur atteint la fin d’une branche donnée dans un dialogue, ce dialogue est considéré comme terminé et ne sera plus jamais présenté à ce visiteur.

**Lorsque je clique sur la mosaïque Dynamic Chat dans Mon Marketo et que je me connecte à Adobe Experience Cloud, pourquoi ai-je le message suivant ? &quot;_Il semble que votre Adobe ID ne soit pas lié à vos comptes de solution Adobe Experience Cloud_.&quot;**

Cela indique probablement que vous n’avez pas été ajouté en tant qu’utilisateur Dynamic Chat dans Adobe Admin Console. Contactez un administrateur système pour votre organisation d’Adobe ou un administrateur de produit pour que Dynamic Chat demande l’accès à Dynamic Chat.

**Comment puis-je accéder à la transcription d’une conversation engagée ?**

Vous pouvez accéder aux transcriptions des Dynamic Chat pour tout prospect connu qui a engagé un dialogue avec un Dynamic Chat via l’activité &quot;Engagé avec un dialogue&quot; en Marketo Engage.

**Une fois qu’un visiteur s’engage dans un dialogue, peut-il relancer la conversation ou revenir à une question précédente ?**

Il n&#39;existe actuellement aucun moyen systématique de relancer une conversation ou de revenir à un point précédent, mais c&#39;est sur la feuille de route du Dynamic Chat.

**Dynamic Chat s’intègre-t-il à Salesforce ?**

Dynamic Chat s’intègre à Salesforce par le biais de l’intégration de Salesforce Marketo Engage.

**Mon calendrier est connecté en Dynamic Chat et je suis inclus dans les règles de routage, alors pourquoi est-ce que je ne reçois aucune réunion ?**

Cela indique probablement que votre connexion au calendrier doit être réauthentifiée. Cela se produit le plus souvent lorsque vous modifiez votre mot de passe pour votre fournisseur de calendrier et que le Dynamic Chat perd la connexion. Vous pouvez simplement accéder à la page Paramètres de l’agent dans Dynamic Chat et cliquer sur &quot;Réauthentifier le calendrier&quot;.

**Quelle est la différence entre un dialogue et un flux de conversation ?**

Un dialogue est une conversation qui s’affiche automatiquement pour les visiteurs web qui répondent à un ensemble défini de critères de ciblage. Un flux de conversation s’affiche uniquement pour les visiteurs qui effectuent une action spécifique sur le Web, comme appuyer sur un bouton.

**Existe-t-il un moyen d’utiliser Dynamic Chat pour réserver des réunions directement à partir d’un email ?**

Oui! [Découvrir comment](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}.

**Puis-je utiliser Dynamic Chat sans Marketo Engage ?**

Non. Bien que Dynamic Chat soit une application distincte de Marketo Engage, les deux sont inextricablement liés.
