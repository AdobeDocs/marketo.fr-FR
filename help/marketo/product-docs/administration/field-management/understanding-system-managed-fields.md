---
unique-page-id: 5472615
description: Présentation des champs gérés par le système - Documents Marketo - Documentation du produit
title: Présentation des champs gérés par le système
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 16%

---

# Présentation des champs gérés par le système {#understanding-system-managed-fields}

Vous avez peut-être remarqué que la [page des détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) comporte une série de champs non modifiables créés par Marketo. Ces données proviennent de diverses sources, et il y a d&#39;innombrables valeurs qui pourraient s&#39;afficher.

## Types de champ {#field-types}

| **Nom de champ** | **Définition** |
|---|---|
| Type source d&#39;origine | L’emplacement d’une personne ou d’un visiteur de site Web a été découvert pour la première fois (exemple : Importation de liste, Visite de page Web) |
| Info source d&#39;origine | Spécifications de cet emplacement (Exemple : Nom de la liste, URL de la page Web) |
| Moteur de recherche d&#39;origine | Le cas échéant, le moteur de recherche qui a renvoyé la personne à la source d&#39;entrée originale |
| Phrase de recherche d&#39;origine | Le cas échéant, le terme de recherche utilisé pour désigner la personne à la source d&#39;entrée originale. |
| Référent d&#39;origine | URL qui hébergeait la source d’entrée d’origine |
| Type source d&#39;inscription | L&#39;endroit où une activité est devenue une personne pour la première fois (Exemple : Importation de liste, Visite de page Web) |
| Info source d&#39;inscription | Spécifications de cet emplacement (Exemple : Nom de la liste, URL de la page Web) |
| IP anonyme | Indique l’adresse IP d’une personne |
| Société déduite | Marketo de la meilleure estimation (basée sur la PI) de la société de la personne |
| Ville déduite | Marketo la meilleure estimation (basée sur l&#39;adresse IP) de la ville de la personne |
| Région déduite | Marketo de la meilleure estimation (en fonction de l’IP) de l’état ou de la région de la personne |
| Code postal déduit | Marketo de la meilleure estimation (basée sur l&#39;adresse IP) du code postal de la personne |
| Pays déduit | Marketo de la meilleure estimation (basée sur la PI) du pays de la personne |
| Aire métropolitaine déduite | Marketo la meilleure estimation (basée sur la PI) de la zone métropolitaine de la personne |
| Indicatif téléphonique local déduit | Marketo de la meilleure estimation (en fonction de l’adresse IP) de l’indicatif régional de la personne |

## Valeurs possibles pour l&#39;original et le type de source d&#39;enregistrement {#possible-values-for-original-and-registration-source-type}

Voici quelques valeurs possibles et ce qu&#39;elles signifient.

| **Type source d&#39;origine** | **Définition** |
|---|---|
| Salesforce.com | Une personne a été découverte à partir d&#39;une synchronisation Salesforce |
| Visites de page Web | Une personne a été découverte à partir d’une page Web. |
| Remplissage de formulaire Web | Une personne a été découverte après avoir rempli un formulaire. |
| Importer une liste | Une personne a été découverte à partir d&#39;une importation de liste |
| Nouvel individu | La personne a été saisie manuellement dans la base de données |
| Click de lien Web | Une personne a été découverte après avoir cliqué sur un lien. |
| Courriel de vente | Une personne a été envoyée par courrier électronique via l&#39;Ajoute électronique de Sales Insight |
| Individu | Une personne a été synchronisée depuis Salesforce en tant que personne. |
| Contact | La personne a été synchronisée depuis Salesforce en tant que contact |
| Munchkin API | Une personne a été découverte par Marketo l&#39;API Munchkin |
| App sociale | Une personne a été découverte par un widget social. |
| API Web Service | Une personne a été découverte par une API de service Web |
| Partenaire événement | Une personne a été découverte par le biais d’un service de webinaires synchronisé. |
| Associer le lead | Personne fusionnée via l&#39;appel de l&#39;API de piste associée |

| **Type source d&#39;inscription** | **Définition** |
|---|---|
| Importer une liste | Est devenu une personne par le biais d’une importation de liste |
| Salesforce.com | Devenir une personne grâce à une synchronisation Salesforce |
| Remplissage de formulaire Web | Devenir une personne après avoir rempli un formulaire |
| Courriel de vente | Une personne a été envoyée par courrier électronique via l&#39;Ajoute électronique de Sales Insight |
| API Web Service | La personne a été créée via l’API SOAP/REST. |
| Nouvel individu | La personne a été saisie manuellement dans la base de données |
| API Munchkin | Est devenu une personne grâce à l&#39;API Marketo Munchkin |
| App sociale | Devenir une personne par le biais d’un widget social |
| Partenaire événement | Devenir une personne par le biais d’un service de webinaire lié |
