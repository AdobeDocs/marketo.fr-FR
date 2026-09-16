---
description: Découvrez comment les règles d’organisation définissent les normes de gouvernance et guident Coworker for Marketo Engage dans la création, la planification et la validation de programmes.
title: Règles d'organisation
source-git-commit: c1581e2b692dd50bf472756e4e6222ff75ae091c
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%
---
# Règles d&#39;organisation {#organizational-rules}

Les règles d’organisation définissent vos normes d’opérations marketing et exigences de gouvernance dans un document unique qui guide Coworker for Marketo Engage dans les workflows de création de programme, de planification de campagne et de validation.

## Que sont les règles d&#39;organisation ? {#what-are-organizational-rules}

Les règles d’organisation sont un document de configuration basé sur Markdown qui capture les normes de campagne de votre organisation :

* Conventions de dénomination pour les programmes, les e-mails et les campagnes intelligentes
* Ressources et structure requises (dossiers, jetons, rapports)
* Exigences de conformité (liens de désabonnement, paramètres UTM, filtres d’exclusion)
* Bonnes pratiques (conception d’e-mail, configuration de liste dynamique)

Chaque environnement Marketo Engage comprend des règles d’organisation par défaut. Vous pouvez les personnaliser en fonction des besoins de gouvernance spécifiques de votre entreprise.

## Où les règles d’organisation sont utilisées {#where-organizational-rules-are-used}

Les règles d’organisation guident Coworker for Marketo Engage selon trois compétences :

| Compétence | Application des règles |
| --- | --- |
| Créer des programmes | Les règles guident la création de la structure, du nom et de la configuration initiale du programme. Un collègue de Marketo Engage signale tout problème de conformité dans votre mémoire avant de créer le programme. |
| Planifier des campagnes | Les règles indiquent comment Coworker pour Marketo Engage structure les campagnes intelligentes, les filtres et les étapes de flux en fonction de vos normes. |
| Valider les programmes | Les règles définissent ce que Coworker for Marketo Engage vérifie lors de la validation des programmes avant activation. |

## Accès et personnalisation des règles d’organisation {#how-to-access-and-customize-organizational-rules}

1. Dans Mon Marketo, cliquez sur la mosaïque **Collègue pour Marketo Engage**.
1. Cliquez sur l’icône d’engrenage.
1. Sélectionnez l’onglet **Règles d’organisation**.
1. Examinez les règles par défaut (elles sont préremplies avec les bonnes pratiques relatives aux opérations marketing).
1. Modifiez les règles pour qu’elles correspondent à celles de votre organisation :

   * Conventions de dénomination (programmes, e-mails, campagnes)
   * Structure de dossiers requise
   * Jetons et champs obligatoires
   * Normes de conformité et d&#39;exclusion

1. Mettez à jour le numéro de version lorsque vous apportez des modifications.
1. Enregistrez vos modifications. Toutes les compétences Coworker for Marketo Engage utiliseront immédiatement vos règles personnalisées.

## Structure des règles d&#39;organisation {#organizational-rules-structure}

Les règles d’organisation sont formatées en Markdown avec la matière de front YAML :

```markdown
---
name: Your Organization Name - Marketo Campaign Governance
version: 1.0
enabled: true
customized: true
---

# Naming Conventions

## Programs
- Pattern: {{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}
- Example: AMER_FY25_Q2_WBR_250315_Product_Launch_Webinar
- Region codes: AMER, EMEA, APAC, GLOBAL

## Emails
- Pattern: {{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}
- Example: Product_Launch_01_Invitation

# Program Structure

## Required Local Folders
- 01 Emails
- 02 Smart Campaigns
- 03 Reports

## Required Tokens
- {{my.eventDate}}
- {{my.replyToEmail}}

# Email Compliance

## Required Elements
- Unsubscribe link in footer
- Company name and physical address
- All external links include UTM parameters

## Recommended Elements
- Alt text on all images
- Mobile-responsive design (600px max-width)
```

## Bonnes pratiques relatives aux règles d’organisation {#best-practices-for-organizational-rules}

* **Commencer par les valeurs par défaut** : consultez les règles par défaut avant de les personnaliser. Ils reflètent les bonnes pratiques du secteur pour les opérations marketing.
* **Rester concentré sur les règles** : incluez uniquement les exigences importantes pour votre organisation. Les règles inutiles créent du bruit et réduisent inutilement les scores de conformité.
* **Utiliser à la fois des vérifications automatisées et manuelles** :

  * Vérifications automatisées : conventions de nommage, dossiers requis, utilisation des jetons (Coworker for Marketo Engage peut vérifier ces éléments)
  * Vérifications manuelles : conception visuelle des e-mails, conformité de la marque, logique de la campagne (un collègue de Marketo Engage les signalera comme étant des étapes de révision manuelle)

