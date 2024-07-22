---
unique-page-id: 37355826
description: Notes de mise à jour - Février 20 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Février 2020
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

# Notes de mise à jour : 20 février {#release-notes-feb}

Les fonctionnalités suivantes sont incluses dans la version du 20 février. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile ( ![(star)](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_** Les fonctionnalités suivantes ont été publiées le **21 février 2020**.

## Engagement Marketo de base {#core-marketo-engage}

* **Action de flux Microsoft Dynamics &quot;Changer de propriétaire dans Microsoft&quot;** : maintenez le contrôle de vos données Microsoft Dynamics CRM avec la possibilité de modifier un propriétaire de prospect/contact directement à partir du Marketo Engage. Il s’agit d’une amélioration de notre fonctionnalité d’intégration CRM native.
* **API de gestion des utilisateurs** : automatisez la gestion des utilisateurs et des rôles par le biais de systèmes de gestion des identités et des organisations externes. Il s’agit d’une amélioration de notre fonctionnalité d’appels API.
* **API de schéma d’objet personnalisé** : gérez et configurez automatiquement les schémas d’objet personnalisé entre les instances dans Marketo Engage afin de préserver la cohérence des modèles de données entre vos outils de vente et de marketing. Grâce à cette API, vous pouvez définir et tester des objets personnalisés dans un environnement de test ou un centre d’excellence et configurer autant d’instances que nécessaire. Il s’agit d’une amélioration de notre fonctionnalité d’appels API. Veuillez contacter votre représentant Marketo Engage pour savoir comment accéder à cette amélioration.
* **API de règles de redirection de page d’entrée** : automatisez la gestion des règles de redirection de page d’entrée. Il s’agit d’une amélioration de notre fonctionnalité d’appels API.
* **Mise en cache des descripteurs de formulaire** : nous réduisons le temps de chargement des formulaires incorporés et améliorons la stabilité globale de l’application en mettant en cache les formulaires en tant que ressources. Veuillez noter que les approbations effectuées sur les formulaires incorporés peuvent prendre jusqu’à quatre minutes pour être reflétées sur le Web. Il s’agit d’une amélioration de la fonctionnalité Pages d’entrée et Forms .

<br> 

**_Mise à jour tout au long du trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

## Bizible {#bizible}

![(star)](assets/yellow-star.png)

* **Segmentation basée sur un compte** : analysez l’attribution au niveau du compte avec la possibilité de créer des segments et des filtres pour les panoramas Discover en fonction des attributs du compte. Utilisez ces segments pour analyser en détail les performances marketing basées sur les comptes.
* **Enregistrement des filtres** : enregistrez des filtres spécifiques à un tableau de bord uniques à chaque utilisateur pour analyser rapidement et de manière cohérente vos tableaux de bord.
* **Exporter vers le PDF** : partagez des informations précieuses dans votre organisation en exportant les tableaux de bord Bizible en tant que PDF.

## Sales Connect {#sales-connect}

* **Composer les mises à jour de la fenêtre** : nous avons rationalisé le processus de sélection des modèles et d’envoi d’emails via Sales Connect. Utilisez la fenêtre Composer de notre client web et de Salesforce comme guichet unique pour les vendeurs, avec la possibilité d’enregistrer des catégories de modèles, de planifier des emails, d’envoyer des emails en masse et d’envoyer des emails avec un suivi des affichages et des clics.
* **Mises à jour du centre de commandes** : nous sommes en train de reconstruire le centre de commandes de Sales Connect afin de fournir aux vendeurs des informations sur tous leurs emails, appels et tâches lancés à partir de Sales Connect. Ils peuvent également afficher des informations telles que l’engagement et la délivrabilité des emails depuis le centre de commandes.

<br> 

## Annonces {#announcements}

* **Centre de succès des Marketo Engage** : nous lançons le Centre de succès Marketo en février 2020. Le centre de succès est un centre d’aide intégré qui vous permet de rechercher des documents produit et la communauté, de lancer des guides pratiques, d’accéder au contenu d’adoption tel que Marketo University et des vidéos de bonnes pratiques, etc., directement depuis votre instance de Marketo Engage. **Remarque** : Cette fonctionnalité sera lancée en version bêta en ANZ et sera déployée en Amérique du Nord plus tard dans le trimestre.

## Obsolescence {#deprecations}

* **Paramètre de l’API de ressource &quot;_method&quot;** : après septembre 2020, les points de fin de l’API de ressource n’accepteront plus &quot;_method&quot; pour transmettre les paramètres de requête dans un corps de POST afin de contourner les limitations de longueur d’URI. Pour répondre aux demandes qui nécessitaient ce paramètre, la limite d’URI pour les API de ressources sera augmentée de 6KiB à 65KiB, de sorte que les URI de demande longue puissent être envoyés.
* **Abandon de la prise en charge d’Internet Explorer** : à compter de notre version du 31 juillet 2020, l’interface utilisateur du Marketo Engage ne sera plus prise en charge sur Internet Explorer.

**__** [Rejoignez-nous](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) le 3 mars à 11h00 PT/14 h ET pour un webinaire en direct hébergé par notre équipe produit et découvrez les fonctionnalités incluses dans cette version.
