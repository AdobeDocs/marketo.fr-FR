---
unique-page-id: 4719316
description: Utilisation Des Comptes De Personne - Documents Marketo - Documentation Du Produit
title: Utilisation de comptes de personnes
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 2%

---

# Utilisation de comptes de personnes {#using-person-accounts}

Les comptes de personne peuvent être configurés dans Salesforce en fonction des besoins de votre entreprise. Voici comment Marketo Engage traite les comptes de personnes.

>[!NOTE]
>
>Les comptes [!DNL Salesforce] par défaut sont des comptes professionnels. Votre administrateur [!DNL Salesforce] doit configurer les comptes de personnes séparément.

## Qu’est-ce qu’un compte personnel ? {#what-is-a-person-account}

Un compte de personne est très similaire à l’objet de compte dans [!DNL Salesforce]. Cependant, un compte de personne a accès aux champs de compte et aux champs de contact.

## Que se passe-t-il lorsqu’un compte de personne est synchronisé avec Marketo ? {#what-happens-when-a-person-account-is-synced-to-marketo}

Un compte de personne est synchronisé avec Marketo en tant que société et en tant que personne.

>[!NOTE]
>
>Les champs personnalisés d’un compte de personne sont copiés à la fois dans la société et dans la personne dans Marketo.

## Comment faire la distinction entre les comptes professionnels et les comptes personnels ? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Utilisez le filtre « Est un compte de personne » dans votre liste dynamique pour séparer les comptes de personne des comptes professionnels standard.

## Où se trouvent les informations sur mes comptes de personne dans Marketo Sales Insight ? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Les activités liées aux comptes de personne s’affichent dans le panneau **[!UICONTROL Compte]**.

>[!NOTE]
>
>Les options Marketo Sales Insight **[!UICONTROL Ajouter à Marketo Campaign]** et **[!UICONTROL Envoyer un e-mail]** ne sont actuellement pas disponibles pour les comptes de personne.

## Comment associer des opportunités à un compte de personne ? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo dépend du rôle du contact de l’opportunité pour déterminer à quelle personne associer l’opportunité. Vous devez ajouter le rôle de contact de l’opportunité pour chaque compte de personne afin de connecter l’opportunité à la personne appropriée dans Marketo. Nous vous recommandons de configurer un workflow pour ajouter automatiquement le rôle de contact d’opportunité.

## Quel champ d’e-mail dois-je utiliser pour les comptes de personne ? {#which-email-field-should-i-use-for-person-accounts}

Il existe deux champs d’adresse électronique pour un compte de personne. Utilisez le champ **[!UICONTROL Adresse e-mail]** dans vos formulaires (et non l’**[!UICONTROL Adresse e-mail de la personne]**) pour vous assurer que la déduplication des Marketo et tout autre traitement des e-mails fonctionnent correctement.
