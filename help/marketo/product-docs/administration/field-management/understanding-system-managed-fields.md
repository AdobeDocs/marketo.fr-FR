---
unique-page-id: 5472615
description: Présentation des champs gérés par le système - Documents Marketo - Documentation du produit
title: Présentation des champs gérés par le système
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 13%

---

# Présentation des champs gérés par le système {#understanding-system-managed-fields}

Vous avez peut-être remarqué que la [page des détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} comporte une série de champs non modifiables créés par Marketo. Ces données proviennent de diverses sources, et il y a d&#39;innombrables valeurs qui pourraient s&#39;afficher.

## Types de champ {#field-types}

| **Nom du champ** | **Définition** |
|---|---|
| Type de source d&#39;origine | L’emplacement de la première découverte d’une personne ou d’un visiteur du site web (par exemple : importation de liste, visite de page web) |
| Informations sur la source d&#39;origine | Informations spécifiques à cet emplacement (exemple : nom de la liste, URL de la page web) |
| Moteur de recherche d&#39;origine | Le cas échéant, le moteur de recherche qui a référé la personne à la source d’entrée d’origine |
| Phrase de recherche d&#39;origine | Le cas échéant, le terme de recherche utilisé qui a référé la personne à la source d’entrée d’origine |
| Référent d&#39;origine | URL qui hébergeait la source d’entrée d’origine |
| Type de source d&#39;inscription | L’emplacement où une activité est devenue une personne pour la première fois (par exemple : importation de liste, visite de page web) |
| Informations sur la source d&#39;inscription | Informations spécifiques à cet emplacement (exemple : nom de la liste, URL de la page web) |
| IP anonyme | Indique l’adresse IP d’une personne |
| Société déduite | Meilleure estimation de Marketo (en fonction de l’adresse IP) de la société de la personne |
| Ville déduite | Meilleure estimation de Marketo (basée sur l’IP) de la ville de la personne |
| Région déduite | Marketo : meilleure estimation (basée sur l’IP) de l’état ou de la région de la personne |
| Code postal déduit | Marketo : meilleure estimation (basée sur l’IP) du code postal de la personne |
| Pays déduit | Meilleure estimation de Marketo (en fonction de l’adresse IP) du pays de la personne |
| Aire métropolitaine déduite | Meilleure estimation de Marketo (en fonction de l’adresse IP) de la zone métropolitaine de la personne |
| Indicatif téléphonique local déduit | Marketo : meilleure estimation (basée sur l’IP) de l’indicatif régional de la personne |

## Valeurs possibles pour le type Source d’origine et d’enregistrement {#possible-values-for-original-and-registration-source-type}

Vous trouverez ci-dessous quelques valeurs possibles et leur signification.

| **Type Source original** | **Définition** |
|---|---|
| Salesforce.com | Une personne a été découverte à partir d’une synchronisation [!DNL Webhook] |
| Visites de page web | Une personne a été découverte sur une page web |
| Remplissage de formulaire web | Une personne a été découverte après avoir rempli un formulaire. |
| Importer une liste | Une personne a été découverte à partir d’un import de liste. |
| Nouvel individu | Personne a été saisie manuellement dans la base de données |
| Clic sur les liens web | Une personne a été découverte après avoir cliqué sur un lien. |
| Courriel de vente | Une personne a reçu un courrier électronique par l’intermédiaire du [!DNL Sales Insight] complément d’adresse électronique |
| Individu | Personne synchronisée depuis [!DNL Salesforce] en tant que personne |
| Contact | Personne synchronisée depuis [!DNL Webhook] en tant que contact |
| API [!DNL Munchkin] | La personne a été découverte par l&#39;API du Marketo Engage [!DNL Munchkin]. |
| App sociale | Une personne a été découverte par un widget social |
| API Web Service | Une personne a été découverte par une API de service Web |
| Partenaire événement | Une personne a été découverte par le biais d’un service de webinaire synchronisé. |
| Associer le lead | Personne fusionnée via l’appel de l’API de piste associée |

| **Type Source d’enregistrement** | **Définition** |
|---|---|
| Importer une liste | Devenir une personne par le biais d’un import de liste |
| Salesforce.com | Devenir une personne grâce à une synchronisation [!DNL Webhook] |
| Remplissage de formulaire web | Devenir une personne après avoir rempli un formulaire |
| Courriel de vente | Une personne a reçu un courrier électronique par l’intermédiaire du [!DNL Webhook] complément d’adresse électronique |
| API Web Service | La personne a été créée via l’API SOAP/REST |
| Nouvel individu | Personne a été saisie manuellement dans la base de données |
| API [!DNL Munchkin] | Devenir une personne grâce à l’API Marketo [!DNL Munchkin] |
| App sociale | Devenir une personne à travers un widget social |
| Partenaire événement | Devenir une personne via un service de webinaire lié |
