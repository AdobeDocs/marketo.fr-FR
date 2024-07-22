---
unique-page-id: 4719316
description: Utilisation de comptes de personne - Documents Marketo - Documentation du produit
title: Utilisation de comptes de personne
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Utilisation de comptes de personne {#using-person-accounts}

Les comptes de personne peuvent être configurés dans Salesforce pour répondre aux besoins de votre entreprise. Voici comment Marketo Engage traite les comptes de personnes.

>[!NOTE]
>
>Les comptes Salesforce par défaut sont des comptes d’entreprise. Votre administrateur Salesforce doit configurer des comptes de personne séparément.

## Qu&#39;est-ce qu&#39;un compte de personne ? {#what-is-a-person-account}

Un compte de personne est très similaire à l’objet de compte dans Salesforce. Cependant, un compte de personne a accès aux champs du compte et aux champs de contact.

## Que se passe-t-il lorsqu’un compte de personne est synchronisé avec Marketo ? {#what-happens-when-a-person-account-is-synced-to-marketo}

Un compte de personne est synchronisé avec Marketo en tant qu’entreprise et en tant que personne.

>[!NOTE]
>
>Les champs personnalisés d’un compte de personne sont copiés dans la société et dans la personne dans Marketo.

## Comment puis-je différencier les comptes de commerce et de personne ? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Utilisez le filtre &quot;Compte de personne&quot; de votre liste dynamique pour séparer les comptes de personne des comptes professionnels standard.

## Où les informations de mes comptes de personne sont-elles affichées dans Marketo Sales Insight ? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Les activités liées aux comptes de personnes s’affichent dans le panneau **[!UICONTROL Compte]**.

>[!NOTE]
>
>Les options **[!UICONTROL Ajouter à la campagne Marketo]** et **[!UICONTROL Envoyer un courrier électronique]** de Marketo Sales Insight ne sont actuellement pas disponibles pour les comptes de personne.

## Comment associer des opportunités à un compte de personne ? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo dépend du rôle de contact de l’opportunité pour déterminer la personne à laquelle associer l’opportunité. Vous devez ajouter le rôle de contact d’opportunité pour chaque compte de personne afin de connecter l’opportunité à la personne appropriée dans Marketo. Nous vous recommandons de configurer un workflow pour ajouter automatiquement le rôle contact opportunité.

## Quel champ d’adresse électronique dois-je utiliser pour les comptes de personne ? {#which-email-field-should-i-use-for-person-accounts}

Il existe deux champs de courrier électronique pour un compte de personne. Utilisez le champ **Adresse électronique** de vos formulaires (et non l’**adresse électronique de la personne**) pour vous assurer que la déduplication Marketo et d’autres traitements de courrier électronique fonctionnent correctement.
