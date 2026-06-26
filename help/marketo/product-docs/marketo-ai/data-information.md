---
description: Explorez la suite d’agents Marketo AI conçue pour automatiser les tâches marketing telles que l’assurance qualité des programmes, l’importation de prospects, la normalisation des données, etc.
title: Fiche d’information sur les données de l’IA dédiée à Marketo
badge: Beta
hide: true
source-git-commit: 39fef7edc7c475efd901a75235ccf7b25f789793
workflow-type: tm+mt
source-wordcount: '1478'
ht-degree: 0%

---

# Fiche d’information sur les données de l’IA dédiée à Marketo {#data-information}

L’IA dédiée à Marketo est une fonctionnalité native d’agent de Adobe Marketo Engage qui permet aux équipes opérationnelles marketing d’automatiser certains workflows par le biais d’interactions en langage naturel, notamment l’importation de pistes, la validation de programme, la normalisation des données, la création de programmes, l’enquête de pistes, l’analyse et les conseils sur les produits. L’IA dédiée à Marketo fonctionne dans l’environnement Marketo Engage existant d’un utilisateur et utilise une infrastructure gérée par Adobe pour le raisonnement et l’orchestration de l’IA.

**Environnement utilisateur :** l’IA dédiée aux Marketo fonctionne dans un environnement Marketo Engage existant et n’introduit pas de nouveau chemin de partage d’utilisateur à utilisateur.

**Portée des données :** le service traite les données marketing B2B standard déjà présentes dans l’environnement de l’utilisateur, y compris les enregistrements de prospect, les données de programme et l’activité de campagne intelligente.

**Services d’IA :** l’IA dédiée au Marketo exploite un faisceau d’IA créé par Adobe et utilise Azure OpenAI GPT-4.1 et Claude sur AWS Bedrock pour le raisonnement de l’IA, avec des outils de MCP Marketo prenant en charge l’exécution d’actions de produit.

**Gouvernance :** les sorties générées par l’IA restent dans l’environnement de l’utilisateur et sont soumises aux contrôles existants en matière de gouvernance, de résidence et de rétention.

**Transparence :** sorties générées par l’IA peuvent être examinées par le biais de l’historique des conversations et des audits afin de prendre en charge la supervision des utilisateurs.

## Contrôles d’accès et déploiement

### Importer les leads

**Fonction :** traite les données de prospect fournies par l’utilisateur pour le mappage, la normalisation, la déduplication et l’importation dans Marketo Engage.

### AQ du programme

**Fonction :** évalue les programmes Marketo par rapport aux règles d’organisation définies par les utilisateurs dans un fichier Markdown de compétences, telles que les normes de nommage, le statut d’approbation, la conformité des e-mails et la logique de flux.

### Créer un programme à partir d’un brief

**Fonction :** utilise des invites en langage naturel pour générer des structures de programme Marketo, notamment des campagnes intelligentes, des étapes de flux et des espaces réservés de contenu, directement dans l&#39;environnement de l&#39;utilisateur.

### Agents appelables

**Fonction :** exécute des actions d’IA déclenchées par une action de flux dans des étapes de flux Smart Campaign pour des cas d’utilisation tels que la validation, la normalisation et la détection de robots.

### Enquête principale

**Fonction :** fournit une analyse conversationnelle des raisons pour lesquelles une personne a atteint ou non un jalon en examinant l’exécution de l’étape de flux et l’appartenance à une liste dynamique.

### Mesures et analyses

**Fonction :** analyse les performances des campagnes et des programmes, y compris les recommandations et les informations sur les causes profondes.

### Connaissances du produit

**Fonction :** fournit des conseils pratiques et pratiques relatifs à Marketo au moyen d’une couche de connaissances partagées utilisée dans l’expérience de l’agent.

## Cas d’utilisation

Outre les problèmes répertoriés, envisagez d’utiliser l’IA dédiée à Marketo pour diagnostiquer et résoudre des problèmes opérationnels complexes (échecs de synchronisation CRM, erreurs webhook, analyse des causes premières des diffusions e-mail, incohérences entre les champs), effectuer des audits sur votre compte (délivrabilité des e-mails, conformité du centre d’abonnement, révisions des campagnes intelligentes, évaluations des modèles de score) et accélérer la création de programmes à partir de résumés et de modèles (programmes d’événement, campagnes par e-mail multilingues, configurations de webinaires). Additional est conçu pour vous aider dans la classification de leads et l’enrichissement des données à grande échelle assistés par l’IA, dans l’analyse de performances avec des recommandations de mesures correctives et dans le débogage guidé de configurations techniques telles que les scripts Velocity et les modèles de cycle de vie.

