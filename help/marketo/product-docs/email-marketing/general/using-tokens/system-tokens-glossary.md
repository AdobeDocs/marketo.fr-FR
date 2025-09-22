---
unique-page-id: 1147344
description: Glossaire Des Jetons Système - Documents Marketo - Documentation Du Produit
title: Glossaire des jetons système
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---

# Glossaire des jetons système {#system-tokens-glossary}

En plus des jetons de personne, vous pouvez utiliser des jetons système vraiment cool. Les voilà.

>[!NOTE]
>
>Les paramètres de fuseau horaire de votre compte affectent l’exécution des jetons de date et d’heure.

## system.date {#system-date}

Le jeton `{{system.date}}` effectue le rendu de la date actuelle au moment de l’exécution comme suit : **8 août 2013**

**Fonctionne dans :**

* Étape de flux [ Modifier la valeur des données ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* [Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} étape de flux
* [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} étape de flux
* Corps d’un e-mail ou d’un modèle

## system.time {#system-time}

Le jeton `{{system.time}}` rendra l’heure actuelle au moment de l’exécution comme suit : **04:34 PM (GMT -0700)**

**Fonctionne dans :**

* Étape de flux [ Modifier la valeur des données ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* [Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} étape de flux
* [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} étape de flux
* Corps d’un e-mail ou d’un modèle

## system.dateTime {#system-datetime}

Le jeton `{{system.dateTime}}` rendra la date et l’heure actuelles au moment de l’exécution comme suit : **2013-08-08 16:36:13**

**Fonctionne dans :**

* Étape de flux [ Modifier la valeur des données ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* [Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} étape de flux
* [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} étape de flux
* Corps d’un e-mail ou d’un modèle

## system.forwardToFriendLink {#system-forwardtofriendlink}

Le jeton `{{system.forwardToFriendLink}}` vous permet de contrôler l’emplacement du [ « Transférer vers un lien d’ami » dans les e-mails](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**Fonctionne dans :**

* [Ajouter un jeton système en tant que lien dans un e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou modèle

## system.unsubscribeLink {#system-unsubscribelink}

Le jeton `{{system.unsubscribeLink}}` permet de contrôler le placement du lien de désabonnement dans un e-mail.

**Fonctionne dans :**

* [Ajouter un jeton système en tant que lien dans un e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou modèle

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Le jeton `{{system.viewAsWebpageLink}}` permet de contrôler le positionnement du lien Afficher en tant que page web dans un e-mail.

**Fonctionne avec :**

* [Ajouter un jeton système en tant que lien dans un e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou modèle
