---
description: Fonctions de rappel - Documents Marketo - Documentation du produit
title: Fonctions de rappel
feature: Dynamic Chat
exl-id: 5ae7f6cb-5c57-4257-8a1a-992c9602cfaa
source-git-commit: fd070322b6741268595d460318246abd3768dd3d
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 7%

---

# Fonctions de rappel {#callback-functions}

Vous pouvez utiliser des fonctions de rappel de widget Dynamic Chat pour envoyer des événements de conversation à des plateformes tierces.

## Prise en main {#getting-started}

Cet événement indique que le widget du Dynamic Chat est prêt à l’emploi et est déclenché lorsque tous les scripts liés au Dynamic Chat sont chargés dans la page web.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    // code here will execute when chatbot scripts are loaded in a webpage 
});
```

## Événements de conversation {#conversation-events}

Ces événements sont liés à une conversation qui est ciblée sur une page spécifique pour un visiteur spécifique.

### Conversation déclenchée

Une conversation (un dialogue, par exemple) qui est ciblée sur un visiteur de site web est résolue et le chatterbot lui est présenté.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 

    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
// code here will execute when chatbot is loaded for a visitor 
   });
});
```

### Conversation engagée {#conversation-engaged}

Le visiteur a interagi (par exemple, a fourni sa première réponse) avec le chatterbot.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => { 
 // code here will execute when visitor engages with chatbot 
    });
});
```

### Conversation terminée {#conversation-completed}

Le visiteur a atteint la fin de la conversation.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => { 
 // code here will execute when conversation is completed 
    });
});
```

### Conversation fermée

Le visiteur a clos la conversation avant d’atteindre la fin.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => { 
 // code here will execute when conversation is closed 
    });
});
```

La variable `event` est un objet avec des métadonnées liées à la conversation. Vous pouvez accéder à ces métadonnées en accédant à `event.data`.

Vous trouverez ci-dessous quelques valeurs de métadonnées clés auxquelles vous pouvez accéder :

<table>
<thead>
  <tr>
    <th style="width:75%">Métadonnées</th>
    <th style="width:25%">Attributs</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nom de la conversation</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identifiant de conversation</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Type de conversation (flux de dialogue/conversation)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Type d’interface utilisateur (pop-up/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID de session</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Événements d’entrée du visiteur

Ces événements sont déclenchés lorsqu’un visiteur participant à une conversation fournit ses coordonnées (par exemple, son numéro de téléphone ou son adresse électronique). Vous trouverez ci-dessous les événements qui entrent dans cette catégorie.

### Numéro de téléphone {#phone-number}

Cet événement est déclenché lorsqu’un visiteur indique son numéro de téléphone au cours de la conversation.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => { 
  // code here will execute when a visitor provides their phone number 
    }); 
}); 
```

### ID d’e-mail {#email-id}

Cet événement est déclenché lorsqu’un visiteur fournit son adresse électronique au cours de la conversation.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => { 
 // code here will execute when a visitor provides their email address 
    }); 
});
```

La variable `event` est un objet avec des métadonnées liées à la conversation. Vous pouvez accéder à ces métadonnées en accédant à `event.data`.

Vous trouverez ci-dessous quelques valeurs de métadonnées clés auxquelles vous pouvez accéder.

<table>
<thead>
  <tr>
    <th style="width:75%">Métadonnées</th>
    <th style="width:25%">Attributs</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nom de la conversation</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identifiant de conversation</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Type de conversation (flux de dialogue/conversation)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Type d’interface utilisateur (pop-up/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID de session</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Événements de réservation de réunions {#meeting-booking-events}

Ces événements sont déclenchés lorsqu’un visiteur organise une réunion avec votre représentant commercial.

Vous trouverez ci-dessous les événements qui entrent dans cette catégorie.

### Réunion programmée {#meeting-booked}

Cet événement est déclenché lorsqu’un visiteur choisit de réserver une réunion sur le calendrier d’un agent.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => { 
 // code here will execute when a meeting is booked 
    }); 
});
```

La variable `event` est un objet avec des métadonnées liées à la conversation. Vous pouvez accéder à ces métadonnées en accédant à `event.data`.

Vous trouverez ci-dessous quelques valeurs de métadonnées clés auxquelles vous pouvez accéder.

<table>
<thead>
  <tr>
    <th style="width:75%">Métadonnées</th>
    <th style="width:25%">Attributs</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nom de la conversation</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identifiant de conversation</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Type de conversation (flux de dialogue/conversation)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Type d’interface utilisateur (pop-up/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID de session</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Nom de l'agent</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Identifiant d'agent</td>
    <td>payload.agentID</td>
  </tr>
  <tr>
    <td>Informations sur la réunion</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## Événements de conversation en direct {#live-chat-events}

Ces événements sont déclenchés lorsqu’un visiteur se connecte à un agent en direct au cours de son engagement avec le chatterbot.

Vous trouverez ci-dessous les événements qui entrent dans cette catégorie.

### Chat en direct demandé {#live-chat-requested}

Cet événement est déclenché lorsqu’un visiteur sélectionne l’option permettant de discuter avec un agent actif et qu’un agent disponible est en cours de résolution.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => { 
 // code here will execute when a visitor requests for live chat 
    }); 
});
```

### Démarrage de tchat en direct {#live-chat-initiated}

Cet événement est déclenché lorsqu’un visiteur sélectionne l’option permettant de discuter avec un agent actif et qu’un agent accepte la conversation.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => { 
 // code here will execute after a live agent accepted the chat 
    }); 
});
```

### Fin de la conversation en direct {#live-chat-ended}

Cet événement est déclenché lorsqu’une conversation entre un visiteur et l’agent actif se termine.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => { 
 // code here will execute when a live chat is ended 
    }); 
});
```

### Délai d’expiration de conversation en direct {#live-chat-timeout}

Cet événement est déclenché lorsqu’une conversation en direct expire, car le visiteur cesse de répondre ou il a abandonné.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => { 
 // code here will execute when a visitor abandoned live chat 
    }); 
});
```

La variable `event` est un objet avec des métadonnées liées à la conversation. Vous pouvez accéder à ces métadonnées en accédant à `event.data`.

Vous trouverez ci-dessous quelques valeurs de métadonnées clés auxquelles vous pouvez accéder.

<table>
<thead>
  <tr>
    <th style="width:75%">Métadonnées</th>
    <th style="width:25%">Attributs</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nom de la conversation</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identifiant de conversation</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Type de conversation (flux de dialogue/conversation)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Type d’interface utilisateur (pop-up/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID de session</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Nom de l'agent</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Identifiant d'agent</td>
    <td>payload.agentID</td>
  </tr>
</tbody>
</table>

Si vous souhaitez envoyer l’un de ces événements à une plateforme d’analyse telle qu’Adobe Analytics ou Google Analytics, vous devez ajouter leur appel de suivi respectif dans ces événements de Dynamic Chat. Cela ressemblerait à l’exemple ci-dessous.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // Enter Adobe Analytics or Google Analytics function here 
    ga('send', 'event', { 
      eventCategory: Dynamic Chat Conversations', 
      eventAction: 'Conversation Triggered', 
      eventLabel: event.data.payload.id, 
    }); 
    }); 
});
```
