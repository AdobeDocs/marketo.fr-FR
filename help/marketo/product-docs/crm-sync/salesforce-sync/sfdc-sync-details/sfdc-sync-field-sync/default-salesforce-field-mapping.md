---
unique-page-id: 4719314
description: Mappage des champs Salesforce par défaut - Docs Marketo - Documentation du produit
title: Mappage des champs Salesforce par défaut
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 57%

---

# Mappage de champ Salesforce par défaut {#default-salesforce-field-mapping}

Lors de la synchronisation initiale de votre compte Marketo avec Salesforce, Marketo crée automatiquement ces associations entre vos champs intégrés Salesforce et Marketo. Marketo synchronise également vos champs personnalisés sur vos pistes, comptes, opportunités et contacts.

## Champs de leads {#lead-fields}

| Champ SFDC | Champ Marketo |
|---|---|
| Chiffre d&#39;affaires annuel | Chiffre d&#39;affaires annuel |
| Ville | Ville |
| Société | Nom de la société |
| Date de conversion | Date conversion SFDC |
| Pays | Pays |
| Date créée | Date de création SFDC |
| Description | Notes du contact |
| E-mails | Adresse e-mail |
| Fax | Numéro de fax |
| Prénom | Prénom |
| Désabonnement par e-mail | Désabonnement |
| Secteur | Secteur |
| Converti | est converti - SFDC |
| Supprimé | est supprimé - SFDC |
| Nom | Nom |
| Lead Source | Source |
| Évaluation des leads | Évaluation |
| Téléphone mobile | Numéro téléphone mobile |
| Employés | Nombre d&#39;employés |
| Téléphone | Numéro de téléphone |
| Code postal | Code postal |
| Classement | Classement |
| Titre | Titre |
| État/province | Pays |
| Statut | Statut |
| Rue | Adresse |
| Titre | Intitulé du poste |
| Site Internet | Site Internet |

## Champs contact {#contact-fields}

| Champ SFDC | Champ Marketo |
|---|---|
| Date de naissance | Date de naissance |
| Date créée | Date de création SFDC |
| Description du contact | Notes du contact |
| E-mails | Adresse e-mail |
| Télécopie professionnelle | Numéro de fax |
| Prénom | Prénom |
| Désabonnement par e-mail | Désabonnement |
| Supprimé | est supprimé - SFDC |
| Nom | Nom |
| Piste Source | Source |
| Évaluation des leads | Évaluation |
| MailingCity | Ville |
| MailingCountry | Pays |
| MailingPostalCode | Code postal |
| MailingState | Pays |
| MailingStreet | Adresse |
| Téléphone mobile | Numéro téléphone mobile |
| Téléphone de l&#39;entreprise  | Numéro de téléphone |
| Titre | Titre |
| Titre | Intitulé du poste |

## Champs de compte {#account-fields}

| Champ SFDC | Champ Marketo |
|---|---|
| Chiffre d&#39;affaires annuel | Chiffre d&#39;affaires annuel |
| Ville de facturation | Ville de facturation |
| Pays de facturation | Pays de facturation |
| Code postal de facturation | Code postal de facturation |
| État/Province de facturation | État de facturation |
| Rue de facturation | Adresse de facturation |
| Description du compte | Notes sur société |
| Secteur | Secteur |
| Supprimé | est supprimé - SFDC |
| Nom du compte | Nom de la société |
| Employés | Nombre d&#39;employés |
| Téléphone du compte | Téléphone principal |
| Code SIC | Code SIC |
| Site du compte | Site |
| Type de compte | Type SFDC |
| Site Internet | Site Internet |

## Champs système liés à Salesforce dans Marketo (lecture seule) {#salesforce-related-system-fields-in-marketo-read-only}

Ces champs sont créés dans Marketo mais ne peuvent pas être ajustés par les clients.

| Champ | Description |
|---|---|
| ID SFDC | ID Salesforce à 18 caractères |
| Type SFDC | Piste ou Contact. S&#39;il est vide, le prospect n&#39;existe qu&#39;en tant que personne à Marketo |
| Date de création SFDC | Date de création dans SFDC (peut être différente de Création dans Marketo) |
| SFDC est supprimé | La personne qui se trouvait auparavant à la DDC a été supprimée et ne vit désormais qu&#39;à Marketo. |
