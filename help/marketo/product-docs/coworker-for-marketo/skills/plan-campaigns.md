---
description: Utilisez CX Enterprise Coworker for Marketo Engage pour transformer un résumé de campagne en un plan de programme structuré couvrant la logique de l’audience, les e-mails, les jetons et les contrôles QA.
title: Planification de campagnes
source-git-commit: b47454801d391f4d7a75ebcfce7ac76c2f4b8af4
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 1%
---
# Planification de campagnes {#plan-campaigns}

Transformez un brief de campagne en un plan d’implémentation structuré pour Marketo Engage. La compétence Planifier des campagnes décrit la structure du programme, la logique d’audience, les e-mails, les campagnes intelligentes, les jetons, le compte rendu des performances et les contrôles de préactivation. La sortie est un rapport téléchargeable qui s’affiche dans le panneau de l’espace de travail.

>[!NOTE]
>
>Cette compétence génère des plans d’implémentation pour les programmes Marketo Engage (documents structurés qui indiquent à un humain ou à un système d’automatisation comment créer une campagne). Il ne crée rien dans Marketo Engage. Il y a une compétence distincte pour [programmes de renforcement](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md).

## Conditions préalables {#prerequisites}

- Pour un plan de programme, fournissez un résumé de campagne avec les informations disponibles, telles que les objectifs de la campagne, l’audience cible, les messages, la chronologie et les mesures de succès.
- Pour améliorer un brief ou un plan existant, fournissez le document et décrivez les modifications que vous souhaitez.
- Pour commencer sans brief, demandez un brief type ou demandez un plan basé sur un scénario de campagne courant.

## Utilisation {#how-to-use}

1. Dans Mon Marketo, cliquez sur la mosaïque **[!UICONTROL CX Enterprise Coworker pour Marketo Engage]**.

1. Sélectionnez la compétence **[!UICONTROL Planifier des campagnes]** et cliquez sur **[!UICONTROL Utiliser cette compétence]**.

1. Choisissez ce que vous souhaitez faire :
   - Planifiez un programme à partir d’un résumé de campagne.
   - Générez un exemple de résumé de campagne.
   - Polonais un brief existant.
   - Révisez un plan de configuration existant.

1. Fournissez le mémoire ou le document. Incluez les modifications spécifiques, les exigences de la campagne ou les conventions organisationnelles.

1. Examinez le rapport généré dans le panneau de l’espace de travail. Ouvrez-le pour consulter les détails ou télécharger le rapport.

1. Examinez et approuvez le plan de configuration avant de créer le programme dans Marketo Engage.

## Options de compétence {#skill-options}

### Planification d’un programme {#plan-a-program}

Un plan de programme traduit les exigences de la campagne en instructions pour créer le programme. En fonction du brief, il peut inclure :

- **Présentation du programme :** nom de la campagne, objectifs, audience cible et calendrier.
- **Structure des dossiers :** dossiers locaux recommandés pour les e-mails, les campagnes intelligentes et les rapports.
- **Listes dynamiques :** logique de segmentation, définitions de filtre et exclusions requises.
- **Configuration du canal e-mail :** objets, texte d’en-tête, structure de contenu, détails de l’expéditeur et éléments de conformité.
- **Campagnes intelligentes :** noms de campagne, désignation de déclencheur ou de lot, étapes de flux et recommandations de planification.
- **Jetons et champs :** Mes jetons, jetons obligatoires et personnalisés, et tous les champs personnalisés nécessaires avec leurs types et valeurs.
- **Flux de Parcours :** séquence de campagne, étapes d’attente et logique de décision.
- **Rapports et contrôle qualité :** mesures de succès, rapports recommandés et contrôles de validation avant activation.

### Créer un exemple de brief {#create-a-sample-brief}

Demandez un exemple de brief lorsque vous souhaitez qu’un exemple s’adapte. Vous pouvez spécifier un sujet ou un type de campagne, tel qu’un lancement de produit ou un webinaire. Si vous demandez un plan sans fournir de résumé, la compétence peut utiliser un exemple de scénario, tel qu’un webinaire de lancement de produit, comme base du plan.

### Polonais un brief ou réviser un plan {#polish-a-brief-or-revise-a-plan}

La compétence identifie le type de document à partir de son contenu, plutôt que de se fier uniquement au libellé de votre requête.

Un **résumé de campagne** décrit généralement les objectifs, l’audience, la stratégie de messagerie, la chronologie et les mesures de succès. Un **plan de configuration** contient généralement des détails d’implémentation tels que les configurations de liste dynamique, les étapes de flux de campagne dynamique, les définitions de jeton, les spécifications d’e-mail et les exigences techniques.

Fournissez le document et les modifications demandées. Par exemple, si vous demandez à peaufiner un plan mais fournissez un résumé de campagne, la compétence traite le document comme un résumé. Si vous fournissez un plan de configuration et demandez à réviser un brief, il traite le document comme un plan.

## Intégration des règles d’organisation {#organizational-rules-integration}

Les documents de configuration doivent incorporer les règles de votre organisation à partir du contexte système.

### Conventions de dénomination {#naming-conventions}

- Programmes : `{{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}`
- E-mails : `{{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}`
- Campagnes intelligentes : `{{NUMBER}}_{{TRIGGER_OR_BATCH}}_{{ACTION}}`

### Éléments requis {#required-elements}

- Trois dossiers locaux (01 E-mails, 02 Campagnes intelligentes, 03 Rapports)
- Quatre jetons requis (eventDate, eventTime, responseToEmail, senderName)
- Filtres d’exclusion (désabonnement, e-mail non valide, marketing suspendu, supprimé)
- Conformité des e-mails (lien de désabonnement, adresse physique)

### Assurance qualité de la pré-activation {#pre-activation-qa}

- Validation du modèle de nom
- Confirmation de la structure du dossier
- Vérification du filtre d’exclusion
- Vérifications des éléments de conformité

## Cas d’utilisation {#use-cases}

**Planifier un programme de webinaire :** indiquez l’objectif du webinaire, l’audience, la chronologie de l’événement et les besoins en matière de messagerie. Le plan de configuration peut décrire la structure du programme, les spécifications des e-mails, la séquence de la campagne, les jetons et les contrôles QA.

**Générer un modèle de brief :** demandez un modèle de brief pour un type de campagne, puis adaptez-le avec les détails de votre campagne avant de demander un plan de programme.

**Mettre à jour un plan de configuration existant :** fournissez le plan et indiquez les modifications, telles que la mise à jour de la chronologie, l’ajout d’une étape de campagne ou la révision de la logique d’audience.

## Étapes suivantes {#next-steps}

Une fois l&#39;opération de planification terminée, les invites de suivi appropriées peuvent inclure :

- « Réviser ce plan de configuration »
- « Obtenir un exemple de résumé de campagne »
- « Créer ce programme dans Marketo » (pour créer un programme, vous devez utiliser les compétences [créer des programmes](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md)).
