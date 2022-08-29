---
description: Notes de mise à jour - Mars 2022 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Mars 2022
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
source-git-commit: beafa230f067972119f1a0eb170b1339d20d3842
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 1%

---

# Notes de mise à jour : Mars 2022 {#release-notes-mar-22}

Les fonctionnalités suivantes sont incluses dans la version du 22 mars. Vérifiez la disponibilité de votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes commenceront à être publiées sur **11 mars 2022**, avec un déploiement échelonné de chaque fonctionnalité au cours des semaines suivantes (sauf indication contraire).

## Orchestration cross-canal {#cross-channel-orchestration}

* **Chat dynamique**: Optimisez chaque opportunité de votre site web en ciblant à la fois les pistes et les comptes à l’aide de conversations proactives, attrayantes et personnalisées 1:1. [Chat dynamique](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;} permet aux utilisateurs Marketo Engage de commencer à utiliser le chat comme un élément clé des expériences cross-canal intégrées pour les cas d’utilisation de marketing et de vente B2B. Les fonctionnalités incluent : la possibilité de réserver des réunions directement dans le chat, de diriger le routage, de lancer des modèles, de créer des conversations par glisser-déposer, etc. Dynamic Chat est inclus dans tous les packages de Marketo Engage et sera déployé par tous les utilisateurs Marketo Engage cette année.

* **Amélioration du filtrage de l’activité des robots de messagerie**: En tant qu’amélioration de la version précédente [Filtrage de l’activité des robots de messagerie](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md)fonction {target=&quot;_blank&quot;}, vous pouvez désormais souscrire à des activités de journalisation qui sont identifiées comme des robots. Vous pouvez ensuite filtrer et déclencher des actions en fonction d’activités identifiées comme étant exécutées par des robots.

## Expérience de nouvelle génération {#next-generation-experience}

* **Mise à jour d’Screens dans l’expérience de nouvelle génération**: Nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour, accessibles par le biais d’un bouton d’activation/désactivation :

   * Mode Liste des formulaires dans Design Studio (y compris les nouvelles actions en bloc)

* **Mise à jour du workflow d’import**: Le workflow du programme d’import est livré avec la nouvelle génération, avec des améliorations de conception et d’utilisation mises à jour. Il s’agit d’une modification automatique sans bouton de basculement.

* **Contrôle d’administration pour le commutateur de basculement de l’expérience de nouvelle génération**: Gérez le déploiement de l’expérience de nouvelle génération de manière à ce que les utilisateurs puissent sélectionner les types d’utilisateurs qui peuvent accéder au bouton d’activation/désactivation.

## Automatisation de l’expérience {#experience-automation}

* **Étapes de flux en libre-service (version bêta)**: Développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes dynamiques. Les utilisateurs et les partenaires de Marketo peuvent exploiter cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes par lots et exécutables, contrairement aux webhooks, qui ne peuvent être utilisés que dans les campagnes de déclenchement.

* **Expiration des ressources**: Contrôlez vos ressources et campagnes sensibles au temps en programmant leur désactivation automatique à une date et une heure spécifiées dans l’expérience utilisateur classique.

* **Remplacement de la priorité de la campagne dynamique**: Assurez-vous que le déclencheur de priorité élevée est exécuté le plus tôt possible avec la possibilité de remplacer le classement de priorité de campagne standard. Le déclencheur de priorité moindre peut également être réduit en priorité afin de libérer des ressources de traitement pour d’autres tâches de priorité élevée.

## Améliorations des API {#api-enhancements}

* **Retour Désactiver l’état de suivi des ouvertures des emails**: Permet la lecture de l’état de suivi des ouvertures des emails via l’API
* **Récupération des lignes d’objet de contenu dynamique à partir d’un courrier électronique**: Permet aux marketeurs d’analyser les objets dynamiques dans les outils de BI
* **CRUD des champs personnalisés des membres du programme**: Permet aux marketeurs de créer par programmation des champs personnalisés de membres de programme
* **Exportation d’objets personnalisés en bloc mise à jour au niveau du filtre**: Permet aux marketeurs de synchroniser par programmation les objets personnalisés
* **Exposer le paramètre Head Start pour les programmes de messagerie**: Permet aux marketeurs de configurer des programmes de messagerie avec un démarrage anticipé via l’API
* **Mise à jour sélective des balises de programme**: Permet aux marketeurs de pousser des mises à jour de balises sélectives sans envoyer toutes les balises en même temps.
* **Champ ActionResult d’extraction d’activité en bloc**: Permet aux marketeurs d’identifier les activités qui ont été ignorées ou qui ont échoué.

**_Sortie pendant tout le trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

## Bizible {#bizible}

![(étoile)](assets/yellow-star.png)

* **Modèles BI**: Bizible fournit désormais des artefacts de rapports et des exemples de rapports téléchargeables et de base pour Tableau et Power BI afin de permettre le développement rapide de rapports personnalisés adaptés à vos besoins spécifiques.

## SalesConnect {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Limitation de la connexion aux e-mails (GA)**: Le contrôle de connexion par e-mail permet aux administrateurs de Sales Connect de configurer le taux d’envoi des e-mails lors de l’utilisation de Gmail ou Exchange comme canal de diffusion, de sorte que le taux auquel les e-mails sont remis au fournisseur de canal de diffusion ne dépasse pas les limites appliquées.

## Annonces {#announcements}

* **Obsolescence du Marketo Sky**: En mars, Marketo Sky ne sera plus disponible, car nous concentrons nos ressources sur la diffusion de l’expérience utilisateur de nouvelle génération. Afin de maintenir l’accès aux fonctionnalités exclusives à Marketo Sky aujourd’hui, nous incluons l’expiration des ressources et le remplacement de la priorité de campagne dynamique dans l’expérience classique. [Cliquez ici](https://nation.marketo.com/t5/the-next-generation-experience/marketo-sky-deprecation-notice/ba-p/320115#M33) pour en savoir plus.

**_Webinaire sur la version du produit_**

[Webinaire de mise à jour des Marketo Engage de mars et mai 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target=&quot;_blank&quot;}
