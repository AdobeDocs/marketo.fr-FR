---
description: Notes De Mise À Jour - Mars 2022 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Mars 2022
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 4%

---

# Notes de mise à jour : mars 2022 {#release-notes-mar-22}

Les fonctionnalités suivantes sont incluses dans la version de mars 2022. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **11 mars 2022**, avec un déploiement échelonné de chaque fonctionnalité au cours des semaines suivantes (sauf indication contraire).

## Orchestration cross-canal {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]** : maximisez chaque opportunité sur votre site web en ciblant les prospects et les comptes avec des conversations proactives, attrayantes et 1:1 personnalisées. [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} permet aux utilisateurs de Marketo Engage de commencer à utiliser le chat comme élément clé des expériences cross-canal intégrées pour les cas d’utilisation de marketing et de ventes B2B. Les fonctionnalités incluent : la possibilité de réserver des réunions directement dans le chat, le routage des prospects, les modèles de démarrage, la création de conversations par glisser-déposer, et bien plus encore. Dynamic Chat est inclus dans tous les packages Marketo Engage et sera déployé auprès de tous les utilisateurs Marketo Engage cette année.

* **Amélioration du filtrage des activités de robots d’e-mail** : en complément de la fonctionnalité [Filtrage des activités de robots d’e-mail](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} publiée précédemment, vous pouvez désormais vous inscrire aux activités de journalisation identifiées comme des robots. Vous pouvez ensuite filtrer et déclencher des actions en fonction des activités identifiées comme étant exécutées par des robots.

## Expérience nouvelle génération {#modern-ux}

* **Mise à jour de Screens dans l’expérience de nouvelle génération** : nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour et accessibles via le bouton bascule :

   * Vue Liste des formulaires dans [!UICONTROL Design Studio] (y compris les nouvelles actions en masse)

* **Mise à jour du workflow d’importation du programme** : le workflow d’importation du programme est fourni dans l’expérience de nouvelle génération avec une conception et des améliorations de convivialité mises à jour. Il s’agira d’une modification automatique sans commutateur.

* **Contrôle d’administration pour le commutateur de basculement d’expérience de nouvelle génération** : gérez le déploiement de l’expérience de nouvelle génération d’une manière qui fonctionne pour vos utilisateurs et qui permet aux administrateurs de sélectionner les types d’utilisateurs pouvant accéder au commutateur de basculement.

## Automatisation de l’expérience {#experience-automation}

* **Étapes de flux en libre-service (Beta)** : développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes intelligentes. Les utilisateurs et partenaires de Marketo peuvent tirer parti de cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes par lots et exécutables, contrairement aux webhooks, qui ne peuvent être utilisés que dans les campagnes de déclenchement.

* **Expiration des ressources** : contrôlez vos ressources et campagnes sensibles au facteur temps et planifiez leur désactivation automatique à une date et une heure spécifiées dans l’expérience utilisateur classique.

* **Remplacement de priorité de campagne intelligente** : assurez-vous que les campagnes intelligentes de déclenchement de priorité élevée s’exécutent dès que possible avec la possibilité de remplacer le classement de priorité de campagne standard. Les campagnes intelligentes à déclenchement de priorité inférieure peuvent également être réduites en priorité afin de libérer des ressources de traitement pour d’autres tâches de priorité élevée.

## Améliorations de l’API {#api-enhancements}

* **Renvoyer Désactiver le statut du suivi des ouvertures des e-mails** : permet la lecture du statut de suivi des ouvertures des e-mails via l’API
* **Récupérer les lignes d’objet de contenu dynamique de l’e-mail** : permet aux spécialistes marketing d’analyser les lignes d’objet dynamiques dans les outils de BI
* **CRUD des champs personnalisés des membres de programme** : permet aux spécialistes marketing de créer par programmation des champs personnalisés des membres de programme
* **Exportation d’objets personnalisés en bloc mise à jourAu filtre** : permet aux spécialistes marketing de synchroniser les objets personnalisés par programmation
* **Exposer le paramètre Head Start pour les programmes de messagerie électronique** : permet aux spécialistes du marketing de configurer des programmes de messagerie avec une avance via l’API
* **Mise à jour sélective des balises de programme** : permet aux marketeurs de pousser les mises à jour sélectives des balises sans pousser toutes les balises en même temps
* **Champ ActionResult de l’extraction d’activité en masse** : permet aux spécialistes marketing d’identifier les activités qui ont été ignorées ou ayant échoué

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes font l’objet d’un cycle non trimestriel et seront publiées au cours des prochains mois.

## [!DNL Bizible] {#bizible}

![(étoile)](assets/yellow-star.png)

* **Modèles BI** : [!DNL Bizible] fournira désormais des artefacts de rapports de base téléchargeables et des exemples de rapports pour Tableau et Power BI afin de permettre le développement rapide de rapports personnalisés adaptés aux besoins spécifiques de votre entreprise.

## [!DNL Sales Connect] {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Ralentissement de la connexion aux e-mails (GA, Email Connection Throttling)** : le ralentissement de la connexion aux e-mails permet aux administrateurs [!DNL Sales Connect] de configurer le taux d’envoi des e-mails lors de l’utilisation de Gmail ou [!DNL Exchange] comme canal de diffusion, de sorte que le taux de transmission des e-mails au fournisseur de canal de diffusion ne dépasse pas les limites appliquées.

## Annonces {#announcements}

* **Obsolescence de Marketo Sky** : en mars, Marketo Sky ne sera plus disponible, car nous concentrons nos ressources sur la diffusion de l’expérience utilisateur de nouvelle génération. Dans un effort de conserver l’accès à une fonctionnalité exclusive à Marketo Sky aujourd’hui, nous ajoutons l’expiration des ressources et le remplacement de priorité de campagne intelligente à l’expérience classique. [Cliquez ici](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) pour en savoir plus.

**_Webinaire de mise à jour du produit_**

[Webinaire de mise à jour de Marketo Engage de mars et mai 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
