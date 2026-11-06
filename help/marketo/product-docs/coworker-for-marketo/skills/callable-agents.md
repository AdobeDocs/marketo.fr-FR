---
description: Utilisez des agents appelables dans CX Enterprise Coworker for Marketo Engage pour exécuter des étapes d’IA dans les campagnes intelligentes qui nettoient, classent, enrichissent ou filtrent les données de prospect.
title: Agents appelables
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
source-git-commit: 16b8e470bd4a4460c0179ccdd406ef89af7e9e17
workflow-type: tm+mt
source-wordcount: '2002'
ht-degree: 1%
---
# Agents appelables {#callable-agents}

Les agents appelables vous permettent d’utiliser un agent d’IA comme étape dans une campagne intelligente Marketo Engage. Créez un agent dans CX Enterprise Coworker pour Marketo Engage, sélectionnez les champs de prospect qu’il lit et met à jour, puis publiez-les pour les utiliser dans les campagnes. Les agents peuvent aider à nettoyer les données, à classer les prospects, à enrichir les informations manquantes ou à filtrer les envois de formulaire.

>[!PREREQUISITES]
>
>Vous devez disposer de l’autorisation **Accès administrateur** dans Marketo Engage.

## Avant de commencer {#before-you-begin}

- Choisissez les champs de prospect que l’agent doit lire et les champs qu’il doit mettre à jour. Chaque entrée et sortie doit être mappée à un champ de prospect Marketo Engage.
- Vérifiez que les champs de sortie sont modifiables. Les champs en lecture seule et les champs de membre de programme ne sont pas pris en charge.

## Utilisation {#how-to-use}

1. Dans Mon Marketo, cliquez sur la mosaïque **[!UICONTROL CX Enterprise Coworker pour Marketo Engage]**.

1. Sélectionnez **[!UICONTROL Agents appelables]** dans le volet de navigation de gauche. La liste affiche le nom, la date de création, le créateur et le statut de chaque agent. Effectuez une recherche par nom ou un tri par nom ou date de création.

1. Sélectionnez **[!UICONTROL Créer un agent appelant]**. Choisissez un modèle ou laissez le sélecteur de modèle vide pour commencer à partir de zéro.

1. Saisissez un **[!UICONTROL Nom de l’agent]** et écrivez **[!UICONTROL Instructions de l’agent]** décrivant comment traiter chaque prospect.

1. Sous **[!UICONTROL Champs de prospect à envoyer]**, ajoutez les champs de prospect dont l’agent a besoin en tant qu’entrées. Sous **[!UICONTROL Champs de prospect à mettre à jour]**, ajoutez chaque valeur que l’agent doit renvoyer et mappez-la à un champ de prospect modifiable.

1. Sélectionnez **[!UICONTROL Enregistrer]** pour enregistrer un brouillon, ou **[!UICONTROL Enregistrer et publier]** pour rendre l’agent disponible dans Marketo Engage.

1. Ouvrez une campagne dynamique et sélectionnez l’onglet **[!UICONTROL Flux]** . Dans la section Marketing de la liste des étapes de flux, recherchez **Appeler l’agent : _[Nom de l’agent]_**&#x200B;et faites-le glisser dans le flux.

1. Testez la campagne avec un petit ensemble de prospects. Consultez le journal des activités et vérifiez que les champs de sortie se mettent à jour comme prévu avant d’activer la campagne pour tous les prospects.

## Éléments à noter {#things-to-note}

- Un agent appelant traite chaque prospect indépendamment. Marketo Engage envoie les valeurs de prospect mappées à l’agent, écrit les valeurs renvoyées dans les champs de prospect mappés et passe à l’étape suivante de la campagne.
- Vous créez et gérez des agents appelables dans CX Enterprise Coworker pour Marketo Engage. Aucune connexion externe n’est requise.
- Les agents publiés ne sont pas modifiables. Pour modifier un agent déjà publié, vous devez créer un agent et mettre à jour les campagnes intelligentes appropriées.

## Créer un agent {#create-an-agent}

### Créer un agent à partir de zéro {#create-an-agent-from-scratch}

Laissez le sélecteur de modèle vide. Le formulaire commence par un champ d’entrée vide et un champ de sortie vide. Saisissez le nom et les instructions, puis configurez les champs d’entrée et de sortie pour qu’ils correspondent à votre règle métier.

### Démarrer à partir d’un modèle {#start-from-a-template}

Choisissez un modèle pour préremplir les instructions, les champs d’entrée et les champs de sortie. L’agent est enregistré en tant que votre propre copie, que vous pouvez modifier ou supprimer. Si vous supprimez un agent créé à partir d’un modèle, le modèle est à nouveau disponible dans le sélecteur.

