---
description: Utilisez l’IA dédiée au Marketo pour créer un programme Marketo à partir d’un résumé en langage clair. Préparez les campagnes intelligentes, la planification et les espaces réservés de ressources à examiner et à affiner.
title: Créer un programme
beta: true
hide: true
source-git-commit: f552c0b0219aede39e0742466ab2473e8e924e55
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Créer un programme {#create-program}

Décrivez une campagne marketing en langage clair et Marketo AI créera la structure du programme, avec les espaces réservés aux ressources et la planification.

>[!PREREQUISITES]
>
>* Pour utiliser cette fonctionnalité, vous devez d’abord accepter les termes [&#x200B; Core Gen-AI et les termes supplémentaires](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
>
>* Vous devez disposer des autorisations nécessaires pour créer des programmes sur votre compte Marketo.

## Utilisation {#how-to-use}

1. Dans Mon Marketo, cliquez sur la mosaïque **Créer avec l’IA**.

1. Dans la fenêtre d’invite, saisissez une description de la campagne que vous souhaitez créer. Soyez aussi spécifique ou général que vous le souhaitez (vous pouvez toujours l’affiner).

1. L’IA dédiée au Marketo confirme son interprétation de votre mémoire et répertorie ce qu’elle prévoit de créer. Examinez-le avant sa génération.

1. Confirmez et l’IA dédiée au Marketo crée le programme dans votre environnement.

1. Ouvrez le programme que vous venez de créer dans Marketo et vérifiez sa structure.

1. Remplacez les ressources d’e-mail d’espace réservé par votre contenu réel.

1. Vérifiez que les filtres de campagne intelligents et les étapes de flux correspondent à l’audience et à la logique prévus.

1. Exécutez l’agent [Program QA](/help/marketo/product-docs/marketo-ai/agents/program-qa.md) avant l’activation.

## Cas d’utilisation {#use-cases}

**Programme d’enregistrement de webinaire** : un responsable de campagne tape « Créer un programme d’enregistrement de webinaire pour notre démonstration du produit d’août. Envoyez un e-mail d’invitation, un rappel la veille et un suivi avec le lien d’enregistrement par la suite. » L’IA dédiée à Marketo crée un programme avec trois campagnes intelligentes (invitation, rappel, suivi), des e-mails d’espace réservé pour chacune d’elles et une planification basée sur la date de l’événement.

**Campagne de déclenchement de la notation du lead** : un spécialiste des opérations marketing tape « Créer un programme qui se déclenche lorsqu’un lead atteint une note de 50 et l’envoie à une liste dynamique MQL ». L’IA dédiée au Marketo crée le programme avec une campagne de déclenchement qui écoute le changement de score et une étape de flux qui ajoute le prospect à la liste MQL.

**Culture de réengagement** : un responsable de la génération de la demande demande une série de 3 e-mails de réengagement ciblant les prospects qui ne se sont pas engagés depuis 90 jours. L’IA dédiée au Marketo crée la campagne par lots avec le filtre d’inactivité, trois étapes d’envoi d’e-mails avec les étapes d’attente appropriées entre elles et une étape de flux pour mettre à jour le statut du prospect si quelqu’un se réengage.

**Programme de suivi des événements** : à l’issue d’un salon, un responsable demande à l’IA dédiée à Marketo de créer un programme de suivi post-événement qui envoie un e-mail de remerciement aux participants et un e-mail de remerciement aux inscrits qui ne se sont pas présentés. L’IA dédiée aux Marketo crée deux campagnes intelligentes, une pour chaque segment, avec les filtres et les espaces réservés d’e-mail appropriés.

## Éléments à noter {#things-to-note}

* Ayez une idée claire de ce que la campagne doit faire ; de l’audience, de l’action qui la déclenche (ou s’il s’agit d’un envoi par lots) et de l’objectif.
* Aucun modèle ou formulaire n’est requis au préalable. L’IA dédiée à Marketo crée la structure et vous pouvez connecter les ressources par la suite (vous êtes toujours chargé de rédiger une copie d’e-mail et de configurer les pages de destination).
* Marketo AI ne peut pas accéder automatiquement à vos listes d’audience existantes. Vous devez connecter les filtres de liste dynamique à vos segments réels une fois le programme créé.
* Les programmes complexes à plusieurs étapes avec une logique de branchement avancée peuvent nécessiter un affinement manuel après leur création.
* Si votre environnement Marketo utilise des conventions de nommage ou des structures de dossiers. Spécifiez-les dans votre mémoire afin que le programme soit créé au bon endroit.
