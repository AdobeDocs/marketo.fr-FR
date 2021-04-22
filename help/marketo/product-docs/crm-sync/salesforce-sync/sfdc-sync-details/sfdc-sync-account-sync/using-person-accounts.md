---
unique-page-id: 4719316
description: Utilisation de comptes personnels - Documents Marketo - Documentation du produit
title: Utilisation de comptes personnels
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Utilisation de comptes personnels {#using-person-accounts}

Les comptes personnels peuvent être configurés dans Salesforce pour répondre aux besoins de votre organisation. Voici comment Marketo traite les comptes des personnes.

>[!NOTE]
>
>Les comptes Salesforce par défaut sont des comptes professionnels. Votre administrateur Salesforce doit configurer des comptes de personnes séparément.

## Qu&#39;est-ce qu&#39;un compte de personne ? {#what-is-a-person-account}

Un compte de personne est très similaire à l’objet de compte dans Salesforce. Cependant, un compte de personne a accès à la fois aux champs du compte et aux champs de contact.

## Que se passe-t-il lorsqu’un compte personnel est synchronisé sur Marketo ? {#what-happens-when-a-person-account-is-synced-to-marketo}

Un compte de personne est synchronisé avec Marketo en tant que société et en tant que personne.

>[!NOTE]
>
>Les champs personnalisés d’un compte de personne sont copiés dans la société et dans la personne de Marketo.

## Comment puis-je différencier les comptes professionnels et les comptes personnels ? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Utilisez le filtre **Est-ce que le compte de personne** de votre liste intelligente pour séparer les comptes de personne des comptes d&#39;entreprise standard.

## Où les informations de mes comptes personnels sont-elles affichées dans Marketo Sales Insight ? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Les Activités relatives aux comptes personnels sont affichées dans le panneau **Compte**.

>[!NOTE]
>
>Les options **Ajouter à Campaign** et **Envoyer un courriel** de Marketo Sales Insight ne sont pas actuellement disponibles pour les comptes de personnes.

## Comment associer des opportunités à un compte de personne ? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo dépend du rôle de contact d&#39;opportunité pour déterminer à quelle personne associer l&#39;opportunité. Vous devez ajouter le rôle de contact d&#39;opportunité pour chaque compte de personne afin de connecter l&#39;opportunité à la personne appropriée à Marketo. Nous vous recommandons de configurer un processus pour ajouter automatiquement le rôle contact opportunité.

## Quel champ de courriel dois-je utiliser pour les comptes de personnes ? {#which-email-field-should-i-use-for-person-accounts}

Il existe deux champs de courrier électronique pour un compte de personne. Utilisez le champ **Adresse électronique** de vos formulaires (et non **Adresse électronique de la personne**) pour vous assurer que la déduplication Marketo et les autres traitements de courrier électronique fonctionnent correctement.
