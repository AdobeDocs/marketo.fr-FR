---
description: Présentation du chat en direct - Documents Marketo - Documentation du produit
title: Aperçu du chat en direct
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 19f7a38a6a87bc66084e7e45f5bf49cd0d29c3cd
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---

# Aperçu du chat en direct {#live-chat-overview}

Le chat en direct permet aux visiteurs du site Web de discuter en temps réel avec vos agents de vente.

>[!NOTE]
>
>Pour les utilisateurs du package Dynamic Chat Select, le chat en direct est une fonctionnalité d’évaluation avec une limite de durée de vie de 100 engagements. Lorsque cette limite sera atteinte, tous les visiteurs qui demandent à discuter avec un agent en direct ne seront pas connectés et recevront à la place le message de secours global. Pour augmenter la limite, contactez votre représentant de compte Adobe pour discuter des options de mise à niveau des packages.

## Ajouter des agents de conversation en direct {#add-live-chat-agents}

Pour commencer à utiliser le chat en direct, vous devez ajouter vos agents de chat en direct en tant qu’[utilisateurs dans le Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} et leur donner l’autorisation [Chat en direct](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. Une fois cette opération terminée, vous pouvez ajouter une carte [chat en direct](#using-the-live-chat-card) à une boîte de dialogue nouvelle ou existante.

Lorsque les visiteurs demandent à discuter avec un agent via votre boîte de dialogue, les agents disposent de plusieurs [options de notification](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. Lorsqu’ils cliqueront sur la notification, ils seront redirigés vers leur [boîte de réception de l’agent](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} où ils pourront commencer à discuter avec le visiteur.

>[!NOTE]
>
>L’avatar de l’agent en direct utilise la photo de profil provenant du profil du compte Adobe de l’agent. Pour mettre à jour l’image, [comme suit ](https://helpx.adobe.com/fr/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

## Utilisation de la carte de conversation en direct {#using-the-live-chat-card}

Utilisez la carte de chat en direct dans le [Stream Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} lorsque vous souhaitez que les visiteurs discutent avec un agent en direct.

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>La carte de chat en direct doit toujours être la dernière carte de la branche. Si la carte est placée dans un point aléatoire de la branche, cela peut surprendre le visiteur en le connectant soudainement à un agent.

### Meilleures pratiques {#best-practices}

* Utilisez une carte de questions avant la carte de chat en direct demandant au visiteur s’il souhaite se connecter.
* Une fois que le visiteur a accepté de se connecter, utilisez la carte de capture d’informations pour collecter certaines de ses informations, telles que son prénom/nom, son adresse e-mail, son intitulé de poste, etc. (il est recommandé de demander au moins le prénom et l’adresse e-mail).

## Options de la carte de conversation en direct {#live-chat-card-options}

Cliquer sur la carte de chat en direct dans le flux vous permet de choisir comment le visiteur est acheminé. Faites votre choix parmi la sélection à tour de rôle, un agent, des règles personnalisées ou une équipe.

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Round-robin</b></td>
   <td>Les conversations sont affectées aux agents dans un ordre séquentiel.</td>
  </tr> 
  <tr> 
   <td><b>Agent ou agente</b></td>
   <td>Choisissez un agent spécifique pour recevoir la conversation.</td>
  </tr>
    <tr> 
   <td><b>Règles personnalisées</b></td>
   <td>Toutes les règles personnalisées seront passées en revue au moment de déterminer où acheminer le visiteur. Si le visiteur ne remplit les critères d’aucune règle personnalisée, il reçoit le <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">message de secours du chat en direct</a>.</td>
  </tr> 
  <tr> 
   <td><b>Équipe</b></td>
   <td>Sélectionnez une équipe spécifique pour recevoir la conversation. Si cette option est choisie, elle sera attribuée à tour de rôle au sein de cette équipe.</td>
  </tr>
 </tbody> 
</table>

## Notifications de conversation en direct {#live-chat-notifications}

>[!IMPORTANT]
>
>Pour recevoir des notifications de navigateur pour le chat en direct, tous les agents de chat en direct doivent activer les notifications de navigateur pour Dynamic Chat lorsque cela vous est demandé.

### Activation des notifications {#enabling-notifications}

Lorsqu’ils se connectent, les agents de messagerie en direct voient une bannière dans la partie supérieure de l’écran indiquant « Veuillez activer les notifications du navigateur pour recevoir des notifications de messagerie en direct. » Cliquez sur **Activer**.

![](assets/live-chat-overview-4.png)

Les agents de chat en direct seront ensuite invités par le navigateur à afficher les notifications. Cliquez sur **Autoriser**.

![](assets/live-chat-overview-5.png)

Si les agents n’obtiennent pas de notifications de navigateur, même après l’avoir autorisé dans le navigateur, ils doivent éventuellement activer les notifications pour le navigateur dans les paramètres de notification du système d’exploitation :

[Étapes pour Mac](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[Étapes pour Windows](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### Lorsqu’une discussion en direct est acheminée vers un agent {#when-a-live-chat-is-routed-to-an-agent}

Lorsqu’un chat en direct est acheminé vers un agent, une bannière bleue s’affiche en haut de l’écran pour lui demander d’accepter, ainsi qu’un son de notification pour éviter les notifications manquées.

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>Vous avez également la possibilité de configurer des notifications de navigateur, qui vous avertiront si vous n’êtes pas connecté à Dynamic Chat.
>
>* Activer les notifications de navigateur dans [Google Chrome](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}
>* Activer les notifications de navigateur dans [Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}

### Notifications d’action ayant échoué {#failed-action-notifications}

Lorsqu’une action telle qu’une réservation de réunion ou un chat en direct échoue, les utilisateurs sont avertis par e-mail.

![](assets/live-chat-overview-6.png)

### Éléments à noter {#things-to-note}

* Les agents ont 100 secondes pour répondre avant l&#39;expiration du message « Accepter le chat ». Ensuite, les visiteurs et visiteuses recevront le [ message de secours ](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback){target="_blank"}. Pour les abonnés Dynamic Chat Prime dont l’option de routage est définie sur **Équipe**, un agent supplémentaire sera essayé avant l’affichage du message de secours.
* Il existe actuellement une limite de 10 discussions en direct par agent.
* La boîte de réception de l’agent est réservée aux conversations en direct. Si le chat n’est pas accepté par un agent, il n’apparaîtra pas dans la boîte de réception de l’agent, car il n’est pas qualifié de chat en direct.
* L’onglet Conversation affiche toutes les conversations, aussi bien les conversations en direct que les conversations automatisées. Ainsi, si une conversation n’est pas acceptée par l’agent, elle est répertoriée dans l’onglet Conversation . L’onglet Conversation peut prendre jusqu’à 24 heures, car il ne s’agit pas de temps réel. La boîte de réception de l’agent est toutefois en temps réel.
* S’il n’y a aucune activité de conversation après 10 minutes (par l’agent ou le visiteur), la conversation expire.
* Si un agent modifie son image de profil (dans account.adobe.com) _pendant_ une discussion en direct, le visiteur verra toujours l’ancienne image jusqu’à la fin de la discussion. Le visiteur verra la nouvelle image la prochaine fois qu’il discutera et obtiendra cet agent.

>[!MORELIKETHIS]
>
>[ Boîte de réception de l’agent ](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
