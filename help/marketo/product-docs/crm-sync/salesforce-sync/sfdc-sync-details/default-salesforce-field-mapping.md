---
unique-page-id: 4719314
description: Mappage des champs Salesforce par défaut - Documents Marketo - Documentation du produit
title: Mappage des champs Salesforce par défaut
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 57%

---

# Mappage des champs Salesforce par défaut {#default-salesforce-field-mapping}

Lors de la synchronisation initiale de votre compte de Marketo Engage avec Salesforce, Marketo crée automatiquement ces associations entre vos champs Salesforce et Marketo intégrés. Marketo synchronise également vos champs personnalisés sur vos pistes, comptes, opportunités et contacts.

## Champs de leads {#lead-fields}

| Champ SFDC | Champ Marketo |
|---|---|
| Chiffre d’affaires annuel | Chiffre d’affaires annuel |
| Ville | Ville |
| Société | Nom de l’entreprise |
| Date de conversion | Date conversion SFDC |
| Pays | Pays |
| Date créée | Date de création SFDC |
| Description | Notes du contact |
| E-mail | Adresse e-mail |
| Fax | Numéro de fax |
| Prénom | Prénom |
| Désabonnement par e-mail | Désabonné |
| Secteur | Secteur |
| Converti | est converti - SFDC |
| supprimé | Suppression de SFDC |
| Nom | Nom |
| Source du lead | Source |
| Évaluation des leads | Évaluation |
| Téléphone mobile | Numéro téléphone mobile |
| Employés | Nombre d’employés |
| Téléphone | Numéro de téléphone |
| Code postal | Code postal |
| Classement | Classement |
| Titre | Titre |
| État/province | État |
| Statut | Statut |
| Rue | Adresse |
| Titre | Intitulé du poste |
| Site Internet | Site Internet |

## Champs de contact {#contact-fields}

| Champ SFDC | Champ Marketo |
|---|---|
| Date de naissance | Date de naissance |
| Date créée | Date de création SFDC |
| Description du contact | Notes du contact |
| E-mail | Adresse e-mail |
| Télécopie professionnelle | Numéro de fax |
| Prénom | Prénom |
| Désabonnement par e-mail | Désabonné |
| supprimé | Suppression de SFDC |
| Nom | Nom |
| Source du lead | Source |
| Évaluation des leads | Évaluation |
| MailingCity | Ville |
| MailingCountry | Pays |
| MailingPostalCode | Code postal |
| MailingState | État |
| MailingStreet | Adresse |
| Téléphone mobile | Numéro téléphone mobile |
| Téléphone de l&#39;entreprise  | Numéro de téléphone |
| Titre | Titre |
| Titre | Intitulé du poste |

## Champs de compte {#account-fields}

| Champ SFDC | Champ Marketo |
|---|---|
| Chiffre d’affaires annuel | Chiffre d’affaires annuel |
| Ville de facturation | Ville de facturation |
| Pays de facturation | Pays de facturation |
| Code postal de facturation | Code postal de facturation |
| État/province de facturation | État de facturation |
| Rue de facturation | Adresse de facturation |
| Description du compte | Notes sur société |
| Secteur | Secteur |
| supprimé | Suppression de SFDC |
| Nom de compte | Nom de l’entreprise |
| Employés | Nombre d’employés |
| Téléphone du compte | Téléphone principal |
| Code SIC | Code SIC |
| Site du compte | Site |
| Type de compte | Type SFDC |
| Site Internet | Site Internet |

## Champs système associés à Salesforce dans Marketo (lecture seule) {#salesforce-related-system-fields-in-marketo-read-only}

Ces champs sont créés dans Marketo mais ne peuvent pas être ajustés par les clients.

| Champ | Description |
|---|---|
| ID SFDC | L’identifiant Salesforce à 18 caractères |
| Type SFDC | Prospérité ou Contact. S’il est vide, le prospect n’existe que comme une personne dans Marketo |
| Date de création SFDC | Date de création dans SFDC (peut différer de celle de création dans Marketo) |
| La collecte de données côté serveur est supprimée | La personne se trouvait auparavant dans la SFDC mais a été supprimée et vit désormais uniquement dans Marketo. |
