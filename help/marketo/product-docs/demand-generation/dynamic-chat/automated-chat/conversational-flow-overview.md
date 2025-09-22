---
description: Présentation du flux de conversation - Documents Marketo - Documentation du produit
title: Vue d’ensemble du flux conversationnel
feature: Dynamic Chat
exl-id: c741886d-d672-471f-8902-208d25898afa
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 3%

---

# Vue d’ensemble du flux conversationnel {#conversational-flow-overview}

Concevez un flux de conversation et déclenchez-le pour tout visiteur en fonction d’une action spécifique (par exemple, cliquer sur un bouton call-to-action, au chargement de la page, temps passé sur la page, etc.).

![](assets/conversational-flow-overview-1.png)

## Dialogues et flux de conversation {#dialogues-vs-conversational-flows}

Bien que les boîtes de dialogue et les flux de conversation aient plusieurs similitudes, il s’agit de deux fonctionnalités distinctes.

<table>
 <tbody>
  <tr>
   <th style="width:50%">Dialogues</th>
   <th style="width:50%">Flux conversationnels</th>
  </tr>
  <tr>
   <td>Les boîtes de dialogue sont ciblées : vous concevez une conversation pour une page et une audience spécifiques en fonction des paramètres que vous avez implémentés.</td>
   <td>Les flux de conversation sont déclenchés : vous concevez une conversation qui peut être déclenchée en fonction de l’action d’un visiteur, comme remplir un formulaire, cliquer sur un lien, etc.</td>
  </tr>
   <tr>
   <td>Pris en charge uniquement dans l’interface du bot conversationnel.</td>
   <td>Actuellement pris en charge dans une interface pop-up, avec d’autres interfaces prévues.</td>
  </tr>
  </tr>
   <tr>
   <td>Il est possible de créer plusieurs boîtes de dialogue pour le même segment de prospects, avec un ordre de priorité afin que chaque visiteur puisse voir la boîte de dialogue en séquence par priorité au fur et à mesure qu’il poursuit son engagement.</td>
   <td>Les flux de conversation n’ont pas d’ordre de priorité et peuvent être déclenchés un certain nombre de fois par le même prospect en fonction du call-to-action déterminé.</td>
  </tr>
  <tr>
   <td>Les conversations du bot conversationnel sont alimentées par des boîtes de dialogue.</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Forms de conversation</a> dans Marketo Engage est optimisé par les flux de conversation.</td>
  </tr>
 </tbody>
</table>

## Onglet Designer de diffusion {#stream-designer-tab}

Le flux Designer pour les flux de conversation est presque identique à celui des boîtes de dialogue. [Pour en savoir plus, cliquez ici](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}.

![](assets/conversational-flow-overview-2.png)

## Onglet Rapports {#reports-tab}

Sous l’onglet Rapports , vous pouvez voir les mesures relatives aux performances de votre flux de conversation.

![](assets/conversational-flow-overview-3.png)

Affichez le taux d’engagement, le taux de conversion, filtrez par visiteurs connus et/ou inconnus, etc.

![](assets/conversational-flow-overview-4.png)

## Onglet Paramètres {#settings-tab}

![](assets/conversational-flow-overview-5.png)

Dans la moitié supérieure de l’onglet Paramètres , vous pouvez mettre à jour le nom du flux de conversation, ajouter une description facultative et modifier la langue.

![](assets/conversational-flow-overview-6.png)

>[!NOTE]
>
>La sélection d’une autre langue modifie uniquement la langue du texte système. Vous êtes responsable de la traduction du contenu.

### SDK des conversations {#conversations-sdk}

Dans la partie inférieure de l’onglet Paramètres , personnalisez le déclencheur de conversation, également appelé SDK de conversations. Vous pouvez décider si la conversation est déclenchée sur votre site web lorsqu’un visiteur clique sur un lien ou au chargement de la page.

![](assets/conversational-flow-overview-7.png)

>[!TIP]
>
>Voir [Conversations SDK](https://experienceleague.adobe.com/tools/marketo-dynamic-chatbot/conversations-sdk/?lang=fr){target="_blank"} en action !

>[!MORELIKETHIS]
>
>[Créer un flux de conversation](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md){target="_blank"}