| Modèle | But | Entrées | Sorties |
| --- | --- | --- | --- |
| Normaliseur de nom de société | Nettoie les noms de société en supprimant les suffixes légaux, en corrigeant les fautes de frappe courantes et en appliquant des majuscules de marque standard. | Société | Société normalisée (texte) ; degré de confiance (nombre) |
| Téléphone E.164 Formateur | Met en forme les numéros de téléphone selon la norme internationale E.164. | Téléphone | Téléphone normalisé (texte) ; degré de confiance (nombre) |
| Normaliseur de titre de tâche | Standardise les titres de postes et déduit l’ancienneté. | Titre | Titre normalisé (texte); ancienneté (niveau C, vice-président, directeur, gestionnaire, individu ou inconnu); confiance |
| Détecteur de robots et de spams | Signale les envois de formulaires de spam ou de robots. | E-mail, Prénom, Nom, Société, Téléphone | N’est pas (true/false) ; confiance ; raison ; indicateurs (séparés par des virgules) |
| Détecteur d&#39;e-mails jetable | Identifie les adresses email temporaires ou jetables. | E-mail | n’est pas (vrai/faux) ; confiance ; raison ; type d’e-mail (jetable, personnel ou professionnel) ; |
| Classificateur de leads | Segmente les prospects par taille d’entreprise, secteur, persona et intention. | Société, Titre, E-mail, Employés, Chiffre d’affaires | Segment (entreprise, milieu de gamme, PME, démarrage ou inconnu) ; secteur ; persona ; niveau d’intention (élevé, Medium ou faible) ; degré de confiance |
| Enrichissement du lead | Déduit les détails de lead manquants à partir des informations disponibles. | E-mail, titre, entreprise | Entreprise, service, ancienneté déduits, décideur (vrai/faux), B2B (vrai/faux), confiance |
| Recherche sur l&#39;entreprise | Génère des renseignements sur les ventes à partir des informations sur la société. | Société, Site Web, Description | Voir le modèle pour la liste complète |

### Rédiger des instructions efficaces {#write-effective-instructions}

- Insérez des règles générales et des exemples dans les instructions de l’agent. Utilisez les instructions de champ pour spécifier les attentes d’une sortie individuelle.
- Soyez précis. Par exemple, « Supprimer les suffixes légaux tels que Inc, LLC et Corp » est plus clair que « nettoyer les noms de sociétés ».
- Incluez des exemples d’entrées et de sorties attendues, en particulier pour les cas de périphérie.
- Indiquez ce que l’agent doit renvoyer lorsqu’il ne peut pas décider, par exemple « Si vous n’êtes pas sûr, renvoyez la valeur d’origine ».
- Ajoutez une sortie de confiance afin que la logique de campagne puisse acheminer les résultats à faible degré de confiance pour révision.
- Conserver les invites concises. Les invites plus courtes sont plus rapides et moins coûteuses.

## Enregistrer, publier et gérer les agents {#save-publish-and-manage-agents}

### Enregistrer en tant que brouillon ou publier {#save-as-a-draft-or-publish}

Sélectionnez **[!UICONTROL Enregistrer]** pour enregistrer l’agent en tant que brouillon. Les brouillons peuvent être modifiés, mais ne sont pas disponibles en tant qu’étapes de flux de campagne intelligente. Sélectionnez **[!UICONTROL Enregistrer et publier]** lorsque l’agent est prêt. Marketo Engage rend l’agent disponible sous la forme d’une étape de flux et vous renvoie à la liste des agents avec une confirmation de publication. Sélectionnez **[!UICONTROL Annuler]** pour quitter sans enregistrer.

| Statut | Signification | Action disponible |
| --- | --- | --- |
| Brouillon | L’agent est enregistré mais n’est pas disponible dans Marketo Engage. | Modifiez-la, puis sélectionnez **[!UICONTROL Enregistrer et publier]** lorsqu’elle est prête. |
| Publié | L’agent est disponible dans les campagnes intelligentes. Les agents publiés sont figés. | Utilisez l’agent publié ou créez un agent pour apporter des modifications. |
| Échec de la publication | Marketo Engage a rejeté l’agent, par exemple, car un nom de champ de sortie est réservé. Mais l’agent est toujours enregistré en tant que brouillon. | Modifiez l’agent, corrigez le champ nommé dans le message, puis publiez à nouveau. |

### Modifier, vérifier l’utilisation ou supprimer {#edit-check-usage-or-delete}

