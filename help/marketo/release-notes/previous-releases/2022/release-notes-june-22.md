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
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

Les fonctionnalités suivantes commenceront à être publiées sur **24 juin 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire).

## Environnement de données marketing {#marketing-data-environment}

* **Exposer les champs CreatedAt/UpdatedAt pour les objets personnalisés**: vous donne la possibilité d’examiner ces champs dans l’écran Détails de la personne pour obtenir des informations supplémentaires.

## Orchestration cross-canal {#cross-channel-orchestration}

* **Amélioration de l’utilisation du concepteur de flux pour Dynamic Chat**: ajoutez des cartes directement à partir du canevas du Concepteur de flux sans avoir à les faire glisser. L’interface du Dynamic Chat a également été améliorée afin d’offrir une meilleure visibilité du contenu dans les cartes individuelles.

* **Règles de routage de rendez-vous avancées pour Dynamic Chat**: Dynamic Chat offre davantage d’options pour le routage des rendez-vous ciblés. Spécifiez les nominations d’agent à router en fonction des attributs du Marketo Engage, en veillant à ce que les prospects soient acheminés vers les agents appropriés.

* **Création de rapports de dialogue avancés pour le Dynamic Chat**: affichez plus en détail les performances de vos campagnes Dynamic Chat à l’aide de toutes nouvelles visualisations de données pour les mesures d’engagement et de conversion.

* **Attributs de Marketo Engage non synchronisés pour Dynamic Chat**: attributs de Marketo Engage non synchronisés de votre abonnement de Dynamic Chat qui restent inutilisés, ce qui vous permet de faciliter la propreté des données et de synchroniser d’autres attributs si nécessaire.

## Expérience de nouvelle génération

**Nouveau basculement des vues**: les vues ci-dessous sont désormais disponibles dans l’expérience de nouvelle génération :

* [Affichage des détails du courrier électronique](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Mode Liste des emails](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automatisation de l’expérience {#experience-automation}

* **Exclusions des règles de validation des champs de formulaire globales**: excluez des formulaires spécifiques des règles de validation de formulaire globales de sorte que les centres d’abonnement et autres processus métier critiques puissent accepter toutes les valeurs.

* **Procédure de flux en libre-service**: développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes dynamiques. Les utilisateurs Marketo Engage et les partenaires peuvent exploiter cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes Trigger, Batch et Exécutable, contrairement aux webhooks, qui ne peuvent être utilisés que dans les campagnes Trigger.

* **Suivi des liens agnostiques du protocole Munchkin**: extension de la prise en charge du suivi des `tel` et `mailto` liens avec Munchkin pour suivre un ensemble étendu de comportements web.

* **Méthodes HTTP supplémentaires pour les webhooks**: spécifiez PUT, PATCH et DELETE en tant que types de requête pour interagir avec les services web.

## Sales Insight {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **Jeu d’autorisations Sales Insight dans Salesforce**: les administrateurs peuvent fournir l’accès à Sales Insight à un nombre limité de personnes au niveau de l’utilisateur plutôt qu’au niveau du profil par le biais du jeu d’autorisations Marketo App, qui fait partie du package Sales Insight Salesforce.

* **Mise à jour de la mosaïque Mes Marketo - Actions d’aperçu des ventes**: les administrateurs Marketo (et les utilisateurs qu’ils désignent) peuvent désormais accéder rapidement à leur instance d’actions Sales Insight par le biais d’une nouvelle mosaïque d’actions Sales Insight située sur la page My Marketo.

## Connect commercial {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Mise à jour de l’API Salesforce**: avec la version d’été 22 de Salesforce, les versions héritées des API 21 à 30 ne seront plus prises en charge par Salesforce. Avec cette version de Marketo Engage, toutes les demandes de Sales Connect utilisant des versions d’API héritées ont été mises à jour afin de rester dans une version prise en charge. Pour plus d’informations sur les plans de retraite de l’API Salesforce, cliquez sur [here](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## Améliorations des API {#api-enhancements}

* **Nouvelles fonctionnalités de filtrage pour l’API d’extraction de membres de programme en bloc**: filtrez par état d’adhésion au programme, mise à jour d’At, cadence ou contenu épuisé pour affiner le jeu de données extrait.

* **Amélioration de l’API d’extraction de membre de programme en bloc**: spécifiez jusqu’à 10 programmes pendant la création de la tâche pour améliorer le débit.

## Annonces {#announcements}

* **Obsolescence de Forms - Forms 1.0, point de fin de capture/enregistrement de piste et versions sans script des formulaires**: la prise en charge des ressources Forms 1.0 sera complètement supprimée de Marketo Engage d’ici octobre 2022. Toutes les ressources Forms 1.0 existantes cesseront de fonctionner. Les formulaires Marketo Engage requièrent du code JavaScript pour être chargés sur les landing pages et les sites web.

**_Webinaire sur la version du produit_**

[Webinaire de mise à jour des Marketo Engage de juin et août 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
