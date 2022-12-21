---
unique-page-id: 5472615
description: Présentation des champs gérés par le système - Documents Marketo - Documentation du produit
title: Présentation des champs gérés par le système
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 16%

---

# Présentation des champs gérés par le système {#understanding-system-managed-fields}

Vous avez peut-être remarqué que la variable [page des détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) comporte une série de champs non modifiables créés par Marketo. Ces données proviennent de diverses sources, et il y a d&#39;innombrables valeurs qui pourraient s&#39;afficher.

## Types de champ {#field-types}

| **Nom de champ** | **Définition** |
|---|---|
| Type source d&#39;origine | L’emplacement où une personne ou un visiteur du site web a été découvert pour la première fois (par exemple : Importation de liste, Visite de page web) |
| Info source d&#39;origine | Informations spécifiques à cet emplacement (exemple : Nom de la liste, URL de la page web) |
| Moteur de recherche d&#39;origine | Le cas échéant, le moteur de recherche qui a référé la personne à la source d’entrée d’origine |
| Phrase de recherche d&#39;origine | Le cas échéant, le terme de recherche utilisé qui a référé la personne à la source d’entrée d’origine |
| Référent d&#39;origine | URL qui hébergeait la source d’entrée d’origine |
| Type source d&#39;inscription | L’emplacement où une activité est devenue une personne pour la première fois (par exemple : Importation de liste, Visite de page web) |
| Info source d&#39;inscription | Informations spécifiques à cet emplacement (exemple : Nom de la liste, URL de la page web) |
| IP anonyme | Indique l’adresse IP d’une personne |
| Société déduite | Meilleure estimation de Marketo (en fonction de l’adresse IP) de la société de la personne |
| Ville déduite | Meilleure estimation de Marketo (basée sur l’IP) de la ville de la personne |
| Région déduite | Marketo : meilleure estimation (basée sur l’IP) de l’état ou de la région de la personne |
| Code postal déduit | Marketo : meilleure estimation (basée sur l’IP) du code postal de la personne |
| Pays déduit | Meilleure estimation de Marketo (en fonction de l’adresse IP) du pays de la personne |
| Aire métropolitaine déduite | Meilleure estimation de Marketo (en fonction de l’adresse IP) de la zone métropolitaine de la personne |
| Indicatif téléphonique local déduit | Marketo : meilleure estimation (basée sur l’IP) de l’indicatif régional de la personne |

## Valeurs possibles pour le type original et source d’enregistrement {#possible-values-for-original-and-registration-source-type}

Vous trouverez ci-dessous quelques valeurs possibles et leur signification.

| **Type source d&#39;origine** | **Définition** |
|---|---|
| Salesforce.com | Une personne a été découverte à partir d’une synchronisation Salesforce. |
| Visites de page web | Une personne a été découverte à partir d’une page web |
| Remplissage de formulaire web | Une personne a été découverte après le remplissage d’un formulaire. |
| Importer une liste | Une personne a été découverte à partir d’un import de liste |
| Nouvel individu | Personne a été saisie manuellement dans la base de données |
| Clic sur les liens web | Une personne a été découverte après avoir cliqué sur un lien. |
| Courriel de vente | Une personne a reçu un e-mail via le module complémentaire d’e-mail Sales Insight |
| Individu | Personne a été synchronisée depuis Salesforce en tant que personne. |
| Contact | Personne synchronisée depuis Salesforce en tant que contact |
| Munchkin API | Une personne a été découverte par l’API Marketo Munchkin. |
| App sociale | Une personne a été découverte par un widget social |
| API Web service | Une personne a été découverte par une API de service Web. |
| Partenaire événement | Une personne a été découverte par le biais d’un service de webinaire synchronisé. |
| Associer le lead | Personne fusionnée via l’appel de l’API de piste associée |

| **Type source d&#39;inscription** | **Définition** |
|---|---|
| Importer une liste | Devenir une personne par le biais d’un import de liste |
| Salesforce.com | Devenir une personne par le biais d’une synchronisation Salesforce |
| Remplissage de formulaire web | Devenir une personne après avoir rempli un formulaire |
| Courriel de vente | Une personne a reçu un e-mail via le module complémentaire d’e-mail Sales Insight |
| API Web service | La personne a été créée via l&#39;API SOAP/REST |
| Nouvel individu | Personne a été saisie manuellement dans la base de données |
| Munchkin API | Devenir une personne grâce à l’API Marketo Munchkin |
| App sociale | Devenir une personne à travers un widget social |
| Partenaire événement | Devenir une personne par le biais d’un service de webinaire lié |
