---
description: Notes de mise à jour - Juin 2022 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Juin 2022
source-git-commit: 4bff61b90cbbe9466c23d9b003378eb72570f56c
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Notes de mise à jour : Juin 2022 {#release-notes-june-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 juin. Vérifiez la disponibilité de votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

Les fonctionnalités suivantes commenceront à être publiées sur **24 juin 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire).

## Environnement de données marketing {#marketing-data-environment}

* **Exposer les champs CreatedAt/UpdatedAt pour les objets personnalisés**: Permet d’examiner ces champs dans l’écran Détails de la personne afin d’obtenir des informations supplémentaires.

## Orchestration cross-canal {#cross-channel-orchestration}

* **Amélioration de l’utilisation du concepteur de flux pour Dynamic Chat**: Ajoutez des cartes directement à partir du canevas du Concepteur de flux sans avoir à les faire glisser. L’interface de messagerie dynamique a également été améliorée afin d’offrir une meilleure visibilité du contenu dans les cartes individuelles.

* **Règles de routage de rendez-vous avancées pour les conversations dynamiques**: Dynamic Chat offre d’autres options pour le routage de rendez-vous ciblé. Spécifiez les nominations d’agent à router en fonction des attributs du Marketo Engage, en veillant à ce que les prospects soient acheminés vers les agents appropriés.

* **Création de rapports de dialogue avancé pour la conversation dynamique**: Affichez plus en détail les performances de vos campagnes de messagerie dynamique à l’aide de toutes nouvelles visualisations de données pour les mesures d’engagement et de conversion.

* **Attributs de Marketo Engage non synchronisés pour Dynamic Chat**: Les attributs de Marketo Engage non synchronisés de votre abonnement Dynamic Chat qui ne sont pas utilisés vous aident à simplifier la propreté des données et permettent de synchroniser d’autres attributs si nécessaire.

## Expérience de nouvelle génération

**Nouveau basculement des vues**: Les vues ci-dessous sont désormais disponibles dans l’expérience de nouvelle génération :

* [Affichage des détails du courrier électronique](/help/marketo/product-docs/marketo-engage-next-generation-experience/toggle-switch.md#email-details-view){target=&quot;_blank&quot;}
* [Mode Liste des emails](/help/marketo/product-docs/marketo-engage-next-generation-experience/toggle-switch.md#email-list-view){target=&quot;_blank&quot;}

## Automatisation de l’expérience {#experience-automation}

* **Exclusions des règles de validation des champs de formulaire globales**: Exclure des formulaires spécifiques des règles de validation de formulaire globales de sorte que les centres d’abonnement et autres processus métier critiques puissent accepter toutes les valeurs.

* **Étapes de flux en libre-service**: Développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes dynamiques. Les utilisateurs Marketo Engage et les partenaires peuvent exploiter cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes Trigger, Batch et Exécutable, contrairement aux webhooks, qui ne peuvent être utilisés que dans les campagnes Trigger.

* **Suivi des liens agnostiques du protocole Munchkin**: Étendre la prise en charge du suivi des `tel` et `mailto` liens avec Munchkin pour suivre un ensemble étendu de comportements web.

* **Méthodes HTTP supplémentaires pour les webhooks**: Spécifiez PUT, PATCH et DELETE comme types de requête pour interagir avec les services web.

## Sales Insight {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **Jeu d’autorisations Sales Insight dans Salesforce**: Les administrateurs peuvent accorder l’accès à Sales Insight à un nombre limité de personnes au niveau de l’utilisateur plutôt qu’au niveau du profil par le biais du jeu d’autorisations Marketo App, qui fait partie du package Sales Insight Salesforce.

* **Mise à jour de la mosaïque Mes Marketo - Actions d’aperçu des ventes**: Les administrateurs Marketo (et les utilisateurs qu’ils désignent) peuvent désormais accéder rapidement à leur instance d’actions Sales Insight via une nouvelle mosaïque Sales Insight Actions (Actions Aperçu des ventes) située sur la page My Marketo.

## SalesConnect {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Mise à jour de l’API Salesforce**: Avec la version d’été 22 de Salesforce, les versions 21 à 30 héritées de l’API ne seront plus prises en charge par Salesforce. Avec cette version de Marketo Engage, toutes les demandes de Sales Connect utilisant des versions d’API héritées ont été mises à jour afin de rester dans une version prise en charge. Pour plus d’informations sur les plans de retraite de l’API Salesforce, cliquez sur [here](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target=&quot;_blank&quot;}.

## Améliorations des API {#api-enhancements}

* **Nouvelles fonctionnalités de filtrage pour l’API d’extraction de membres de programme en bloc**: Filtrez par statut d’adhésion au programme, mise à jour d’At, cadence ou contenu épuisé pour affiner le jeu de données extrait.

* **Amélioration de l’API d’extraction de membre de programme en bloc**: Spécifiez jusqu’à 10 programmes pendant la création de la tâche pour améliorer le débit.

## Annonces {#announcements}

* **Obsolescence de Forms - Forms 1.0, point de fin de capture/enregistrement de piste et versions sans script des formulaires**: La prise en charge des ressources Forms 1.0 sera complètement supprimée de Marketo Engage d’ici octobre 2022. Toutes les ressources Forms 1.0 existantes cesseront de fonctionner. Les formulaires Marketo Engage nécessitent JavaScript pour être chargés sur les landing pages et les sites web.

**_Webinaire sur la version du produit_**

Rejoignez-nous le 24 août 2022, à 9h00 PT / 12h00 ET pour une [webinaire en direct](https://engage.marketo.com/2022_June_August_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} hébergé par notre équipe produit où vous pouvez apprendre à utiliser toutes les dernières innovations de produit.