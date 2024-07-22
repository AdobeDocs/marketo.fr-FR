---
unique-page-id: 1147344
description: Glossaire des jetons système - Documents Marketo - Documentation du produit
title: Glossaire des jetons système
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Glossaire des jetons système {#system-tokens-glossary}

En plus des jetons de personne, vous pouvez utiliser des jetons système vraiment cool. Les voici.

>[!NOTE]
>
>Les paramètres de fuseau horaire du compte affectent la date et l’heure d’exécution des jetons.

## system.date {#system-date}

Le jeton `{{system.date}}` affichera la date actuelle au moment de l’exécution comme suit : **8 août 2013**

**Fonctionne dans :**

* Étape de flux [Modifier la valeur de données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* Étape de flux [Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Étape de flux [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* Le corps d&#39;un email ou d&#39;un modèle

## system.time {#system-time}

Le jeton `{{system.time}}` affichera l’heure actuelle au moment de l’exécution comme suit : **04:34 PM (GMT -0700)**

**Fonctionne dans :**

* Étape de flux [Modifier la valeur de données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* Étape de flux [Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Étape de flux [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* Le corps d&#39;un email ou d&#39;un modèle

## system.dateTime {#system-datetime}

Le jeton `{{system.dateTime}}` affichera la date et l’heure actuelles au moment de l’exécution comme suit : **2013-08-08 16:36:13**

**Fonctionne dans :**

* Étape de flux [Modifier la valeur de données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* Étape de flux [Moment intéressant](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Étape de flux [Créer une tâche](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* Le corps d&#39;un email ou d&#39;un modèle

## system.forwardToFriendLink {#system-forwardtofriendlink}

Le jeton `{{system.forwardToFriendLink}}` vous permet de contrôler l’emplacement de [’Forward to a Friend Link’ (Transférer vers un lien d’ami) dans les courriers électroniques](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**Fonctionne dans :**

* [Ajouter un jeton système en tant que lien dans un email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou un modèle

## system.unsubscribeLink {#system-unsubscribelink}

Le jeton `{{system.unsubscribeLink}}` vous permet de contrôler l’emplacement du lien de désabonnement dans un email.

**Fonctionne dans :**

* [Ajouter un jeton système en tant que lien dans un email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou un modèle

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Le jeton `{{system.viewAsWebpageLink}}` vous permet de contrôler l’emplacement du lien Afficher comme page web dans un email.

**Fonctionne avec :**

* [Ajouter un jeton système en tant que lien dans un email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou un modèle