- Sélectionnez **[!UICONTROL Modifier]** sur un brouillon pour le modifier. **[!UICONTROL Enregistrer]** vous maintient sur la page et affiche une confirmation « Agent enregistré ». Vous pouvez également sélectionner **[!UICONTROL Enregistrer et publier]**, **[!UICONTROL Annuler]** ou **[!UICONTROL Supprimer]**.
- Les agents publiés sont figés, car les campagnes intelligentes peuvent en dépendre. Créez un agent pour apporter des modifications.
- Cochez la case **[!UICONTROL Utilisé par]** pour identifier les campagnes intelligentes qui font référence à un agent avant de supprimer un agent ou de modifier sa configuration de campagne.
- Vous ne pouvez pas supprimer un agent tant qu’une campagne intelligente l’utilise toujours. Supprimez l’étape de flux de l’agent de chaque campagne répertoriée, puis supprimez l’agent.

## Intégration des règles d’organisation {#organizational-rules-integration}

### Conventions de dénomination {#naming-conventions}

- **Nom de l’agent :** 1 à 100 caractères et unique dans l’abonnement. Le nom est également utilisé dans l’étape de flux de campagne intelligente. Choisissez un nom reconnaissable, tel que `Company Name Normalizer`.
- **Nom du champ de sortie :** utilisez des lettres, des chiffres et des traits de soulignement. Le nom doit commencer par une lettre ou un trait de soulignement, être unique et ne pas dépasser 64 caractères.
- **Noms réservés :** certains noms de sortie sont réservés à une utilisation par le système. Si un nom est rejeté, choisissez un autre nom, tel que `qualificationReason` au lieu de `reason`.

### Eléments requis et champs pris en charge {#required-elements-and-supported-fields}

- Mappez chaque champ de saisie à un champ de prospect Marketo Engage avant d’enregistrer.
- Configurez au moins un champ de sortie. Mappez chaque sortie à un champ de prospect modifiable ; les champs en lecture seule ne sont pas disponibles dans le sélecteur de champs.
- Les champs de membre de programme ne sont pas pris en charge. Le sélecteur de champs affiche uniquement les champs de prospect.
- Les types de sortie pris en charge sont **Texte**, **Nombre** et **Vrai/Faux**.
- Pour renvoyer une liste, utilisez une valeur de texte séparée par des virgules et décrivez le format attendu dans les instructions de champ.
- Chaque exécution réussie renvoie exactement les champs de sortie configurés.

### Limites {#limits}

| Paramètre | Limite |
| --- | --- |
| Nom de l’agent ou de l’agente | 1 à 100 caractères ; unique dans l’abonnement |
| Instructions de l’agent | 1-4 000 caractères |
| Champs de saisie | Jusqu’à 20 ; chacun doit être mappé à un champ de prospect |
| Champs de sortie | 1 à 20 ; chacun doit être mappé à un champ de prospect modifiable |
| Nom du champ de sortie | 64 caractères maximum ; lettres, chiffres et traits de soulignement ; commence par une lettre ou un trait de soulignement ; unique |
| Instructions relatives au champ de sortie | Jusqu’à 512 caractères |
| Leads par demande | Jusqu’à 1 000 prospects provenant de Marketo Engage, traités en parallèle |

## Filtrage du contenu et gestion des données {#content-screening-and-data-handling}

Lorsque vous créez un agent ou modifiez ses instructions, Marketo Engage filtre les instructions de l’agent et les instructions des champs de sortie pour détecter les violations de politique, les injections d’invite et les tentatives d’exfiltration de données. Par exemple, des requêtes pour afficher des informations d’identification ou remplacer le comportement de l’agent. Si le contenu est marqué, l’enregistrement est bloqué et un message tel que « L’invite contient du contenu restreint » ou « L’invite a échoué dans la modération du contenu » peut apparaître. Révisez le texte et enregistrez-le à nouveau.

- **Accès :** la gestion des agents nécessite l’autorisation **Accès administrateur**. Les agents et l’historique des appels sont isolés par abonnement.
- **Protection des données de lead :** les données de lead sont transmises séparément des instructions de l’agent, avec des mesures de protection qui traitent les valeurs de lead comme des données plutôt que des commandes.
- **Politique de contenu :** si les données d’un prospect enfreignent la politique de contenu du fournisseur d’IA, ce prospect reçoit une activité d’erreur au lieu d’un résultat.
- **Rétention :** les payloads de la requête et de la réponse, y compris les valeurs des champs de prospect envoyées à l’agent, sont conservées pendant 30 jours dans l’historique des appels afin de prendre en charge la résolution des problèmes, puis supprimées automatiquement.

## Exécution des agents appelables dans une campagne {#how-callable-agents-run-in-a-campaign}

