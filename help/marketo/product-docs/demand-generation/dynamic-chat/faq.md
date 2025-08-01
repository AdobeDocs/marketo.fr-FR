---
description: FAQ sur Dynamic Chat - Documents Marketo - Documentation du produit
title: FAQ sur Dynamic Chat
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# FAQ sur Dynamic Chat {#dynamic-chat-faq}

Consultez ci-dessous les réponses à certaines questions fréquentes sur Dynamic Chat.

**Je n’ai apparemment pas accès à Dynamic Chat. Comment puis-je l&#39;avoir ?**

Contactez votre administrateur Marketo Engage et assurez-vous qu’il vous a [ajouté en tant qu’utilisateur](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} dans le Adobe Admin Console.

**Puis-je installer Dynamic Chat n’importe où sur le site web de ma société ou est-ce que cela fonctionne uniquement sur les pages de destination de Marketo ?**

Le fragment de code Dynamic Chat JavaScript peut être installé sur n’importe quel site web, ainsi que sur les pages de destination Marketo.

**Pendant combien de temps les données sont-elles stockées pour la création de rapports ?**

90 jours. Pour obtenir la liste complète des limites/paramètres, consultez la page Marketo Engage [Description du produit](https://helpx.adobe.com/fr/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

**Dynamic Chat prend-il en charge d’autres langues que l’anglais ?**

Oui. Dynamic Chat prend en charge les langues suivantes : français, espagnol, allemand, japonais, néerlandais, italien, portugais brésilien, coréen, chinois simplifié et chinois traditionnel. En savoir plus dans [Modification de la langue](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"}.

**Prenez-vous en charge les fonctionnalités AI/NLP ?**

Nous ne prenons pas en charge les fonctionnalités d’IA/NLP.

**Comment cibler des personnes anonymes ?**

Dans votre boîte de dialogue, vous devez utiliser l’attribut _L’e-mail de la personne est vide_.

**Qu’est-ce qui qualifie une conversation engagée ?**

Une conversation engagée se produit dès qu’un visiteur répond au robot dans une boîte de dialogue ou un flux de conversation. Si le visiteur ouvre le bot conversationnel mais ne répond pas au bot (par exemple, sélectionnez une réponse ou envoyez des informations), cela n’est pas comptabilisé comme un engagement.

**Que se passe-t-il si j’atteint ma limite mensuelle de conversations engagées ?**

Lorsque vous atteignez votre limite mensuelle de conversation engagée, toutes les boîtes de dialogue et tous les flux de conversation publiés cesseront de se déclencher jusqu’à ce que vous augmentiez votre limite ou que votre limite se réinitialise au début du mois suivant.

**Comment puis-je savoir quand j’approche de ma limite de conversation engagée ?**

Lorsque vous aurez atteint 90 % de votre limite de conversation engagée, les administrateurs de Dynamic Chat recevront une notification par e-mail et tous les utilisateurs verront une notification de bannière dans Dynamic Chat.

**Si un visiteur engage une boîte de dialogue, puis se connecte par la suite à un agent en direct, cela compte-t-il comme un engagement ou deux ?**

Pour les clients du package Select, cela compte comme deux engagements distincts : un pour l’engagement dans la boîte de dialogue et un pour l’engagement dans le chat en direct. Pour les clients du package Prime, les engagements de conversation en direct ne sont pas comptabilisés séparément, ce qui signifie qu’ils ne sont comptabilisés que pour un seul engagement.

**À quelle fréquence la limite de conversation engagée est-elle réinitialisée ?**

La limite de conversation engagée est réinitialisée le premier de chaque mois civil.

**Pourquoi le bot conversationnel ne revient-il pas une fois que j’ai terminé une conversation ?**

Les boîtes de dialogue sont conçues pour n’être affichées qu’une seule fois pour un visiteur. Ainsi, dès qu’un visiteur atteint la fin d’une branche donnée dans une boîte de dialogue, celle-ci est considérée comme terminée et ne lui sera plus jamais présentée.

**Lorsque je clique sur la mosaïque Dynamic Chat dans Mon Marketo et que je me connecte à Adobe Experience Cloud, pourquoi est-ce que j’obtiens le message suivant ?  »_Il semble que votre Adobe ID ne soit pas lié à vos comptes de solution Adobe Experience Cloud_. »**

Cela indique probablement que vous n’avez pas été ajouté en tant qu’utilisateur Dynamic Chat dans le Adobe Admin Console. Contactez un administrateur système pour votre organisation Adobe ou un administrateur produit pour Dynamic Chat pour demander l’accès à Dynamic Chat.

**Comment puis-je accéder au relevé de notes d’une conversation engagée ?**

Les transcriptions Dynamic Chat sont accessibles pour tout prospect connu qui a engagé une boîte de dialogue Dynamic Chat via l’activité « Engagé dans la boîte de dialogue » dans Marketo Engage et dont le statut de conversation est soit « Terminé » soit « Abandonné ».

**Une fois qu’un visiteur s’engage dans une boîte de dialogue, peut-il relancer la conversation ou revenir à une question précédente ?**

Il n’existe actuellement aucun moyen systématique de relancer une conversation ou de revenir à un point précédent, mais celui-ci se trouve sur la feuille de route de Dynamic Chat.

**Dynamic Chat s’intègre-t-il à Salesforce ?**

Dynamic Chat s’intègre à Salesforce via l’intégration de Marketo Engage Salesforce.

**Mon calendrier est connecté à Dynamic Chat et je suis inclus dans les règles de routage, alors pourquoi n’ai-je aucune réunion ?**

Cela indique probablement que votre connexion au calendrier doit être réauthentifiée. Cela se produit le plus souvent lorsque vous modifiez le mot de passe de votre fournisseur de calendrier et que Dynamic Chat perd la connexion. Vous pouvez simplement accéder à la page Paramètres d’agent dans Dynamic Chat et cliquer sur « Réauthentifier le calendrier ».

**Quelle est la différence entre un dialogue et un flux de conversation ?**

Une boîte de dialogue est une conversation automatiquement affichée pour les visiteurs et visiteuses web qui répondent à un ensemble défini de critères de ciblage. Un flux de conversation ne s’affiche que pour les visiteurs et visiteuses qui effectuent une action spécifique sur le web, comme appuyer sur un bouton.

**Existe-t-il un moyen d’utiliser Dynamic Chat pour réserver des réunions directement à partir d’un e-mail ?**

Oui! [Découvrez comment procéder](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}.

**Que signifient exactement des termes tels que « Engagé » ou « Personnes acquises » ?**

Plusieurs termes sont utilisés dans Dynamic Chat. Les définitions de plusieurs d’entre eux se trouvent dans les articles d’aide de leurs zones respectives.

* Des termes Analytics tels que « Personnes acquises » [se trouvent ici](/help/marketo/product-docs/demand-generation/dynamic-chat/analytics.md#definitions){target="_blank"}.
* Définitions de filtre/déclencheur de liste dynamique [ici](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities.md#definitions){target="_blank"}.
* Les descriptions des différentes cartes Stream Designer [sont disponibles ici](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}.

**Puis-je utiliser Dynamic Chat sans Marketo Engage ?**

Non. Bien que Dynamic Chat soit une application distincte de Marketo Engage, les deux sont inextricablement liés.