## Disponibilité et statut du déploiement

**Éligibilité :** l’activation initiale des utilisateurs se limite aux utilisateurs de Marketo Engage éligibles qui ont accepté le programme Adobe Gen AI Rider.

**Mise en service :** l’accès est géré par le biais de contrôles d’activation de produit existants et de la mise en service des indicateurs de fonctionnalité dans l’expérience Marketo Engage.

**Modèle de déploiement :** le déploiement progresse dans Alpha et Private Beta avant l’extension plus large de Public Beta.

**Portée géographique :** la version initiale est destinée aux utilisateurs globaux de Marketo Engage, à l’exclusion de la Chine continentale.

**Étendue du secteur :** le déploiement actuel n’inclut pas de fonctionnalités verticales spécifiques pour les secteurs fortement réglementés tels que la santé, les services financiers, le gouvernement ou la défense.

## Documentation et assistance

**Documentation :** la documentation d’Experience League se développe dans le cadre de la préparation générale à la disponibilité.

**Modèle d’assistance :** l’approche d’assistance actuelle comprend la réception des commentaires des utilisateurs, les heures de bureau et une communauté Marketo AI Experience League.

**Suivi des services :** Adobe identifie l’observabilité, les tableaux de bord de commentaires et les mécanismes d’évaluation de la qualité comme des composants importants de la maturité du lancement et de l’amélioration continue.

## Données et exclusions hors de la portée

**Aucune nouvelle donnée de catégorie spéciale :** l’IA dédiée aux Marketo n’introduit pas de nouveau traitement pour les données relatives à la santé, aux finances, à la localisation précise, à la biométrie ou à d’autres données de catégorie spéciale.

**Aucun nouveau chemin de partage :** le service ne crée pas de mécanisme de partage de contenu d’utilisateur à utilisateur.

**Sorties contenues par l’utilisateur ou l’utilisatrice :** les sorties générées par l’IA restent dans l’environnement Marketo Engage de l’utilisateur ou de l’utilisatrice sous les contrôles de gouvernance existants.

**Exclusions actuelles :** le déploiement initial exclut la Chine continentale et ne fournit pas de fonctionnalités spécifiques verticales pour les secteurs fortement réglementés.

## Utilisation d’Azure OpenAI et de Claude sur AWS Bedrock

Cette section explique comment Azure OpenAI prend en charge les workflows d’IA Marketo. Tous les diagrammes ou descriptions de flux associés doivent être lus avec les contrôles décrits ici, y compris les limitations sur la portée des données, la supervision de l&#39;utilisateur et la formation des modèles.

**Objectif :** Azure OpenAI GPT-4.1 est utilisé pour le raisonnement conversationnel et l’orchestration des workflows pilotés par des agents.

**Portée des données :** les entrées sont limitées aux données marketing B2B standard déjà présentes dans l’environnement Marketo Engage de l’utilisateur et nécessaires pour exécuter le workflow demandé.

**Sortie IA : les sorties IA** sont déterminées par les invites et la configuration de l&#39;utilisateur, et les fonctionnalités IA de Marketo ne prennent aucune décision de manière autonome sans configuration de l&#39;utilisateur.

**Formation :** Adobe n’utilise pas les données utilisateur pour entraîner ou affiner les modèles Azure OpenAI pour ce service.

**Supervision de l’utilisateur :** les sorties générées par l’IA restent examinables dans Marketo Engage par le biais de fonctionnalités d’historique de conversation et d’audit.

## Conservation et stockage des données

**Sorties contenues par l’utilisateur/utilisatrice :** les sorties générées par l’IA telles que les listes de prospects nettoyées, les rapports d’assurance qualité, les structures de programme générées et les données normalisées restent dans l’environnement Marketo Engage de l’utilisateur/utilisatrice.

**Alignement de la gouvernance :** les données de sortie restent soumises aux contrôles existants de l’utilisateur en matière de gouvernance des données, de résidence et de conservation dans Marketo Engage.

**Pas de nouvelle boutique inter-utilisateurs :** le service n’introduit pas de chemin de partage de données d’utilisateur à utilisateur distinct.

## Emplacements de traitement et de stockage des données

Cette section résume les environnements dans lesquels l’IA dédiée au Marketo fonctionne et où le traitement se produit. Si le document comprend des diagrammes régionaux ou des visuels d&#39;infrastructure, ces documents doivent être compris comme des représentations de haut niveau de l&#39;emplacement du service et du flux de traitement plutôt que comme des schémas de réseau exhaustifs.

**Environnement d’application :** l’IA dédiée au Marketo fonctionne dans l’environnement Adobe Marketo Engage existant de l’utilisateur.

