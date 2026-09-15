---
description: Utilisez Coworker for Marketo Engage pour créer un programme Marketo en adaptant un modèle existant. Préparez les campagnes intelligentes, la planification et les espaces réservés de ressources à examiner et à affiner.
title: Créer des programmes
source-git-commit: 0949e5193333d56943a5c9a52c1715ecbcb274f3
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%
---
# Créer des programmes {#build-programs}

Décrivez une campagne marketing en langage simple et Coworker for Marketo Engage adapte un modèle de programme existant en fonction de vos besoins, en mettant automatiquement à jour le contenu des e-mails et en créant des ressources supplémentaires en dupliquant la structure de votre modèle.

>[!PREREQUISITES]
>
>* Pour utiliser cette fonctionnalité, vous devez d’abord accepter les termes [ Core Gen-AI et les termes supplémentaires](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
>
>* Vous devez être autorisé à créer des programmes dans votre compte Marketo et disposer d’au moins un programme Marketo existant à utiliser comme modèle. Le programme modèle doit contenir au moins un e-mail et une campagne intelligente.

## Utilisation {#how-to-use}

1. Dans Mon Marketo, cliquez sur la mosaïque **Collègue pour Marketo Engage**.

1. Sélectionnez un modèle de programme. Choisissez un programme existant correspondant à votre type de campagne (par exemple, e-mail, webinaire, formation).

1. Dans la fenêtre d’invite, saisissez une description de la campagne que vous souhaitez créer. Soyez aussi spécifique ou général que vous le souhaitez (vous pouvez toujours l’affiner).

1. Coworker for Marketo Engage confirme son interprétation de votre mémoire et énumère ce qu&#39;il prévoit de créer. Examinez-le avant sa génération.

1. Confirmez et Coworker for Marketo Engage crée le programme dans votre environnement.

1. Ouvrez le programme que vous venez de créer dans Marketo et vérifiez sa structure.

1. Remplacez les ressources d’e-mail d’espace réservé par votre contenu réel.

1. Vérifiez que les filtres et les étapes de flux de Campagne intelligente correspondent à l’audience et à la logique prévus.

1. Une fois toutes les améliorations manuelles effectuées (configurer la logique de campagne intelligente, finaliser les filtres, personnaliser le contenu des e-mails), exécutez [Valider les programmes](/help/marketo/product-docs/coworker-for-marketo/skills/validate-programs.md) pour vous assurer que vos modifications sont conformes à vos règles d’organisation avant l’activation.

## Cas d’utilisation {#use-cases}

**Programme d’enregistrement de webinaire** : un responsable de campagne tape « Créer un programme d’enregistrement de webinaire pour notre démonstration du produit d’août. Envoyez un e-mail d’invitation, un rappel la veille et un suivi avec le lien d’enregistrement par la suite. » Coworker for Marketo Engage crée un programme avec trois campagnes intelligentes (invitation, rappel, suivi), des e-mails d’espace réservé pour chacune d’elles et une planification basée sur la date de l’événement.

**Campagne de déclenchement de la notation du lead** : un spécialiste des opérations marketing tape « Créer un programme qui se déclenche lorsqu’un lead atteint une note de 50 et l’envoie à une liste dynamique MQL ». Coworker for Marketo Engage crée le programme avec une campagne de déclenchement qui écoute le changement de score et une étape de flux qui ajoute le prospect à la liste MQL.

**Culture de réengagement** : un responsable de la génération de la demande demande une série de 3 e-mails de réengagement ciblant les prospects qui ne se sont pas engagés depuis 90 jours. Coworker for Marketo Engage crée la campagne par lots avec le filtre d’inactivité, trois étapes d’envoi d’e-mails avec les étapes d’attente appropriées entre elles et une étape de flux pour mettre à jour le statut du prospect si quelqu’un se réengage.

**Programme de suivi des événements** : après un salon professionnel, un responsable demande à Coworker for Marketo Engage de créer un programme de suivi post-événement qui envoie un e-mail de remerciement aux participants et un e-mail de remerciement aux inscrits qui ne se sont pas présentés. Coworker for Marketo Engage crée deux campagnes intelligentes, une pour chaque segment, avec les filtres et les espaces réservés d’e-mail appropriés.

>[!NOTE]
>
>Dans chacun des exemples ci-dessus, Coworker clone un modèle de programme existant (un simple e-mail ou un programme d’événement avec une structure de base) et crée les e-mails et campagnes supplémentaires en dupliquant les ressources du modèle et en mettant à jour leur contenu. Les étapes et les filtres du flux de campagne intelligente sont adaptés si possible, mais peuvent nécessiter un affinement manuel pour correspondre à la logique spécifique de la campagne.

## Éléments à noter {#things-to-note}

* Ayez une idée claire de ce que la campagne doit faire, de l’audience, de l’action qui la déclenche (ou s’il s’agit d’un envoi par lots) et de l’objectif.
* La sélection du modèle est obligatoire. Choisissez un modèle avec au moins un e-mail et une campagne intelligente. L’outil ne peut pas fonctionner avec des modèles vides.
* Le contenu des e-mails est généré automatiquement, mais les filtres de campagne intelligente et les étapes de flux restent manuels. Vous devez configurer la logique après la création pour qu’elle corresponde au comportement prévu de votre campagne.
* Les ressources supplémentaires sont créées par duplication. Si votre brief appelle 4 emails mais que votre modèle en comporte 1, l’outil crée 3 doublons. Examinez-les toutes pour assurer la cohérence ; elles héritent de la conception et de la structure du modèle.
* Coworker for Marketo Engage ne peut pas accéder automatiquement à vos listes d’audience existantes. Vous devez configurer manuellement les filtres de liste dynamique pour cibler vos segments réels une fois le programme créé.
* Les programmes complexes à plusieurs étapes avec une logique de branchement avancée peuvent nécessiter un affinement manuel après leur création.
* Si votre environnement Marketo utilise des conventions de nommage ou des structures de dossiers, spécifiez-les dans votre résumé afin que le programme soit créé au bon endroit.
