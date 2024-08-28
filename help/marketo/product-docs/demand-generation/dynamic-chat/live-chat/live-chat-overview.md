---
description: Présentation de la messagerie instantanée - Documents Marketo - Documentation du produit
title: Présentation de la messagerie instantanée
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: d88406c1f9d72c57a6d4f09934cbf685499ed198
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 1%

---

# Présentation de la messagerie instantanée {#live-chat-overview}

Le chat en direct permet aux visiteurs du site Web de discuter en temps réel avec vos agents de vente.

>[!NOTE]
>
>Pour les utilisateurs du module Sélection du Dynamic Chat, le chat en direct est une fonctionnalité d’évaluation dont la durée de vie est limitée à 100 engagements. Lorsque cette limite est atteinte, les visiteurs qui souhaitent discuter avec un agent en direct ne sont pas connectés et recevront à la place le message de secours global. Pour augmenter cette limite, contactez votre gestionnaire de compte Adobe pour discuter des options de mise à niveau du package.

## Ajout d’agents de messagerie instantanée {#add-live-chat-agents}

Pour commencer à discuter en direct, vous devez ajouter vos agents de conversation en direct en tant qu’ [utilisateurs dans Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} et leur accorder l’[autorisation de conversation en direct](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. Une fois cette opération terminée, vous pouvez ajouter une [carte de conversation en direct](#using-the-live-chat-card) à un dialogue nouveau ou existant.

Lorsque les visiteurs demandent à dialoguer avec un agent via votre dialogue, les agents ont plusieurs [options de notification](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. Lorsqu’ils cliquent sur la notification, ils sont redirigés vers leur [boîte de réception de l’agent](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} où ils peuvent commencer à discuter avec le visiteur.

>[!NOTE]
>
>L’avatar de l’agent en direct utilise l’image de profil du profil d’Adobe de l’agent. Pour mettre à jour l&#39;image, suivez [ces étapes](https://helpx.adobe.com/fr/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

## Utilisation de la carte de conversation en direct {#using-the-live-chat-card}

Utilisez la carte de conversation en direct dans le [ flux Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} lorsque vous souhaitez que les visiteurs discutent avec un agent en direct.

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>La carte de conversation en direct doit toujours être la dernière carte de la branche. Si la carte est placée au hasard dans la branche, le visiteur pourrait être surpris en la connectant soudainement à un agent.

### Meilleures pratiques {#best-practices}

* Utilisez une carte de questions avant la carte de conversation en direct qui demande au visiteur s’il souhaite se connecter.
* Une fois que le visiteur a accepté de se connecter, utilisez la carte de capture d’informations pour collecter certaines de ses informations, telles que le prénom/nom, l’adresse électronique, le titre de la tâche, etc. (il est recommandé de demander au moins le prénom et l’adresse électronique).

## Options de carte de conversation en direct {#live-chat-card-options}

Cliquer sur la carte de conversation en direct dans le flux vous permet de choisir comment le visiteur est routé. Faites votre choix parmi un robot rond, un agent, des règles personnalisées ou une équipe.

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Round-robin</b></td>
   <td>Les tchats sont attribués aux agents dans l’ordre séquentiel.</td>
  </tr> 
  <tr> 
   <td><b>Agent</b></td>
   <td>Sélectionnez un agent spécifique pour recevoir la conversation.</td>
  </tr>
    <tr> 
   <td><b>Règles personnalisées</b></td>
   <td>Toutes les règles personnalisées sont analysées lors de la prise en compte de l’emplacement du visiteur. Si le visiteur n’est éligible à aucune règle personnalisée, il reçoit le <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">message de secours de conversation en direct</a>.</td>
  </tr> 
  <tr> 
   <td><b>Équipe</b></td>
   <td>Choisissez une équipe spécifique pour recevoir la conversation. Si cette option est sélectionnée, elle se verra attribuer un tourbillon au sein de cette équipe.</td>
  </tr>
 </tbody> 
</table>

## Notifications de tchat en direct {#live-chat-notifications}

>[!IMPORTANT]
>
>Pour recevoir des notifications de navigateur pour la messagerie instantanée, tous les agents de messagerie instantanée doivent activer les notifications de navigateur pour le Dynamic Chat lorsqu’ils y sont invités.

### Activation des notifications {#enabling-notifications}

Les agents de messagerie instantanée voient une bannière en haut de l’écran lorsqu’ils se connectent. Celle-ci indique &quot;Veuillez activer les notifications de navigateur pour recevoir des notifications de conversation en direct.&quot; Cliquez sur **Activer**.

![](assets/live-chat-overview-4.png)

Les agents de conversation en direct seront alors invités par le navigateur à afficher les notifications. Cliquez sur **Autoriser**.

![](assets/live-chat-overview-5.png)

Si les agents n’obtiennent pas de notifications du navigateur même après l’avoir autorisé dans le navigateur, ils peuvent avoir besoin d’activer les notifications du navigateur dans les paramètres de notification du système d’exploitation :

[Étapes pour Mac](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[Étapes pour Windows](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### Lorsqu’une conversation en direct est acheminée vers un agent {#when-a-live-chat-is-routed-to-an-agent}

Lorsqu’une conversation en direct est envoyée à un agent, une bannière bleue s’affiche en haut de l’écran pour lui demander d’accepter, ainsi qu’un son de notification pour empêcher les notifications manquées.

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>Vous avez également la possibilité de configurer des notifications de navigateur qui vous avertiront si vous n’êtes pas connecté à Dynamic Chat.
>
>* Activation des notifications de navigateur dans [Google Chrome](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}
>* Activation des notifications de navigateur dans [Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}

### Notifications d’action ayant échoué {#failed-action-notifications}

Lorsqu’une action telle qu’une réservation de réunion ou une conversation en direct échoue, les utilisateurs sont avertis par e-mail.

![](assets/live-chat-overview-6.png)

### Informations à noter {#things-to-note}

* Les agents disposent de 45 secondes pour répondre avant que le message &quot;Chat Accept&quot; n’expire. Ensuite, les visiteurs recevront le [message de secours](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback){target="_blank"}. Pour les abonnés Dynamic Chat Prime dont l’option de routage est définie sur **Team**, un autre agent sera tenté avant l’affichage du message de secours.
* Il existe actuellement une limite de 10 conversations en direct par agent.

>[!MORELIKETHIS]
>
>[Boîte de réception de l’agent](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
