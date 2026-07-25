---
description: Découvrez comment les politiques de conservation des données sur 25 mois et 90 jours de Marketo affectent les rapports Analytics, avec une répartition par rapport et des conseils pour conserver les données plus longtemps.
title: Conservation des données
feature: Reporting
source-git-commit: 0828b4cb43dd18d02b80083ea5128e2f0e5e40d6
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 5%

---

# Politique de conservation des données d’activité de Marketo - Impact sur les rapports

Marketo conserve les données d’activité marketing de manière progressive. Les données sur les activités et les adhésions aux campagnes sont stockées pendant 25 mois consécutifs après la date d’activité. Par défaut, les données d’activité volumineuses sont conservées pendant 90 jours consécutifs après la date d’activité, après quoi elles peuvent être ajustées par utilisateur. Au-delà de ces périodes de conservation, les données ne sont plus disponibles via l’interface utilisateur de Marketo.

## Rapports Marketo analytics

Les données d’activité étant conservées jusqu’à 25 mois, certains rapports Marketo Analytics sont affectés par cette politique, tandis que d’autres ne le sont pas. Les rapports qui extraient des données des journaux d’activité des personnes n’affichent des données que pour une durée maximale de 25 mois. Les rapports qui ne font aucune référence à l’activité des personnes ne sont pas affectés.

Cependant, même les rapports qui ne font pas référence à l’activité des personnes par défaut peuvent être affectés si des filtres sont ajoutés à la liste dynamique du rapport. Les filtres qui référencent des attributs de personne (informations dans les champs de l’enregistrement de personne) n’entraînent aucune modification du rapport. Les filtres qui recherchent les activités que la personne a prises ne peuvent accéder aux activités qu’à l’intérieur de la fenêtre de conservation. Par conséquent, si l’activité s’est produite il y a plus longtemps que cela, les résultats du rapport seront modifiés.

Le tableau ci-dessous résume le comportement de chaque rapport, y compris les scénarios de filtre courants.

## Référence du rapport

| Type de rapport | Filtrer le scénario | Affecté par la politique de rétention ? |
|---|---|---|
| **Rapports de l’explorateur du cycle de revenus** | Aucun filtre disponible | Non — Les utilisateurs de Revenue Cycle Explorer et d’Advanced Analytics sont entièrement exemptés de ces limites de conservation. Les données RCE sont envoyées pendant la nuit dans un serveur de base de données distinct qui gère les rapports RCE. Étant donné qu’ils sont hébergés séparément et non dans des journaux d’activité personnels, ces rapports ne sont pas affectés par cette politique. L’Explorateur du cycle de revenu n’extrait pas directement les données de la base de données des personnes. Les filtres ne sont donc pas disponibles. |
| **Rapport sur les performances des personnes** | Aucun filtre de liste dynamique | Non |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Personnes par statut** | Aucun filtre de liste dynamique | Non |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Personnes par étape de chiffre d’affaires** | Aucun filtre de liste dynamique | Non |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Analyseur de chemin de succès** | N’inclut pas les listes dynamiques | S/O |
| **Rapport d’influence sociale** | Aucun filtre de liste dynamique | Oui |
| | Filtres sur les attributs de personne (par exemple : prénom) | Oui |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Oui |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Analyseur d’influence d’opportunité** | N’inclut pas les listes dynamiques | Non |
| **Performances des e-mails** | Aucun filtre de liste dynamique | Non |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Performances du lien e-mail** | Aucun filtre de liste dynamique | Non |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Email Insights** | N’utilise pas de listes dynamiques | Non |
| **Performances des e-mails de Sales Insight** | Aucun filtre de liste dynamique | Non |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Performances de la page de destination** | Aucun filtre de liste dynamique | Non — Les données de performances des pages de destination sont conservées indéfiniment et ne sont pas soumises à la politique de conservation. |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Non |
| **Activité de page web** | Aucun filtre de liste dynamique | Oui - sous réserve de la période de conservation par défaut de 90 jours (ajustable par utilisateur) |
| | Filtres sur les attributs de personne (par exemple : prénom) | Oui |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Oui |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Activité Web de l’entreprise** | Aucun filtre de liste dynamique | Oui |
| | Filtres sur les attributs de personne (par exemple : prénom) | Oui |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Oui |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Performance du programme** | Aucun filtre de liste dynamique | Non |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Performances du flux d’engagement** | Aucun filtre de liste dynamique | Non |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Analyseur de programmes** | N’utilise pas de listes dynamiques | Non |
| **Activité de campagne** | Aucun filtre de liste dynamique | Non |
| | Filtres sur les attributs de personne (par exemple : prénom) | Non |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Non |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |
| **Performances des emails de Campaign** | Aucun filtre de liste dynamique | Oui |
| | Filtres sur les attributs de personne (par exemple : prénom) | Oui |
| | Filtres sur les activités des personnes au cours des 25 derniers mois | Oui |
| | Filtres sur les activités des personnes sans contrainte de date | Oui |

## Solutions de contournement des rapports

De nombreux utilisateurs peuvent considérer que les données d’activité antérieures à la fenêtre de conservation sont obsolètes. Cependant, il se peut que vous ayez besoin de ces informations dans un cas d’utilisation. Vous trouverez ci-dessous des moyens de conserver ces données au-delà de la période de conservation standard.

## Exporter les données

Marketo propose l’API REST [Bulk Extract](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/bulk-extract/bulk-extract), qui permet d’exporter les activités des personnes et de les héberger localement. Une fois les données extraites via l’API, vous pouvez les stocker et les trier selon vos besoins dans votre cas d’utilisation.

>[!TIP]
>
>Exportez vos données de personne régulièrement, et pas une seule fois. Les activités des personnes sont conservées selon un cycle continu de 25 mois. Définissez un rappel pour exporter à nouveau _avant_ la fin de cette période de 25 mois.

## Utiliser des champs personnalisés

Les valeurs des champs de personne ne sont pas affectées par la politique de conservation des données. Vous pouvez utiliser des campagnes intelligentes pour renseigner des champs personnalisés avec des valeurs en fonction des activités menées par vos employés. Vous pouvez ainsi filtrer les personnes en fonction de ces attributs de personne (non soumis à la politique de rétention) plutôt que par les activités elles-mêmes (qui sont soumises à la politique de rétention).

Un autre avantage de cette approche est que la recherche par attributs de personne est plus rapide que la recherche à travers les journaux d’activité des personnes.
