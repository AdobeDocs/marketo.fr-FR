---
solution: Marketo Engage
product: marketo
title: Jetons Personalization
description: Découvrez comment utiliser les jetons de personnalisation dans le nouveau Designer d’e-mail de Marketo Engage.
level: Beginner, Intermediate
exl-id: 4828e1a5-822f-48a9-bbb8-b1ffe8421e4f
source-git-commit: 5575ab0d7141d4bfc610430db625439c9f52e231
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Jetons Personalization {#personalization-tokens}

Le Concepteur d’email a un format différent de celui de l’éditeur d’email classique en ce qui concerne les jetons de personnalisation d’email. La modification a été mise en œuvre pour améliorer la compatibilité avec les scripts Handlebar et rationaliser votre processus de création d’e-mail.

>[!AVAILABILITY]
>
>À compter du 23 mai 2025, cette fonctionnalité sera mise en service pour les utilisateurs de Marketo Engage par lots, avec une région mise à jour par semaine. Pendant le déploiement, tous les e-mails créés à l’aide du nouveau concepteur d’e-mail migreront automatiquement les jetons existants vers le nouveau format. Avec cette mise à jour, tous les jetons seront disponibles uniquement en anglais.

## Cas d’utilisation du Principal {#primary-use-case}

Cette amélioration bénéficie principalement aux personnes qui passent du [script Velocity](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting){target="_blank"} au script Handlebar. Le nouveau concepteur d’e-mail ne prend en charge que le nouveau format de jeton. Le format mis à jour élimine les espaces et introduit une structure de texte par défaut révisée, assurant ainsi une expérience de script plus fluide et plus efficace.

## Expérience de jeton {#token-experience}

Aperçu de l’expérience des jetons, à la fois ancienne et nouvelle.

### Ancien format {#old-format}

Dans l’éditeur d’e-mail classique, vous pouvez ajouter des jetons avec des espaces, tels que `lead.Anonymous IP` ou `member.registration code`. Le format du texte par défaut était : `{{lead.City:default=fallback}}`

![](assets/personalization-tokens-1.png){width="800" zoomable="yes"}

### Nouveau format {#new-format}

Dans le concepteur d’e-mail, vous devez utiliser [casse mixte](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) ou des traits de soulignement pour les jetons (par exemple, `lead.anonymousIP` ou `member.registration_code`). Le format du texte par défaut est également remplacé par `{%=lead.city ?: "fallback" %}`.

![](assets/personalization-tokens-2.png){width="800" zoomable="yes"}

## Éléments à noter {#things-to-note}

* L’éditeur de personnalisation propose également les fonctions suivantes pour faciliter la création :

   * Annuler/rétablir
   * Rechercher/Rechercher et remplacer
   * Saisie automatique

* **Tous** les jetons précédemment pris en charge dans Marketo Engage sont pris en charge dans le nouvel éditeur de personnalisation.
