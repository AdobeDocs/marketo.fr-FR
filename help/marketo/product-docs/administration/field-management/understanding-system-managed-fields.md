---
unique-page-id: 5472615
description: Présentation des champs gérés par le système - Documents marketing - Documentation du produit
title: Présentation des champs gérés par le système
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Présentation des champs gérés par le système {#understanding-system-managed-fields}

Vous avez peut-être remarqué que la page [des détails de la](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) personne comporte une série de champs non modifiables créés par Marketo. Ces données proviennent de diverses sources, et il y a d&#39;innombrables valeurs qui pourraient s&#39;afficher.

## Types de champ {#field-types}

| **Nom du champ** | **Définition** |
|---|---|
| Type de source original | L’emplacement d’une personne ou d’un visiteur de site Web a été découvert pour la première fois (exemple : Importation de liste, Visite de page Web) |
| Infos source d&#39;origine | Spécifications de cet emplacement (Exemple : Nom de la liste, URL de la page Web) |
| Moteur de recherche original | Le cas échéant, le moteur de recherche qui a renvoyé la personne à la source d&#39;entrée originale |
| Expression de recherche d’origine | Le cas échéant, le terme de recherche utilisé pour désigner la personne à la source d&#39;entrée originale. |
| Parrain original | URL qui hébergeait la source d’entrée d’origine |
| Type de source d&#39;enregistrement | L&#39;endroit où une activité est devenue une personne pour la première fois (Exemple : Importation de liste, Visite de page Web) |
| Informations sur la source d&#39;enregistrement | Spécifications de cet emplacement (Exemple : Nom de la liste, URL de la page Web) |
| IP anonyme | Indique l’adresse IP d’une personne |
| Société déduite | La meilleure estimation du marché (basée sur l&#39;IP) de la société de la personne |
| Ville d&#39;origine | La meilleure estimation du marché (basée sur l&#39;adresse IP) de la ville de la personne |
| Région d&#39;État désignée | La meilleure estimation du marché (basée sur l’adresse IP) de l’état ou de la région de la personne |
| Code postal déduit | La meilleure estimation du marché (basée sur l&#39;adresse IP) du code postal de la personne |
| Pays d&#39;origine | La meilleure estimation du marché (basée sur l&#39;adresse IP) du pays de la personne |
| Zone métropolitaine désignée | La meilleure estimation du marché (basée sur l&#39;IP) de la zone métropolitaine de la personne |
| Code de zone de téléphone indiqué | La meilleure estimation du marché (basée sur l’adresse IP) de l’indicatif régional de la personne |

## Valeurs possibles pour l’original et le type de source d’enregistrement {#possible-values-for-original-and-registration-source-type}

Voici quelques valeurs possibles et ce qu&#39;elles signifient.

| **Type de source original** | **Définition** |
|---|---|
| Salesforce.com | Une personne a été découverte à partir d&#39;une synchronisation Salesforce |
| Visites de page Web | Une personne a été découverte à partir d’une page Web. |
| Remplissage de formulaire Web | Une personne a été découverte après avoir rempli un formulaire. |
| Importation liste | Une personne a été découverte à partir d&#39;une importation de liste |
| Nouvelle personne | La personne a été saisie manuellement dans la base de données |
| Click de lien Web | Une personne a été découverte après avoir cliqué sur un lien. |
| Courriel de vente | Une personne a été envoyée par courrier électronique via l&#39;Ajoute électronique de Sales Insight |
| Personne | Une personne a été synchronisée depuis Salesforce en tant que personne. |
| Contact | La personne a été synchronisée depuis Salesforce en tant que contact |
| API Munchkin | Une personne a été découverte par l&#39;API Munchkin de Marketo |
| Application Social | Une personne a été découverte par un widget social. |
| API du service Web | Une personne a été découverte par une API de service Web |
| Partenaire événement | Une personne a été découverte par le biais d’un service de webinaires synchronisé. |
| Responsable associé | Personne fusionnée via l&#39;appel de l&#39;API de piste associée |

| **Type de source d&#39;enregistrement** | **Définition** |
|---|---|
| Importation liste | Est devenu une personne par le biais d’une importation de liste |
| Salesforce.com | Devenir une personne grâce à une synchronisation Salesforce |
| Remplissage de formulaire Web | Devenir une personne après avoir rempli un formulaire |
| Courriel de vente | Une personne a été envoyée par courrier électronique via l&#39;Ajoute électronique de Sales Insight |
| API du service Web | La personne a été créée via l’API SOAP/REST. |
| Nouvelle personne | La personne a été saisie manuellement dans la base de données |
| API Munchkin | Est devenu une personne grâce à l&#39;API Munchkin de Marketo |
| Application Social | Devenir une personne par le biais d’un widget social |
| Partenaire événement | Devenir une personne par le biais d’un service de webinaire lié |