**Traitement IA :** l’IA Marketo utilise Azure OpenAI GPT-4.1 et Claude sur AWS Bedrock pour le raisonnement conversationnel et l’orchestration des tâches.

**Emplacement des données utilisateur :** les données utilisateur et les sorties générées par l’IA restent dans l’environnement Marketo Engage de l’utilisateur et sont soumises aux contrôles existants de résidence, de gouvernance et de conservation de l’utilisateur.

**Pas de banque de données inter-utilisateurs distincte :** le service n’introduit pas de couche de partage ou de stockage de données d’utilisateur à utilisateur distincte.

## Considérations relatives aux informations d’identification personnelles et à la confidentialité des données

### Étendue des données par type de workflow

Les données traitées par l’IA dédiée au Marketo sont déterminées par le modèle d’utilisation de l’utilisateur et le workflow spécifique appelé. Tous les workflows ne nécessitent pas de traiter des données au niveau du prospect.

### Workflows qui traitent uniquement les métadonnées de campagne (aucune PII de prospect)

* Création de programme à partir d’un résumé — génère des structures de programme, des campagnes intelligentes, des étapes de flux et des espaces réservés de contenu à partir d’instructions en langage naturel
* Clonage et traduction d&#39;emails : duplique et traduit le contenu, les objets et la copie marketing d&#39;email HTML dans différentes variantes linguistiques
* Contrôle des campagnes : examine les configurations de campagnes intelligentes, les définitions de déclencheur/filtre, la logique de flux et les conventions de nommage.
* Validation du contrôle qualité du programme : évalue les programmes par rapport aux règles définies par l’utilisateur en termes de conformité, de statut d’approbation et d’exhaustivité structurelle
* Révisions du centre d&#39;abonnement et de l&#39;architecture du programme — analyse la logique de la campagne et la structure du programme
* Connaissances sur les produits et conseils sur les bonnes pratiques : fournit des réponses pratiques Marketo à partir d’une couche de connaissances partagées.

### Workflows qui traitent les enregistrements au niveau du lead (champs de contact B2B standard)

* Recherche et dépannage de lead — Examine les valeurs de champ de lead individuel, l’historique d’activité et la progression du cycle de vie afin de déterminer pourquoi un lead a atteint ou non les normes MQL ou s’est qualifié pour une campagne marketing
* Import et normalisation des leads : traite les données de leads fournies par l’utilisateur, y compris les noms, adresses e-mails, numéros de téléphone et champs d’entreprise, à des fins de mappage, de nettoyage et de déduplication
* Classification et enrichissement des leads : évalue les enregistrements de leads par rapport à la notation ou à la logique de classification définies par l’utilisateur (par exemple, leads valides ou spams pour l’intégrité de la base de données, personas à des fins de personnalisation, leads d’entreprise avec leads d’entreprise par e-mail par rapport aux leads consommateurs).
* Audits de la qualité et de la délivrabilité des données : analyse les données d’engagement au niveau du prospect, les modèles de rebond et les enregistrements en double pour identifier les problèmes d’intégrité de la base de données
* Analyses des performances de Campaign : fait apparaître les modèles d’engagement des prospects, les données de conversion et la composition de l’audience pour prendre en charge l’analyse des performances

### Minimisation des données par conception

* Dans tous les cas, les données envoyées au modèle d’IA sont limitées à ce qui est nécessaire pour répondre à la demande spécifique de l’utilisateur dans ce workflow
* L’IA hérite des autorisations Marketo Engage existantes de l’utilisateur demandeur. Elle ne peut pas accéder aux enregistrements, champs ou programmes du lead au-delà de ce que l’utilisateur peut déjà voir dans l’interface utilisateur du produit
* Les workflows d’enquête et d’opérations de données nécessitent nécessairement des données au niveau du prospect, car l’utilisateur demande explicitement à l’IA d’analyser, de classer ou d’agir sur ces enregistrements
* Les utilisateurs qui souhaitent limiter le traitement des données de prospect peuvent restreindre l’accès aux outils et aux workflows d’investigation par le biais des contrôles de rôle et d’autorisation Marketo Engage existants tout en conservant un accès complet aux fonctionnalités d’IA structurelle et administrative

### Aucune exposition incrémentielle des données

L’IA fonctionne comme un accélérateur des autorisations utilisateur existantes, et non comme un chemin d’escalade. Un utilisateur qui ne peut pas afficher certains champs de prospect, programmes ou partitions dans l’interface utilisateur de Marketo Engage ne peut pas non plus faire apparaître ces données via l’IA dédiée à Marketo. Le service ne contourne pas les règles de partition, les autorisations au niveau du champ ou les restrictions de l’espace de travail.
