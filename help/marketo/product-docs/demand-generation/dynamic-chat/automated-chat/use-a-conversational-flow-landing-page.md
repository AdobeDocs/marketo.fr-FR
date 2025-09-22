---
description: Utiliser une page de destination de flux de conversation - Documents Marketo - Documentation du produit
title: Utiliser une page de destination de flux de conversation
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 2%

---

# Utiliser une page de destination de flux de conversation{#use-a-conversational-flow-landing-page}

L’incorporation d’un flux de conversation Dynamic Chat directement dans une page de destination Marketo Engage permet aux visiteurs de planifier une réunion via Dynamic Chat sans avoir à remplir un formulaire ou interagir avec un bot conversationnel.

>[!PREREQUISITES]
>
>Créez un [Flux de conversation](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md) simple contenant uniquement une carte **Réservation de réunion**.

## Pages de destination guidées {#guided-landing-pages}

Insérez le code suivant dans votre modèle de page de destination guidée : `<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`.

Ouvrez votre modèle de page de destination guidée dans l’éditeur et sélectionnez l’espace réservé Flux de conversation .

Cliquez sur le menu déroulant Flux de conversation et sélectionnez le CF que vous avez créé à l’étape 1.

Conservez toujours le type de diffusion **En ligne**. Cliquez sur **Insérer**.

Le flux de conversation que vous venez d’entrer s’affiche sous la forme d’un élément à droite.

CAPTURE D’ÉCRAN

>[!NOTE]
>
>À ce stade, le flux de conversation n’apparaîtra pas dans la fenêtre d’aperçu principale.

## Pages de destination à structure libre {#free-form-landing-pages}

Texte

NOTES DE LA RÉUNION DE STEVE

lp guidée, nouvel identifiant div pour le modèle, choisissez conv flow

lp à structure libre, icône de survol - mise en garde : ajouter une note - lorsque vous placez cf sur l’éditeur, il ne vous affiche pas d’aperçu (pas d’espace réservé non plus) - « vous ne verrez pas d’aperçu » - sur la barre latérale, ils verront que le cf est sur la page - le lp guidé le répertorie comme un élément - utilisez « à ce moment » lors de l’explication - la fonctionnalité est activée peut-être la semaine du 22
