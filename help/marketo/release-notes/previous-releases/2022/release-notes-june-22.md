---
description: Notes De Mise À Jour - Juin 2022 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Juin 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Notes De Mise À Jour : Juin 2022 {#release-notes-june-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 juin. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo Engage pour en savoir plus.

Les fonctionnalités suivantes seront publiées le **24 juin 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire).

## Environnement de données marketing {#marketing-data-environment}

* **Exposer les champs CreatedAt/UpdatedAt pour les objets personnalisés** : permet d’inspecter ces champs dans l’écran Détails de la personne pour obtenir des insight supplémentaires.

## Orchestration cross-canal {#cross-channel-orchestration}

* **Utilisation améliorée de Stream Designer pour les[!DNL Dynamic Chat]** : ajoutez des cartes directement à partir de la zone de travail de Stream Designer sans avoir à effectuer un glisser-déposer. L’interface [!DNL Dynamic Chat] a également été améliorée afin d’offrir une meilleure visibilité du contenu dans les cartes individuelles.

* **Règles avancées de routage des rendez-vous pour les[!DNL Dynamic Chat]** : [!DNL Dynamic Chat] offre davantage d’options de routage des rendez-vous ciblé. Spécifiez les rendez-vous d’agent qui doivent être acheminés en fonction des attributs de Marketo Engage, en vous assurant que les prospects sont acheminés vers les agents appropriés.

* **Rapports de boîte de dialogue avancés pour[!DNL Dynamic Chat]** : affichez plus en détail les performances de vos campagnes [!DNL Dynamic Chat] à l’aide de toutes nouvelles visualisations de données pour les mesures d’engagement et de conversion.

* **Désynchroniser les attributs Marketo Engage inutilisés pour les[!DNL Dynamic Chat]** : désynchronisez les attributs Marketo Engage de votre abonnement [!DNL Dynamic Chat] qui ne sont pas utilisés, ce qui vous permet de faciliter la propreté des données et de synchroniser d’autres attributs si nécessaire.

## Expérience nouvelle génération

**Nouveau bouton (bascule) des vues** : les vues ci-dessous sont désormais disponibles dans l’expérience de nouvelle génération :

* [Vue Détails de l’e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Vue Liste d’e-mails](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automatisation de l’expérience {#experience-automation}

* **Exclusions des règles de validation de champ de formulaire global** : excluez des formulaires spécifiques des règles de validation de formulaire global afin que les centres d’abonnements et d’autres workflows critiques pour l’entreprise puissent accepter toutes les valeurs.

* **Étapes de flux en libre-service** : développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes intelligentes. Les utilisateurs et partenaires de Marketo Engage peuvent tirer parti de cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes déclencheuses, par lots et exécutables, contrairement aux Webhooks, qui ne peuvent être utilisés que dans les campagnes déclencheuses.

* **Suivi des liens incompatibles avec le protocole Munchkin** : étendez la prise en charge du suivi des liens `tel` et `mailto` avec Munchkin pour suivre l’ensemble étendu des comportements web.

* **Méthodes HTTP supplémentaires pour les Webhooks** : spécifiez PUT, PATCH et DELETE comme types de requête pour interagir avec les services web.

## [!DNL Sales Insight] {#sales-insight}

![(étoile)](assets/yellow-star.png)

* Jeu d’autorisations **[!DNL Sales Insight]dans[!DNL Salesforce]** : les administrateurs peuvent fournir un accès [!DNL Sales Insight] à un ensemble limité de personnes au niveau de l’utilisateur plutôt qu’au niveau du profil via le jeu d’autorisations de l’application Marketo, qui fait partie du package d’[!DNL Salesforce] [!DNL Sales Insight].

* **My Marketo Tile Update - [!DNL Sales Insight] Actions** : les administrateurs Marketo (et les utilisateurs qu’ils désignent) peuvent désormais accéder rapidement à leur instance [!DNL Sales Insight] Actions via une nouvelle mosaïque [!DNL Sales Insight] Actions située sur la page My Marketo.

## [!DNL Sales Connect] {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **[!DNL Salesforce]mise à jour de l’API** : avec la version [!DNL Salesforce] de l’été 2022, les anciennes versions 21 à 30 de l’API ne seront plus prises en charge par [!DNL Salesforce]. Avec cette version de Marketo Engage, toutes les requêtes [!DNL Sales Connect] utilisant des versions d’API héritées ont été mises à jour afin de rester dans une version prise en charge. Pour plus d&#39;informations sur les plans de retraite des API [!DNL Salesforce], cliquez [ici](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## Améliorations de l’API {#api-enhancements}

* **Nouvelles fonctionnalités de filtrage pour l’API d’extraction de membre de programme en bloc** : filtrez par statut d’appartenance au programme, updatedAt, cadence ou contenu épuisé pour affiner le jeu de données extrait.

* **Amélioration de l’API d’extraction des membres de programme en bloc** : spécifiez jusqu’à 10 programmes lors de la création de tâche pour améliorer le débit.

## Annonces {#announcements}

* **Obsolescence de Forms : Forms 1.0, point d’entrée de capture/enregistrement de prospect et versions de formulaires sans script** : la prise en charge des ressources Forms 1.0 sera complètement supprimée de Marketo Engage d’ici octobre 2022. Toutes les ressources Forms 1.0 existantes cesseront de fonctionner. Les formulaires Marketo Engage devront être chargés sur des pages de destination et des sites web sous JavaScript.

**_Webinaire de mise à jour du produit_**

[Webinaire de mise à jour de Marketo Engage juin et août 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