* **Équilibrer rigueur et flexibilité** : des règles trop strictes peuvent ralentir la création d’un programme. Les règles trop souples ne détecteront pas les problèmes de conformité importants.
* **Version de vos règles** : mettez à jour le numéro de version lorsque vous effectuez des modifications importantes afin que votre équipe sache que les normes de gouvernance ont été mises à jour.
* **Communiquer les modifications** : lorsque vous mettez à jour les règles d’organisation, informez votre équipe des opérations marketing de ce qui a changé et pourquoi.

## Ce que Coworker for Marketo Engage peut ou ne peut pas valider {#what-coworker-can-and-cannot-validate}

Coworker for Marketo Engage PEUT valider (contrôles automatisés) :

* Les conventions de nommage correspondent à vos modèles
* La structure de dossiers requise existe.
* Les jetons requis sont en place.
* L’e-mail comporte un lien de désabonnement et les éléments de pied de page requis.
* Les liens externes incluent les paramètres UTM.
* Les noms de campagnes intelligentes respectent les conventions

Collègue pour Marketo Engage NE PEUT PAS valider (révision manuelle requise) :

* Logique de filtre de liste dynamique (limitation de l’API : vous devez configurer les filtres manuellement)
* Logique d’étape de flux de campagne intelligente (limitation de l’API : vous devez configurer les flux manuellement)
* Rendu visuel et réactivité des emails (nécessite une inspection visuelle)
* Conformité de la marque et ton des messages (nécessite un jugement humain)
* Règles de segmentation de contenu dynamique (limitation d’API)

Lorsque Coworker for Marketo Engage rencontre un élément qu’il ne peut pas valider, il le signale comme une étape de révision manuelle dans le workflow.

## Score de conformité {#compliance-scoring}

Lorsque vous utilisez Valider les programmes, Coworker for Marketo Engage calcule un score de conformité en fonction des éléments suivants :

* **Vérifications réussies** : la conformité a été vérifiée par un collègue de Marketo Engage et aucun problème n’a été détecté
* **Échec des vérifications** : un collègue de Marketo Engage a détecté des violations de vos règles d’organisation
* **Étapes de vérification manuelle** : éléments nécessitant une vérification humaine (ils ne sont PAS comptabilisés dans votre score)

Un programme peut être conforme à 100 % et nécessiter toujours des étapes de révision manuelles ; elles sont exclues du calcul de la note.

## Exemples de personnalisation des règles d’organisation {#examples-of-organizational-rules-customization}

**Exemple 1 : convention de nommage stricte**

```markdown
## Programs
Pattern: {{COUNTRY}}-{{BUSINESS_UNIT}}-{{CAMPAIGN_TYPE}}-FY{{YEAR}}-{{QUARTER}}-{{DATE}}
```

Utilisez cette option si votre organisation nécessite une gouvernance stricte entre les régions et les unités commerciales.

**Exemple 2 : dénomination flexible avec préfixe requis**

```markdown
## Programs
Pattern: {{PREFIX}}_* (where PREFIX = EMEA, AMER, APAC, GLOBAL)
Example: AMER_Q2_Product_Launch_Webinar_2025
```

Utilisez cette option si vous souhaitez une cohérence sur les codes région, mais une flexibilité sur le reste.

**Exemple 3 : règles minimales (accent mis sur la conformité)**

```markdown
# Email Compliance - REQUIRED

- Unsubscribe link present
- CAN-SPAM physical address in footer
- Reply-to email configured
```

Utilisez cette option si votre entreprise donne la priorité à la conformité plutôt qu’à la cohérence des noms/structures.

## Dépannage {#troubleshooting}

**Q : J’ai mis à jour les règles d’organisation, mais Coworker pour Marketo Engage utilise toujours les anciennes règles.**

R : Les modifications prennent effet immédiatement pour les nouveaux programmes et validations. Si vous travaillez sur un programme existant, actualisez votre navigateur ou démarrez un workflow Coworker for Marketo Engage pour afficher les règles mises à jour.

**Q : Puis-je revenir aux règles par défaut ?**

R : Oui. Accédez à **Paramètres** > **Règles d’organisation** et cliquez sur **Réinitialiser aux valeurs par défaut**. Vos règles personnalisées seront remplacées par les règles par défaut.

**Q : Mon score de conformité est faible, même si le programme semble correct.**

A : vérifiez les vérifications qui échouent. Passez en revue vos règles d’organisation pour voir si elles sont trop strictes pour vos workflows actuels ou si vous devez ajuster le programme pour qu’il réponde à vos normes.
