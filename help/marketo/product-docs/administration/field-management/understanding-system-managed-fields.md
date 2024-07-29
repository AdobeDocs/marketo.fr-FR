---
unique-page-id: 5472615
description: Présentation des champs gérés par le système - Documents Marketo - Documentation du produit
title: Présentation des champs gérés par le système
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: fc25a088005ee1d552f6e61e2fa7b953e2fde862
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 16%

---

# Présentation des champs gérés par le système {#understanding-system-managed-fields}

Vous avez peut-être remarqué que la [page des détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} comporte une série de champs non modifiables créés par Marketo. Ces données proviennent de diverses sources, et il y a d&#39;innombrables valeurs qui pourraient s&#39;afficher.

## Types de champ {#field-types}

<table><thead>
  <tr>
    <th>Nom du champ</th>
    <th>Définition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Type de source d'origine</td>
    <td>L’emplacement de la première découverte d’une personne ou d’un visiteur du site web (par exemple : importation de liste, visite de page web)</td>
  </tr>
  <tr>
    <td>Informations sur la source d'origine</td>
    <td>Informations spécifiques à cet emplacement (exemple : nom de la liste, URL de la page web)</td>
  </tr>
  <tr>
    <td>Moteur de recherche d'origine</td>
    <td>Le cas échéant, le moteur de recherche qui a référé la personne à la source d’entrée d’origine</td>
  </tr>
  <tr>
    <td>Phrase de recherche d'origine</td>
    <td>Le cas échéant, le terme de recherche utilisé qui a référé la personne à la source d’entrée d’origine</td>
  </tr>
  <tr>
    <td>Référent d'origine</td>
    <td>URL qui hébergeait la source d’entrée d’origine</td>
  </tr>
  <tr>
    <td>Type de source d'inscription</td>
    <td>L’emplacement où une activité est devenue une personne pour la première fois (par exemple : importation de liste, visite de page web)</td>
  </tr>
  <tr>
    <td>Informations sur la source d'inscription</td>
    <td>Informations spécifiques à cet emplacement (exemple : nom de la liste, URL de la page web)</td>
  </tr>
  <tr>
    <td>IP anonyme</td>
    <td>Indique l’adresse IP d’une personne</td>
  </tr>
  <tr>
    <td>Société déduite</td>
    <td>Meilleure estimation de Marketo (en fonction de l’adresse IP) de la société de la personne</td>
  </tr>
  <tr>
    <td>Ville déduite</td>
    <td>Meilleure estimation de Marketo (basée sur l’IP) de la ville de la personne</td>
  </tr>
  <tr>
    <td>Région déduite</td>
    <td>Marketo : meilleure estimation (basée sur l’IP) de l’état ou de la région de la personne</td>
  </tr>
  <tr>
    <td>Code postal déduit</td>
    <td>Marketo : meilleure estimation (basée sur l’IP) du code postal de la personne</td>
  </tr>
  <tr>
    <td>Pays déduit</td>
    <td>Meilleure estimation de Marketo (en fonction de l’adresse IP) du pays de la personne</td>
  </tr>
  <tr>
    <td>Aire métropolitaine déduite</td>
    <td>Meilleure estimation de Marketo (en fonction de l’adresse IP) de la zone métropolitaine de la personne</td>
  </tr>
  <tr>
    <td>Indicatif téléphonique local déduit</td>
    <td>Marketo : meilleure estimation (basée sur l’IP) de l’indicatif régional de la personne</td>
  </tr>
</tbody></table>

## Valeurs possibles pour le type Source d’origine et d’enregistrement {#possible-values-for-original-and-registration-source-type}

Vous trouverez ci-dessous quelques valeurs possibles et leur signification.

<table><thead>
  <tr>
    <th>Type de source d'origine</th>
    <th>Définition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>Une personne a été découverte à partir de la synchronisation Salesforce</td>
  </tr>
  <tr>
    <td>Visites de page web</td>
    <td>Une personne a été découverte sur une page web</td>
  </tr>
  <tr>
    <td>Remplissage de formulaire web</td>
    <td>Une personne a été découverte après avoir rempli un formulaire.</td>
  </tr>
  <tr>
    <td>Importer une liste</td>
    <td>Une personne a été découverte à partir d’un import de liste.</td>
  </tr>
  <tr>
    <td>Nouvel individu</td>
    <td>Personne a été saisie manuellement dans la base de données</td>
  </tr>
  <tr>
    <td>Clic sur les liens web</td>
    <td>Une personne a été découverte après avoir cliqué sur un lien.</td>
  </tr>
  <tr>
    <td>Courriel de vente</td>
    <td>Une personne a reçu un e-mail via le module complémentaire d’e-mail Sales Insight</td>
  </tr>
  <tr>
    <td>Personne</td>
    <td>Personne a été synchronisée depuis Salesforce en tant que personne.</td>
  </tr>
  <tr>
    <td>Contact</td>
    <td>Personne synchronisée depuis Webhook en tant que contact</td>
  </tr>
  <tr>
    <td>API Munchkin</td>
    <td>Une personne a été découverte par l’API Munchkin Marketo Engage.</td>
  </tr>
  <tr>
    <td>App sociale</td>
    <td>Une personne a été découverte par un widget social</td>
  </tr>
  <tr>
    <td>API Web Service</td>
    <td>Une personne a été découverte par une API de service Web</td>
  </tr>
  <tr>
    <td>Partenaire événement</td>
    <td>Une personne a été découverte par le biais d’un service de webinaire synchronisé.</td>
  </tr>
  <tr>
    <td>Association au prospect</td>
    <td>Personne fusionnée via l’appel de l’API de piste associée</td>
  </tr>
</tbody></table>

<table><thead>
  <tr>
    <th>Type de source d'inscription</th>
    <th>Définition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Importer une liste</td>
    <td>Devenir une personne par le biais d’un import de liste</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>Devenir une personne grâce à la synchronisation Salesforce</td>
  </tr>
  <tr>
    <td>Remplissage de formulaire web</td>
    <td>Devenir une personne après avoir rempli un formulaire</td>
  </tr>
  <tr>
    <td>Courriel de vente</td>
    <td>Une personne a reçu un e-mail via le module complémentaire d’e-mail Sales Insight</td>
  </tr>
  <tr>
    <td>API Web Service</td>
    <td>La personne a été créée via l’API SOAP/REST</td>
  </tr>
  <tr>
    <td>Nouvel individu</td>
    <td>Personne a été saisie manuellement dans la base de données</td>
  </tr>
  <tr>
    <td>API Munchkin</td>
    <td>Devenir une personne grâce à l’API Marketo Munchkin</td>
  </tr>
  <tr>
    <td>App sociale</td>
    <td>Devenir une personne à travers un widget social</td>
  </tr>
  <tr>
    <td>Partenaire événement</td>
    <td>Devenir une personne via un service de webinaire lié</td>
  </tr>
</tbody>
</table>
