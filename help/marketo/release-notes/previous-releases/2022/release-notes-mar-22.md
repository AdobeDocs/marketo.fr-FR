---
description: Notes de mise à jour - Mars 2022 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Mars 2022
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Notes de mise à jour : mars 2022 {#release-notes-mar-22}

Les fonctionnalités suivantes sont incluses dans la version du 22 mars. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes commenceront à être publiées le **11 mars 2022**, avec un déploiement échelonné de chaque fonctionnalité au cours des semaines suivantes (sauf indication contraire).

## Orchestration cross-canal {#cross-channel-orchestration}

* **Dynamic Chat** : optimisez chaque opportunité de votre site web en ciblant à la fois les prospects et les comptes avec des conversations personnalisées proactives, attrayantes et 1:1. [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} permet aux utilisateurs Marketo Engage de commencer à utiliser le chat comme élément clé des expériences cross-canal intégrées pour les cas d’utilisation marketing et de vente B2B. Les fonctionnalités incluent : la possibilité de réserver des réunions directement dans le chat, le routage en direct, les modèles de démarrage, la création de conversations par glisser-déposer, etc. Dynamic Chat est inclus dans tous les packages de Marketo Engage et sera déployé sur tous les utilisateurs Marketo Engage cette année.

* **Amélioration du filtrage de l’activité des robots de messagerie** : à titre d’amélioration de la fonctionnalité de [ filtrage de l’activité des robots de messagerie](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} lancée précédemment, vous pouvez désormais souscrire à la journalisation des activités identifiées comme des robots. Vous pouvez ensuite filtrer et déclencher des actions en fonction d’activités identifiées comme étant exécutées par des robots.

## Expérience de nouvelle génération {#modern-ux}

* **Mise à jour de Screens dans l’expérience de nouvelle génération** : nous proposons des écrans supplémentaires actualisés dans l’expérience de nouvelle génération qui offrent une mise à jour de la conception et de la convivialité, accessibles par basculement :

   * Mode Liste des formulaires dans Design Studio (y compris les nouvelles actions en bloc)

* **Mise à jour du workflow du programme d’importation** : le workflow du programme d’importation est fourni dans l’expérience de nouvelle génération avec des améliorations de conception et de convivialité mises à jour. Il s’agit d’une modification automatique sans bouton de basculement.

* **Contrôle d’administration pour le commutateur d’activation/désactivation de l’expérience de nouvelle génération** : gérez le déploiement de l’expérience de nouvelle génération d’une manière qui fonctionne pour vos utilisateurs avec la possibilité pour les administrateurs de sélectionner les types d’utilisateurs qui peuvent accéder au bouton d’activation/désactivation.

## Automatisation de l’expérience {#experience-automation}

* **Étapes de flux en libre-service (Beta)** : développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes dynamiques. Les utilisateurs et les partenaires de Marketo peuvent exploiter cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes par lots et exécutables, contrairement aux webhooks, qui ne peuvent être utilisés que dans les campagnes de déclenchement.

* **Expiration des ressources** : maintenez le contrôle de vos ressources et campagnes sensibles au temps avec la possibilité de planifier leur désactivation automatique à une date et une heure spécifiées dans l’expérience utilisateur classique.

* **Remplacement de priorité de la campagne dynamique** : assurez-vous que le déclencheur de priorité élevée est exécuté le plus tôt possible avec la possibilité de remplacer le classement de priorité de la campagne standard. Le déclencheur de priorité moindre peut également être réduit en priorité afin de libérer des ressources de traitement pour d’autres tâches de priorité élevée.

## Améliorations des API {#api-enhancements}

* **Retour Désactiver l’état de suivi des ouvertures des emails** : permet la lecture de l’état de suivi des ouvertures des emails via l’API
* **Récupérer les lignes d’objet de contenu dynamique à partir d’un email** : permet aux marketeurs d’analyser les lignes d’objet dynamique dans les outils de BI
* **Champs personnalisés du membre de programme CRUD** : permet aux marketeurs de créer par programmation des champs personnalisés du membre de programme
* **Exportation d’objets personnalisés en bloc mise à jourAt Filter** : permet aux marketeurs de synchroniser par programmation les objets personnalisés
* **Exposer le paramètre Head Start pour les programmes de messagerie** : permet aux marketeurs de configurer les programmes de messagerie avec le démarrage anticipé via l’API
* **Mise à jour sélective de balises de programme** : permet aux marketeurs de pousser des mises à jour de balises sélectives sans envoyer toutes les balises en même temps.
* **Champ ActionResult d’extraction d’activité en masse** : permet aux marketeurs d’identifier les activités qui ont été ignorées ou qui ont échoué

**_Mise à jour tout au long du trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

## Bizible {#bizible}

![(star)](assets/yellow-star.png)

* **Modèles de BI** : Bizible fournit désormais des artefacts de rapports et des exemples de rapports téléchargeables de base pour Tableau et Power BI afin de permettre le développement rapide de rapports personnalisés adaptés à vos besoins spécifiques.

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **Limitation de la connexion par e-mail (GA)** : la limitation de la connexion par e-mail permet aux administrateurs de Sales Connect de configurer le taux d’envoi des e-mails lors de l’utilisation de Gmail ou Exchange comme canal de diffusion, de sorte que le taux auquel les e-mails sont remis au fournisseur de canal de diffusion ne dépasse pas les limites appliquées.

## Annonces {#announcements}

* **Dépréciation du Marketo Sky** : en mars, Marketo Sky ne sera plus disponible, car nous concentrons nos ressources sur la diffusion de l’expérience utilisateur de nouvelle génération. Afin de maintenir l’accès aux fonctionnalités exclusives à Marketo Sky aujourd’hui, nous incluons l’expiration des ressources et le remplacement de la priorité de campagne dynamique dans l’expérience Classic. [Cliquez ici](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) pour en savoir plus.

**_Webinaire sur la version du produit_**

[Webinaire de mise à jour des Marketo Engage de mars et mai 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
