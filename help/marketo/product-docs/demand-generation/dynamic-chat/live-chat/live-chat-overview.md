---
description: Présentation de la messagerie instantanée - Documents Marketo - Documentation du produit
title: Présentation de la messagerie instantanée
feature: Dynamic Chat
source-git-commit: 9a8f6fe57b585ba0eac6a577bf99e0419d8818a1
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 3%

---

# Présentation de la messagerie instantanée {#live-chat-overview}

Utilisez la carte de conversation en direct dans le [Concepteur de diffusion](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} lorsque vous souhaitez que les visiteurs discutent avec un agent en direct.

## Utilisation de la carte de conversation en direct {#using-the-live-chat-card}

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
   <td>Toutes les règles personnalisées sont analysées lors de la prise en compte de l’emplacement du visiteur. Si le visiteur n’est éligible à aucune règle personnalisée, il obtient la variable <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">message de secours de la conversation en direct</a>.</td>
  </tr> 
  <tr> 
   <td><b>Équipe</b></td>
   <td>Choisissez une équipe spécifique pour recevoir la conversation. Si cette option est sélectionnée, elle se verra attribuer un tourbillon au sein de cette équipe.</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Boîte de réception de l’agent(e)](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}