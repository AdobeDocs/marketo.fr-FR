---
unique-page-id: 1147344
description: Glossaire des jetons système - Documents Marketo - Documentation du produit
title: Glossaire des jetons système
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Glossaire des jetons système {#system-tokens-glossary}

En plus des jetons de personne, vous pouvez utiliser des jetons système vraiment cool. Les voici.

>[!NOTE]
>
>Les paramètres de fuseau horaire du compte affectent la date et l’heure d’exécution des jetons.

## system.date {#system-date}

Le `{{system.date}}` token affiche la date actuelle au moment de l’exécution comme suit : **8 août 2013**

**Fonctionne dans :**

* [Modifier la valeur des données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} étape de flux
* [Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} étape de flux
* [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} étape de flux
* Le corps d&#39;un email ou d&#39;un modèle

## system.time {#system-time}

Le `{{system.time}}` jeton affiche l’heure actuelle au moment de l’exécution comme suit : **04:34 PM (GMT -0700)**

**Fonctionne dans :**

* [Modifier la valeur des données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} étape de flux
* [Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} étape de flux
* [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} étape de flux
* Le corps d&#39;un email ou d&#39;un modèle

## system.dateTime {#system-datetime}

Le `{{system.dateTime}}` jeton affiche la date et l’heure actuelles au moment de l’exécution comme suit : **2013-08-08 16:36:13**

**Fonctionne dans :**

* [Modifier la valeur des données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} étape de flux
* [Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} étape de flux
* [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} étape de flux
* Le corps d&#39;un email ou d&#39;un modèle

## system.forwardToFriendLink {#system-forwardtofriendlink}

Le `{{system.forwardToFriendLink}}` vous permet de contrôler l’emplacement de la variable [&quot;Transfert vers un lien d’ami&quot; dans les courriels](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**Fonctionne dans :**

* [Ajout d’un jeton système en tant que lien dans un courrier électronique](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou modèle

## system.unsubscribeLink {#system-unsubscribelink}

Le `{{system.unsubscribeLink}}` token vous permet de contrôler l’emplacement du lien de désabonnement dans un email.

**Fonctionne dans :**

* [Ajout d’un jeton système en tant que lien dans un courrier électronique](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou modèle

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Le `{{system.viewAsWebpageLink}}` token vous permet de contrôler l’emplacement du lien Afficher comme page web dans un email.

**Fonctionne avec :**

* [Ajout d’un jeton système en tant que lien dans un courrier électronique](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou modèle
