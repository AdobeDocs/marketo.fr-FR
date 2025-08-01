---
unique-page-id: 5472615
description: Comprendre les champs gérés par le système - Documentation de Marketo - Documentation du produit
title: Comprendre les champs gérés par le système
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 16%

---

# Comprendre les champs gérés par le système {#understanding-system-managed-fields}

Vous avez peut-être remarqué que la page [détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} comporte une série de champs non modifiables créés par Marketo. Ces données proviennent de diverses sources et d’innombrables valeurs peuvent s’afficher.

## Types de champs {#field-types}

<table><thead>
  <tr>
    <th>Nom du champ</th>
    <th>Définition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Type de source d'origine</td>
    <td>Emplacement où une personne ou un visiteur du site web a été découvert pour la première fois (exemple : importation de liste, visite de page web).</td>
  </tr>
  <tr>
    <td>Informations sur la source d'origine</td>
    <td>Détails relatifs à cet emplacement (exemple : nom de la liste, URL de la page web)</td>
  </tr>
  <tr>
    <td>Moteur de recherche d'origine</td>
    <td>Le cas échéant, moteur de recherche qui a renvoyé la personne à la source d’entrée d’origine</td>
  </tr>
  <tr>
    <td>Phrase de recherche d'origine</td>
    <td>Le cas échéant, terme de recherche utilisé qui a référencé la personne à la source d’entrée d’origine</td>
  </tr>
  <tr>
    <td>Référent d'origine</td>
    <td>URL qui a hébergé la source d’entrée originale</td>
  </tr>
  <tr>
    <td>Type de source d'inscription</td>
    <td>Emplacement où une activité est devenue pour la première fois une personne (exemple : importation de liste, visite de page web).</td>
  </tr>
  <tr>
    <td>Informations sur la source d'inscription</td>
    <td>Détails relatifs à cet emplacement (exemple : nom de la liste, URL de la page web)</td>
  </tr>
  <tr>
    <td>IP anonyme</td>
    <td>Indique l’adresse IP d’une personne</td>
  </tr>
  <tr>
    <td>Société déduite</td>
    <td>Meilleure estimation du Marketo (en fonction de l’adresse IP) de la société de la personne</td>
  </tr>
  <tr>
    <td>Ville déduite</td>
    <td>Meilleure estimation du Marketo (basée sur l’adresse IP) de la ville de la personne</td>
  </tr>
  <tr>
    <td>Région déduite</td>
    <td>Meilleure estimation du Marketo (basée sur l’adresse IP) de l’état ou de la région de la personne</td>
  </tr>
  <tr>
    <td>Code postal déduit</td>
    <td>Meilleure estimation du Marketo (en fonction de l’adresse IP) du code postal de la personne</td>
  </tr>
  <tr>
    <td>Pays déduit</td>
    <td>Meilleure estimation du Marketo (basée sur l’adresse IP) du pays de la personne</td>
  </tr>
  <tr>
    <td>Aire métropolitaine déduite</td>
    <td>Meilleure estimation du Marketo (basée sur l’adresse IP) de la zone métropolitaine de la personne</td>
  </tr>
  <tr>
    <td>Indicatif téléphonique local déduit</td>
    <td>Meilleure estimation du Marketo (basée sur l’adresse IP) de l’indicatif régional de la personne</td>
  </tr>
</tbody></table>

## Valeurs possibles pour l’original et le type de Source d’enregistrement {#possible-values-for-original-and-registration-source-type}

Vous trouverez ci-dessous quelques valeurs possibles et leur signification.

<table><thead>
  <tr>
    <th>Type de source d'origine</th>
    <th>Définition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>La personne a été découverte à partir de la synchronisation Salesforce.</td>
  </tr>
  <tr>
    <td>Visites de page web</td>
    <td>La personne a été découverte à partir d’une page web.</td>
  </tr>
  <tr>
    <td>Remplissage de formulaire web</td>
    <td>La personne a été découverte après avoir rempli un formulaire.</td>
  </tr>
  <tr>
    <td>Importer une liste</td>
    <td>La personne a été découverte à partir d’un import de liste</td>
  </tr>
  <tr>
    <td>Nouvel individu</td>
    <td>La personne a été saisie manuellement dans la base de données</td>
  </tr>
  <tr>
    <td>Clic sur le lien web</td>
    <td>La personne a été découverte après avoir cliqué sur un lien</td>
  </tr>
  <tr>
    <td>E-mail de vente</td>
    <td>Un courrier électronique a été envoyé à la personne via le complément de messagerie de Sales Insight</td>
  </tr>
  <tr>
    <td>Personne</td>
    <td>La personne a été synchronisée à partir de Salesforce en tant que personne</td>
  </tr>
  <tr>
    <td>Contact</td>
    <td>La personne a été synchronisée à partir du Webhook en tant que contact</td>
  </tr>
  <tr>
    <td>API Munchkin</td>
    <td>La personne a été découverte par l’API Marketo Engage Munchkin.</td>
  </tr>
  <tr>
    <td>App sociale</td>
    <td>La personne a été découverte par un widget social.</td>
  </tr>
  <tr>
    <td>API Web Service</td>
    <td>La personne a été découverte par une API de service web.</td>
  </tr>
  <tr>
    <td>Partenaire événement</td>
    <td>La personne a été découverte via un service de webinaire synchronisé.</td>
  </tr>
  <tr>
    <td>Association au prospect</td>
    <td>Personne fusionnée via l’appel de l’API du lead associé</td>
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
    <td>Devenez une personne par le biais d’un import de liste</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>Devenir une personne via la synchronisation Salesforce</td>
  </tr>
  <tr>
    <td>Remplissage de formulaire web</td>
    <td>Devenez une personne après avoir rempli un formulaire</td>
  </tr>
  <tr>
    <td>E-mail de vente</td>
    <td>Un courrier électronique a été envoyé à la personne via le complément de messagerie de Sales Insight</td>
  </tr>
  <tr>
    <td>API Web Service</td>
    <td>La personne a été créée via l’API SOAP/REST.</td>
  </tr>
  <tr>
    <td>Nouvel individu</td>
    <td>La personne a été saisie manuellement dans la base de données</td>
  </tr>
  <tr>
    <td>API Munchkin</td>
    <td>Devenir une personne via l’API Munchkin Marketo</td>
  </tr>
  <tr>
    <td>App sociale</td>
    <td>Devenir une personne via un widget social</td>
  </tr>
  <tr>
    <td>Partenaire événement</td>
    <td>Devenez une personne via un service de webinaire lié</td>
  </tr>
</tbody>
</table>
