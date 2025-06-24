---
unique-page-id: 37355826
description: Notes De Mise À Jour - Février 20 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Février 20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Notes De Mise À Jour : Février 20 {#release-notes-feb}

Les fonctionnalités suivantes sont incluses dans la version de février 2020. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile ( ![(étoile)](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo Engage pour en savoir plus.

**_Versions trimestrielles_** Les fonctionnalités suivantes ont été publiées le **21 février 2020**.

## Engagement Marketo de base {#core-marketo-engage}

* **[!DNL Microsoft Dynamics]action de flux « Modifier le propriétaire dans Microsoft »** : conservez le contrôle de vos données CRM [!DNL Microsoft Dynamics] tout en ayant la possibilité de modifier un prospect/propriétaire de contact directement à partir de Marketo Engage. Il s’agit d’une amélioration de notre fonctionnalité d’intégration CRM native.
* **API User Management** : automatisez la gestion des utilisateurs et des rôles par le biais de systèmes de gestion des identités et des organisations externes. Il s’agit d’une amélioration de notre fonctionnalité d’appels API.
* **API de schéma d’objet personnalisé** : gérez et configurez automatiquement des schémas d’objet personnalisés entre les instances de Marketo Engage pour garantir la cohérence des modèles de données au sein de vos outils de vente et de marketing. Avec cette API, vous pouvez définir et tester des objets personnalisés dans un sandbox ou un centre d’excellence et les configurer sur autant d’instances que nécessaire. Il s’agit d’une amélioration de notre fonctionnalité Appels d’API . Veuillez contacter votre représentant Marketo Engage pour savoir comment accéder à cette amélioration.
* **API de règles de redirection de page de destination** : automatisez la gestion des règles de redirection de page de destination. Il s’agit d’une amélioration de notre fonctionnalité d’appels API.
* **Mise en cache des descripteurs de formulaire** : nous réduisons le temps de chargement des formulaires incorporés et améliorons la stabilité globale de l’application en mettant en cache les formulaires en tant que ressources. Veuillez noter que les approbations de formulaires incorporés peuvent prendre jusqu&#39;à quatre minutes pour être reflétées sur le Web. Il s’agit d’une amélioration de notre fonctionnalité Pages de destination et Forms .

<br> 

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes font l’objet d’un cycle non trimestriel et seront publiées au cours des prochains mois.

## [!DNL Bizible] {#bizible}

![(étoile)](assets/yellow-star.png)

* **Segmentation basée sur les comptes** : analysez l’attribution au niveau du compte avec la possibilité de créer des segments et des filtres pour les tableaux Discover en fonction des attributs du compte. Utilisez ces segments pour analyser en profondeur les performances marketing basées sur votre compte.
* **Enregistrement des filtres** : enregistrez les filtres spécifiques aux tableaux de bord, propres à chaque utilisateur, pour analyser vos tableaux de bord rapidement et de manière cohérente.
* **Exporter vers PDF** : partagez de précieuses informations à l’échelle de votre organisation en exportant les tableaux de bord Bizible au format PDF.

## [!DNL Sales Connect] {#sales-connect}

* **Composer les mises à jour de fenêtre** : nous avons rationalisé le processus de sélection des modèles et d’envoi d’e-mails par le biais de [!DNL Sales Connect]. Utilisez la fenêtre Composer de notre client web et de Salesforce comme guichet unique pour les vendeurs. Vous pouvez ainsi enregistrer les catégories de modèles, planifier des e-mails, les envoyer en bloc et envoyer des e-mails avec suivi des affichages et des clics.
* **Mises à jour du centre de commande** : nous sommes en train de reconstruire le centre de commande [!DNL Sales Connect] pour fournir aux vendeurs insight tous leurs e-mails, appels et tâches lancés à partir d’[!DNL Sales Connect]. Ils peuvent également afficher des informations telles que l’engagement des e-mails et la délivrabilité depuis le centre de commande.

<br> 

## Annonces {#announcements}

* **Centre de succès Marketo Engage** : nous lançons le Centre de succès Marketo en février 2020. Le centre de succès est un centre d’aide intégré au produit qui vous permet de rechercher des documents produit et la communauté, de lancer des guides pratiques, d’accéder au contenu d’adoption tel que Marketo University et des vidéos de bonnes pratiques pour les pairs, et bien plus encore, et ce directement à partir de votre instance Marketo Engage. **Remarque** : cette fonctionnalité sera lancée en version Beta en Australie et en Nouvelle-Zélande et sera déployée en Amérique du Nord plus tard dans le trimestre.

## Obsolescence {#deprecations}

* **Paramètre « _method » de l’API de ressources** : après septembre 2020, les points d’entrée de l’API de ressources n’accepteront plus « _method » pour transmettre des paramètres de requête dans un corps POST afin de contourner les limites de longueur d’URI. Pour répondre aux requêtes qui nécessitaient ce paramètre, la limite d’URI pour les API de ressources passera de 6 Ko à 65 Ko, de sorte que les URI de requête longues puissent être envoyés.
* **Obsolescence de la prise en charge d’Internet Explorer** : à compter de la version de juillet du 31 juillet 2020, l’interface utilisateur de Marketo Engage ne sera plus prise en charge dans Internet Explorer.

**_Webinaire de mise à jour du produit_** [Rejoignez-nous](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) le 3 mars à 11 h 00 (heure de Paris) / 14 h 00 (heure de Paris) pour un webinaire en direct hébergé par notre équipe produit et découvrez en détail les fonctionnalités incluses dans cette version.
