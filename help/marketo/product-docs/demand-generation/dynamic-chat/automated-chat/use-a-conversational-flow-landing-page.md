---
description: Utilisation d’une page d’entrée de flux de conversation - Documents Marketo - Documentation du produit
title: Utilisation d’une page d’entrée de flux de conversation
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 1%

---

# Utilisation d’une page d’entrée de flux de conversation{#use-a-conversational-flow-landing-page}

L’incorporation d’un flux de conversation de Dynamic Chat directement dans une page d’entrée de Marketo Engage permet aux visiteurs de planifier une réunion par l’intermédiaire d’un Dynamic Chat sans avoir à remplir un formulaire ni à interagir avec un chatterbot.

>[!PREREQUISITES]
>
>Créez un simple [flux de conversation](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md) qui contient uniquement une carte **réservation de réunions**.

## Pages d’entrée guidées {#guided-landing-pages}

Incorporez le code suivant dans votre modèle de page d’entrée guidée : `<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`.

Ouvrez votre modèle de page d’entrée guidée dans l’éditeur et sélectionnez l’espace réservé Flux de conversation .

Cliquez sur le menu déroulant Flux de conversation et sélectionnez le CF que vous avez créé à l’étape 1.

Conservez toujours le type de diffusion **En ligne**. Cliquez sur **Insérer**.

Le flux de conversation que vous venez de saisir s’affiche sous la forme d’un élément à droite.

CAPTURE D’ÉCRAN

>[!NOTE]
>
>Pour l’instant, le flux de conversation n’apparaîtra pas dans la fenêtre d’aperçu principale.

## Pages d’entrée de forme libre {#free-form-landing-pages}

Texte


NOTES DE LA RÉUNION DÉTAILLÉE

lp guidé, nouvel id div pour le modèle, choisissez enchaînement conv

liste à structure libre, apportez une icône - attention : ajoutez une note : lorsque vous placez cf sur l’éditeur, il ne vous affiche pas d’aperçu (pas d’espace réservé non plus) - &quot;vous ne verrez pas d’aperçu&quot; - dans la barre latérale, vous verrez que les cf sont sur la page - la liste guidée la répertorie comme élément - utilisez &quot;à ce moment&quot; pour expliquer - la fonctionnalité est en ligne peut-être la semaine du 22e

