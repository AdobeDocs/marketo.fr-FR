---
description: Notes de mise à jour - Juin 2022 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Juin 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Notes de mise à jour : juin 2022 {#release-notes-june-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 juin. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

Les fonctionnalités suivantes commenceront à être publiées le **24 juin 2022**, avec un déploiement progressif des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire).

## Environnement de données marketing {#marketing-data-environment}

* **Exposer les champs CreatedAt/UpdatedAt pour les objets personnalisés** : vous permet d’examiner ces champs dans l’écran Détails de la personne pour obtenir des informations supplémentaires.

## Orchestration cross-canal {#cross-channel-orchestration}

* **Amélioration de l’utilisation de Stream Designer pour Dynamic Chat** : ajoutez des cartes directement à partir du canevas Stream Designer sans avoir à effectuer un glisser-déposer. L’interface du Dynamic Chat a également été améliorée afin d’offrir une meilleure visibilité du contenu dans les cartes individuelles.

* **Règles de routage de rendez-vous avancées pour le Dynamic Chat** : Dynamic Chat offre davantage d’options de routage de rendez-vous ciblé. Spécifiez les nominations d’agent à router en fonction des attributs du Marketo Engage, en veillant à ce que les prospects soient acheminés vers les agents appropriés.

* **Création de rapports de dialogue avancé pour les Dynamic Chat** : affichez plus en détail les performances de vos campagnes Dynamic Chat à l’aide de toutes nouvelles visualisations de données pour les mesures d’engagement et de conversion.

* **Attributs de Marketo Engage non synchronisés pour Dynamic Chat** : attributs de Marketo Engage non synchronisés de votre abonnement de Dynamic Chat qui restent inutilisés, ce qui vous permet de faciliter la propreté des données et de synchroniser d’autres attributs selon vos besoins.

## Expérience de nouvelle génération

**Nouvelles vues de basculement** : les vues ci-dessous sont désormais disponibles dans l’expérience de nouvelle génération :

* [Affichage des détails d’un email](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Affichage de liste d’emails](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automatisation de l’expérience {#experience-automation}

* **Exclusions de règles de validation de champ de formulaire global** : excluez des formulaires spécifiques des règles de validation de formulaire globales pour que les centres d’abonnement et autres processus métier critiques puissent accepter toutes les valeurs.

* **Étapes de flux en libre-service** : développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes dynamiques. Les utilisateurs Marketo Engage et les partenaires peuvent exploiter cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes Trigger, Batch et Exécutable, contrairement aux webhooks, qui ne peuvent être utilisés que dans les campagnes Trigger.

* **Suivi des liens agnostique du protocole Munchkin** : étendez la prise en charge du suivi des liens `tel` et `mailto` avec Munchkin pour suivre un ensemble étendu de comportements web.

* **Méthodes HTTP supplémentaires pour les webhooks** : spécifiez PUT, PATCH et DELETE comme types de requête pour interagir avec les services web.

## Sales Insight {#sales-insight}

![(star)](assets/yellow-star.png)

* **Jeu d’autorisations Sales Insight dans Salesforce** : les administrateurs peuvent fournir un accès Sales Insight à un nombre limité de personnes au niveau de l’utilisateur plutôt qu’au niveau du profil par le biais de l’ensemble d’autorisations Marketo App, qui fait partie du package Sales Insight Salesforce.

* **Mise à jour de la mosaïque Mon Marketo - Actions d’aperçu des ventes** : les administrateurs de Marketo (et les utilisateurs qu’ils désignent) peuvent désormais accéder rapidement à leur instance d’actions d’aperçu des ventes via une nouvelle mosaïque d’actions d’aperçu des ventes située sur la page Mon Marketo.

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **Mise à jour de l’API Salesforce** : avec la version d’été 22 de Salesforce, les versions héritées de l’API 21-30 ne seront plus prises en charge par Salesforce. Avec cette version de Marketo Engage, toutes les demandes de Sales Connect utilisant des versions d’API héritées ont été mises à jour afin de rester dans une version prise en charge. Pour plus d’informations sur les plans de retraite de l’API Salesforce, cliquez [ici](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## Améliorations des API {#api-enhancements}

* **Nouvelles fonctionnalités de filtrage pour l’API Bulk Program Adtract** : filtrez par statut d’adhésion au programme, mise à jour d’At, de cadence ou de contenu épuisé pour affiner le jeu de données extrait.

* **Amélioration de l’API d’extraction de membre de programme en masse** : spécifiez jusqu’à 10 programmes pendant la création de tâche pour améliorer le débit.

## Annonces {#announcements}

* **Dépréciation de Forms - Forms 1.0, point de terminaison Capture/enregistrement de piste et versions sans script des formulaires** : la prise en charge des ressources Forms 1.0 sera complètement supprimée de Marketo Engage d’ici octobre 2022. Toutes les ressources Forms 1.0 existantes cesseront de fonctionner. Les formulaires Marketo Engage nécessitent JavaScript pour être chargés sur les landing pages et les sites web.

**_Webinaire sur la version du produit_**

[Webinaire de mise à jour des Marketo Engage de juin et août 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
