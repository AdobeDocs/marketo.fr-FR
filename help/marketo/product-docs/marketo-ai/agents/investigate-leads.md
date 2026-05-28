---
description: L’agent principal Enquêter répond aux questions les plus fréquentes des spécialistes marketing. Elle est plus rapide et plus fiable que l’exploration manuelle des journaux d’activité, de l’historique des campagnes intelligentes et des enregistrements de notation.
title: Enquête sur les prospects
badge: Beta
hide: true
hidefromtoc: true
source-git-commit: 54702db63ae356706fceba7dc4c09c70e164612f
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 1%

---

# Enquête sur les prospects {#investigate-leads}

Découvrez pourquoi une personne/un prospect spécifique n’a pas atteint un jalon (comme MQL, qualification d’un programme ou une campagne) et obtenez une explication en langage clair de ce qui s’est passé.

>[!PREREQUISITES]
>
>* Pour utiliser cette fonctionnalité, vous devez d’abord accepter les termes [ Core Gen-AI et les termes supplémentaires](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
>
>* Vous devez disposer d’un accès en affichage à l’enregistrement de la personne/du prospect et au programme ou au jalon faisant l’objet de votre enquête.

>[!AVAILABILITY]
>
>Cette fonctionnalité est actuellement en version bêta fermée. Veuillez ne pas diffuser cette documentation.

## Utilisation {#how-to-use}

1. Dans Mon Marketo, cliquez sur la mosaïque **Créer avec l’IA**.

1. Dans la fenêtre d’invite, décrivez l’objet de votre enquête. Indiquez le prospect (par adresse électronique ou nom) et ce qui devait se produire.

   >[!NOTE]
   >
   >Voici quelques exemples : « Pourquoi n’avez-`john.smith@example.com` pas atteint MQL le mois dernier ? » ou « Pourquoi Sato Hanako n’a-t-il pas été ajouté au programme du webinaire du 3e trimestre ? »

1. L’IA dédiée à Marketo récupère les données historiques et pertinentes du prospect.

1. Consultez l’explication. L’IA dédiée au Marketo vous indique la raison spécifique pour laquelle le jalon n’a pas été atteint et, si possible, ce qui doit changer pour que le prospect soit qualifié.

1. Agissez en fonction du résultat : corrigez un problème de données, ajustez un filtre, mettez à jour le score du prospect ou acceptez que le résultat était correct.

## Cas d’utilisation {#use-cases}

**Seuil MQL non atteint** : un responsable de la génération de demandes remarque un prospect que les ventes ont marqué comme intéressé, mais qui n’a jamais atteint MQL. Ils demandent : « Pourquoi n’avez-`david.chen@techcorp.com` pas atteint MQL ? » L’IA dédiée au Marketo constate que le score comportemental du prospect est de 42 (8 points en dessous du seuil MQL de 50) et répertorie les activités de notation qui ont contribué. Ils peuvent voir exactement quels comportements pousseraient le prospect au-delà du seuil.

**Ignorer la campagne en raison de la suppression** : un responsable de campagne demande pourquoi un contact spécifique n&#39;a pas reçu un e-mail d&#39;invitation qui est allé au reste de la liste. L’IA dédiée au Marketo trouve que le contact est sur la liste marketing suspendue, ce qui l’exclut automatiquement de tous les envois de Campaign. Le responsable communique directement avec eux pour enquêter sur les raisons pour lesquelles ils ont été supprimés.

**Échec de qualification du programme** : un spécialiste des opérations marketing tente de résoudre les problèmes pourquoi un prospect qui a assisté à un webinaire n’a pas été ajouté au programme de suivi post-événement. L’IA dédiée à Marketo suit le problème : le prospect s’est enregistré mais a été marqué comme « Pas d’affichage » dans le programme d’événement, et le filtre de campagne de suivi nécessite le statut « Participé ». Le statut n’a pas été défini correctement dans l’intégration.

## Éléments à noter {#things-to-note}

* L’enquête de lead explique ce qui s’est passé en fonction de la configuration et de l’activité enregistrées Marketo. Il ne peut pas expliquer les décisions prises en dehors de Marketo (par exemple, pourquoi un prospect a été supprimé manuellement par un collègue).
* Si l’historique des activités d’un prospect est très long, l’IA dédiée au Marketo se concentre sur les événements les plus récents et les plus pertinents liés à votre question.
* L’enquête de lead est en lecture seule. Il vous indique ce qui s’est passé, mais n’apporte aucune modification à l’enregistrement du prospect ou à l’appartenance au programme.
* Pour les problèmes qui s’avèrent être des problèmes de qualité des données (valeurs de champ manquantes, source de lead incorrecte), la correction doit être effectuée manuellement dans l’enregistrement du lead.
* Si l’enquête révèle un problème de logique de campagne intelligente affectant de nombreux prospects, utilisez l’assurance qualité du programme pour examiner la configuration complète du programme.