1. Lorsque la campagne s’exécute, Marketo Engage envoie à l’agent les valeurs des champs de prospect mappés pour chaque prospect éligible.
1. L’agent traite chaque prospect indépendamment et renvoie les champs de sortie configurés.
1. Marketo Engage écrit les résultats dans les champs de prospect mappés. Les champs modifiés apparaissent également comme des activités de modification de valeur de données standard.
1. La campagne passe à l’étape suivante.

Le traitement est asynchrone. L’étape de flux attend un résultat jusqu’à la fenêtre d’attente de l’étape de flux dans Marketo Engage. Si un prospect échoue (en raison d’une temporisation, par exemple), il est affecté d’une activité d’erreur et les autres prospects continuent. Chaque résultat apparaît dans le journal d’activité du prospect pour l’agent appelant.

Utilisez les champs de sortie dans la logique de campagne. Par exemple, branchez sur **N’est pas** pour acheminer différemment les envois de spam, ou branchez-vous sur **Confiance** pour envoyer les résultats à faible degré de confiance à une étape de révision.

## Assurance qualité de la pré-activation {#pre-activation-qa}

Avant d’activer une campagne pour tous les prospects :

- Exécutez la campagne avec un petit jeu de tests de prospects.
- Vérifiez le journal d’activité de chaque prospect et confirmez que les champs de sortie ont été correctement mis à jour.
- Testez les cas de périphérie, y compris les valeurs manquantes et les entrées inhabituelles.
- Vérifiez que les branches de campagne gèrent des valeurs telles qu’un niveau de confiance faible ou une classification de robot/spam comme prévu.

## Cas d’utilisation {#use-cases}

- **Nettoyage des données :** normaliser les noms de société, mettre en forme les numéros de téléphone en E.164 et normaliser les intitulés de poste lorsque des prospects sont créés ou importés.
- **Filtrage des robots et des spams :** vérifiez les envois pour trouver les noms charabia, les e-mails suspects et les numéros de téléphone à chiffres répétés ; dirigez la campagne en fonction des résultats.
- **Détection des e-mails jetables :** identifiez les adresses e-mail temporaires et acheminez-les différemment des adresses e-mail professionnelles.
- **Classification de lead :** segmente les leads en fonction de la taille de la société, du secteur, du profil et de l’intention de prendre en charge le routage ou la notation.
- **Enrichissement du prospect :** déduisez les détails manquants tels que le service, l’ancienneté ou le statut de décideur d’un prospect.
- **Règles personnalisées :** créez une vérification ou une catégorisation par oui/non qui peut être décrite comme une règle de traitement des prospects, telle que le marquage des prospects d’une région ou d’un secteur.

## Dépannage {#troubleshooting}

| Problème | Résolution |
| --- | --- |
| **Agents** n’apparaît pas dans la navigation. | Demandez à votre administrateur Marketo Engage d’accorder l’autorisation **Accès administrateur**. |
| L’enregistrement est bloqué avec un message de contenu. | Révisez les instructions de l’agent ou les instructions du champ pour supprimer le contenu marqué, puis enregistrez à nouveau. |
| Le statut de l’agent est **Échec de la publication**. | Modifiez l’agent, corrigez le champ nommé dans le message, puis sélectionnez **Enregistrer et publier**. |
| Vous ne pouvez pas modifier un agent publié. | Les agents publiés sont figés. Créez un agent pour apporter des modifications. |
| Vous ne pouvez pas supprimer un agent. | Supprimez son étape de flux de chaque campagne intelligente répertoriée comme utilisant l’agent, puis supprimez-la. |
| Un nom de champ est signalé comme réservé. | Choisissez un autre nom de champ de sortie, tel que `qualificationReason`, puis enregistrez à nouveau. |
| Certains prospects reçoivent une activité d’erreur. | Vérifiez le journal d’activité du prospect. Les échecs individuels, y compris les dépassements de délai ou les violations de politique de contenu, n’affectent pas les autres prospects. |
| Les résultats sont inattendus. | Renseignez les instructions plus spécifiques, ajoutez des exemples, affinez les instructions de champ et testez à nouveau avec un petit ensemble de prospects. |

## Étapes suivantes {#next-steps}

- Vérifiez la liste **Utilisé par** de l’agent et confirmez quelles campagnes intelligentes l’utiliseront.
- Testez l’étape de flux avec un petit groupe de prospects et validez les journaux d’activité et les champs de sortie.
- Utilisez les champs de sortie pour ajouter des branches de campagne pour les classifications ou les résultats de faible confiance.
- Supprimez l’étape de flux de l’agent de toutes les campagnes avant de supprimer l’agent.
