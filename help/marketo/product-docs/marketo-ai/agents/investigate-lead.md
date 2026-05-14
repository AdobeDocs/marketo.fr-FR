---
description: L’agent principal Enquêter répond aux questions les plus fréquentes des spécialistes marketing. Elle est plus rapide et plus fiable que l’exploration manuelle des journaux d’activité, de l’historique des campagnes intelligentes et des enregistrements de notation.
title: Examiner le prospect
beta: true
hide: true
hidefromtoc: true
source-git-commit: a2c170ced2119a86ffe1f2da1bde212afa4841f0
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%

---

# Examiner le prospect {#investigate-lead}

Découvrez pourquoi une personne/un prospect spécifique n’a pas atteint un jalon (comme MQL, qualification d’un programme ou une campagne) et obtenez une explication en langage clair de ce qui s’est passé.

>[!PREREQUISITES]
>
>Vous devez disposer d’un accès en affichage à l’enregistrement du prospect et au programme ou au jalon faisant l’objet de votre enquête.

## Fonctionnement

Vous indiquez à l’IA dédiée au Marketo le prospect faisant l’objet de l’enquête et le jalon ou le résultat attendu. L’IA dédiée au Marketo examine l’historique des activités du prospect, l’enregistrement de notation, l’appartenance à un programme, l’historique de qualification de la campagne intelligente et tous les filtres ou règles de suppression pertinents. Elle renvoie ensuite une explication claire de ce qui a bloqué ou retardé le résultat attendu ; par exemple, « Ce lead a atteint le score 48, mais le seuil MQL est de 50 » ou « Ce lead a été exclu de la campagne parce qu’il s’est désabonné le 3 mars ».

## Utilisation {#how-to-use}

1. Dans Mon Marketo, cliquez sur la mosaïque **Créer avec l’IA**.

1. Dans la fenêtre d’invite, décrivez l’objet de votre enquête. Indiquez le prospect (par adresse électronique ou nom) et ce qui devait se produire.

>[!NOTE]
>
>Voici quelques exemples : « Pourquoi n’avez-`john.smith@example.com` pas atteint MQL le mois dernier ? » ou « Pourquoi Brenda Gonzales n’a-t-elle pas été ajoutée au programme de webinaires du 3e trimestre ? »

1. L’IA dédiée à Marketo récupère les données historiques et pertinentes du prospect.

1. Consultez l’explication. L’IA dédiée au Marketo vous indique la raison spécifique pour laquelle le jalon n’a pas été atteint et, si possible, ce qui doit changer pour que le prospect soit qualifié.

1. Agissez en fonction du résultat : corrigez un problème de données, ajustez un filtre, mettez à jour le score du prospect ou acceptez que le résultat était correct.

## Exemples

Seuil **MQL non atteint**
Un responsable de la génération de demandes remarque un prospect que les ventes ont marqué comme intéressé mais qui n’a jamais atteint MQL. Elle demande : « Pourquoi david.chen@techcorp.com n&#39;a-t-il pas atteint MQL ? » Marketo AI constate que le score comportemental du prospect est de 42 (8 points en dessous du seuil MQL de 50) et répertorie les activités de notation qui ont contribué. Elle peut voir exactement quels comportements pousseraient le prospect au-delà du seuil.

**Campagne ignorée en raison de la suppression**
Une responsable de campagne demande pourquoi un contact spécifique n’a pas reçu un e-mail d’invitation qui est allé au reste de sa liste. L’IA dédiée au Marketo trouve que le contact est sur la liste marketing suspendue, ce qui l’exclut automatiquement de tous les envois de Campaign. Le responsable contacte directement le contact pour enquêter sur la raison pour laquelle il a été supprimé.

**Échec de qualification du programme**
Un spécialiste des opérations marketing tente de déterminer pourquoi un prospect qui a assisté à un webinaire n’a pas été ajouté au programme de suivi post-événement. L’IA dédiée à Marketo suit le problème : le prospect s’est enregistré mais a été marqué comme « Pas d’affichage » dans le programme d’événement, et le filtre de campagne de suivi nécessite le statut « Participé ». Le statut n’a pas été défini correctement dans l’intégration.

**Le plomb coincé dans une culture**
Un responsable de génération de demandes remarque qu’un prospect se trouve au même stade de maturation depuis 90 jours sans progresser. Elle demande à Marketo AI d&#39;enquêter. Elle constate que le score d’engagement du prospect a chuté en dessous du seuil requis pour passer à l’étape suivante, et que le prospect n’a pas ouvert d’e-mail depuis 60 jours, ce qui le qualifie plutôt pour la branche de réengagement.

## Conseils et restrictions

* L’enquête de lead explique ce qui s’est passé en fonction de la configuration et de l’activité enregistrées dans Marketo. Elle ne peut pas expliquer les décisions prises en dehors de Marketo (p. ex. pourquoi un lead a été supprimé manuellement par un collègue).
* Si l’historique des activités d’un prospect est très long, l’IA dédiée au Marketo se concentre sur les événements les plus récents et les plus pertinents liés à votre question.
* L’enquête de lead est en lecture seule. Elle vous indiquera ce qui s’est passé, mais ne modifiera pas l’enregistrement du lead ni l’appartenance au programme.
* Pour les problèmes qui s’avèrent être des problèmes de qualité des données (valeurs de champ manquantes, source de lead incorrecte), la correction devra être effectuée manuellement dans l’enregistrement du lead.
* Si l’enquête révèle un problème de logique de campagne intelligente affectant de nombreux prospects, utilisez l’assurance qualité du programme pour examiner la configuration complète du programme.
