---
unique-page-id: 4719314
description: Mappage des champs Salesforce par défaut - Documents marketing - Documentation du produit
title: Mappage des champs Salesforce par défaut
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Mappage des champs Salesforce par défaut {#default-salesforce-field-mapping}

Lors de la synchronisation initiale de votre compte Marketo avec Salesforce, Marketo crée automatiquement ces associations entre vos champs intégrés Salesforce et Marketo. Marketo synchronise également vos champs personnalisés sur vos pistes, comptes, opportunités et contacts.

## Champs de piste {#lead-fields}

| Champ SFDC | Champ Marketo |
|---|---|
| Recettes annuelles | Recettes annuelles |
| Ville | Ville |
| Société | Nom de la société |
| Date de conversion | Date de conversion SFDC |
| Pays | Pays |
| Date de création | Date de création SFDC |
| Description | Notes sur les personnes |
| Courriel | Adresse électronique |
| Télécopie | Numéro de télécopie |
| Prénom | Prénom |
| Opt-out par courriel | Non abonné |
| Industrie | Industrie |
| Converti | La collecte de données régionale est convertie |
| Supprimé | La collecte de données régionale est supprimée |
| Nom | Nom |
| Source du prospect | Source |
| Note de piste | Score |
| Téléphone mobile | Numéro de téléphone mobile |
| Employés | Nombre d&#39;employés |
| Téléphone | Numéro de téléphone |
| Code postal | Code postal |
| Évaluation | Évaluation |
| Salutation | Salutation |
| Etat/Province | État |
| Statut | Statut |
| Rue | Adresse |
| Titre | Titre de la tâche |
| Site Web | Site Web |

## Champs de contact {#contact-fields}

| Champ SFDC | Champ Marketo |
|---|---|
| Anniversaire | Date de naissance |
| Date de création | Date de création SFDC |
| Description du contact | Notes sur les personnes |
| Courriel | Adresse électronique |
| Télécopie professionnelle | Numéro de télécopie |
| Prénom | Prénom |
| Opt-out par courriel | Non abonné |
| Supprimé | La collecte de données régionale est supprimée |
| Nom | Nom |
| Source du prospect | Source |
| Note de piste | Score |
| MailingCity | Ville |
| MailingCountry | Pays |
| MailingPostalCode | Code postal |
| MailingState | État |
| MailingStreet | Adresse |
| Téléphone mobile | Numéro de téléphone mobile |
| Téléphone professionnel | Numéro de téléphone |
| Salutation | Salutation |
| Titre | Titre de la tâche |

## Champs du compte {#account-fields}

| Champ SFDC | Champ Marketo |
|---|---|
| Recettes annuelles | Recettes annuelles |
| Ville de facturation | Ville de facturation |
| Pays de facturation | Pays de facturation |
| Code postal de facturation | Code postal de facturation |
| État/Province de facturation | État de la facturation |
| Rue de facturation | Adresse de facturation |
| Description du compte | Notes de société |
| Industrie | Industrie |
| Supprimé | La collecte de données régionale est supprimée |
| Nom du compte | Nom de la société |
| Employés | Nombre d&#39;employés |
| Téléphone du compte | Téléphone principal |
| Code SIC | Code SIC |
| Site du compte | Site |
| Type de compte | Type SFDC |
| Site Web | Site Web |

## Champs système liés à Salesforce dans Marketo (lecture seule) {#salesforce-related-system-fields-in-marketo-read-only}

Ces champs sont créés dans Marketing mais ne peuvent pas être ajustés par les clients.

| Champ | Description |
|---|---|
| ID SFDC | ID Salesforce à 18 caractères |
| Type SFDC | Piste ou Contact. S&#39;il est vide, le prospect n&#39;existe qu&#39;en tant que personne sur le marché |
| Date de création SFDC | Date de création dans SFDC (peut être différente de la date de création dans Marketo) |
| SFDC est supprimé | La personne qui se trouvait auparavant à la DDC a été supprimée et ne vit désormais qu&#39;à Marketo. |
