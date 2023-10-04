---
description: Présentation de la messagerie instantanée - Documents Marketo - Documentation du produit
title: Présentation de la messagerie instantanée
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 870dd6df82c605fffa6681d68867354084988bcd
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 2%

---

# Présentation de la messagerie instantanée {#live-chat-overview}

Le chat en direct permet aux visiteurs du site Web de discuter en temps réel avec vos agents de vente.

## Ajout d’agents de messagerie instantanée {#add-live-chat-agents}

Pour commencer à parler en direct, vous devez ajouter vos agents de chat en direct en tant que [utilisateurs dans Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. Une fois cette opération terminée, vous pouvez ajouter une [carte de conversation en direct](#using-the-live-chat-card) à un dialogue nouveau ou existant.

Lorsque les visiteurs demandent à dialoguer avec un agent via votre dialogue, les agents ont plusieurs [options de notification](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} où ils peuvent commencer à discuter avec le visiteur.

>[!NOTE]
>
>L’avatar de l’agent en direct utilise l’image de profil du profil d’Adobe de l’agent. Pour mettre à jour l’image, suivez [ces étapes](https://helpx.adobe.com/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

## Utilisation de la carte de conversation en direct {#using-the-live-chat-card}

Utilisez la carte de conversation en direct dans le [Concepteur de diffusion](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} lorsque vous souhaitez que les visiteurs discutent avec un agent en direct.

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
