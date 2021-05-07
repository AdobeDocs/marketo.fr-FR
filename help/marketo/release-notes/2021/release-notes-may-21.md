---
description: Notes de mise à jour - Mai 2021 - Marketo Docs - Documentation du produit
title: Notes de mise à jour - Mai 2021
translation-type: tm+mt
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '1510'
ht-degree: 0%

---

# Notes de mise à jour : Mai 2021 {#release-notes-may-21}

Les fonctionnalités suivantes sont incluses dans la version du 21 mai. Consultez votre édition Marketo pour connaître la disponibilité des fonctionnalités.

>[!AVAILABILITY]
>
>Les fonctions signalées par une étoile ![](assets/star.png) sont des modules complémentaires payants. Veuillez contacter votre représentant Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **7 mai 2021**.

>[!NOTE]
>
>Ces trois fonctionnalités seront disponibles d&#39;ici le mardi 11 mai au soir :

* **Listes intelligentes du compte**
* **Exécuter les étapes de flux Campaign**
* **Filtrage de l&#39;Activité des robots de messagerie électronique**

## Expériences basées sur un compte {#Account-based-eaperiences}

* **Listes intelligentes du compte (disponibilité générale)** ![](assets/star.png) : Identifiez et qualifiez dynamiquement les comptes dotés des attributs de compte et de personne souhaités à la cible dans les campagnes marketing inter-canaux et envoyez des alertes opportunes aux ventes pour conclure plus rapidement les offres. Cette nouvelle fonctionnalité permet une automatisation robuste des stratégies marketing basées sur les comptes. Les Listes intelligentes de compte sont disponibles pour les clients disposant de la gestion de compte de Cible et qui bénéficient de la prochaine génération d’utilisateurs.

## Expérience utilisateur de nouvelle génération {#next-generation-user-experience}

Grâce à la prévisualisation de recherche globale, les marketeurs peuvent rapidement déterminer où se trouve une ressource partagée dans leur instance. Les onglets du navigateur affichent l’emplacement permettant d’améliorer la navigation dans les Activités marketing ou dans Design Studio. L&#39;arborescence et les filtres de recherche globaux vous aident à affiner vos critères de recherche. La fonctionnalité de glisser-déposer dans l’arborescence a été rétablie, ce qui vous permet de déplacer rapidement et efficacement les dossiers et les fichiers dans les principales zones de l’application. Les icônes récemment mises à jour (conformes aux normes d’accessibilité de l’Adobe) et les badges d’état permettent aux spécialistes du marketing de distinguer rapidement et facilement les dossiers et les fichiers dans l’arborescence et d’identifier l’état des programmes et des ressources.

## Automatisation de l’expérience {#experience-automation}

* **Exécuter les étapes** de flux Campaign : Rationalisez les workflows de création de campagne et améliorez les performances de la campagne grâce à une nouvelle étape de flux pour les campagnes dynamiques. Créez et enregistrez des campagnes de modèles centralisées pour les tâches répétitives dans votre espace de travail, telles que la normalisation du code de pays, à appeler et exécuter à partir de n’importe quelle Campaign dynamique via la nouvelle étape de flux &quot;Exécuter Campaign&quot;. Les campagnes liées s’exécutent dans l’ordre indiqué et garantissent la tâche terminée avant de passer à l’étape de flux suivante. Modifiez rapidement le flux en une seule campagne centralisée afin de mettre à jour chaque Campaign intelligente qui l’utilise pour rationaliser les workflows de data Management, de score de piste et de routage.

## Orchestration de plusieurs Canaux {#cross-channel-orchestration}

* **Champs de données sensibles dans Forms** : Les informations d’identification personnelle du client Protect ne s’affichent pas dans les formulaires Marketo Engage d’Adobe en définissant les champs de données comme sensibles et en limitant la préremplissage des formulaires pour ces champs. Lorsqu’un visiteur vue un formulaire sur le landing page, les champs définis comme sensibles n’affichent aucune donnée préremplie.

* **Bloquer les envois** de formulaires de courrier indésirable : Protect votre base de données des Marketo Engage d&#39;Adobes à partir de données indésirables qui peuvent provoquer des alertes non valides pour les ventes, déclencher des retards de campagne et créer des activités indésirables. Le nouveau mécanisme de validation rejette les envois de formulaire non valides et arrête les attaques de robots. Vos données sont plus nettes et vos campagnes marketing s’exécutent comme prévu, ce qui réduit le risque d’envoi de pistes non qualifiées vers les ventes.

* **Avertissement** d&#39;approbation des Programmes électroniques : Empêchez l’envoi d’e-mails erronés lorsque de nouvelles modifications ont été apportées à un programme précédemment approuvé.  L’avertissement sert de garde lorsque le spécialiste du marketing applique des modifications à un courrier électronique qui est déjà approuvé, mais oublie ensuite d’approuver les dernières modifications et envoie le courrier électronique à une grande audience sans contenu, contenu incorrect ou contenu ancien.

* **Action de flux unique dans la page** de détails de piste : Permet aux utilisateurs d’exécuter des actions de flux, telles que l’envoi de courriers électroniques, la modification du propriétaire de la piste ou toute autre action de campagne intelligente sur des pistes individuelles à partir de la page des détails de la piste à l’aide du menu d’actions de flux. Les marketeurs peuvent exécuter des actions de flux sur des pistes sans basculer vers la vue de grille de la base de données de pistes.

* **Filtrage de l&#39;Activité** des robots de messagerie : Empêchez les alertes de vente involontaires et les rapports électroniques inexacts grâce à la nouvelle fonctionnalité de filtrage des activités des robots de messagerie. Identifiez et filtrez les ouvertures et les clics qui peuvent être associés à des robots de messagerie qui inspectent les liens menant à de faux déclencheurs et à des alertes de vente, ou à un rapports incorrect.

## Améliorations de l&#39;API {#api-enhancements}

Plusieurs mises à jour critiques des API en bloc et pistes, notamment la possibilité d&#39;exporter des données d&#39;objet personnalisé en bloc, d&#39;associer la société au plomb en bloc, la possibilité de filtrer l&#39;extraction d&#39;activité en bloc en fonction d&#39;un attribut Principal et la possibilité de créer et de mettre à jour l&#39;adhésion au programme.

* **Programmes** de Événement d&#39;imbrication : Dans Adobe Marketo Engage, vous pouvez créer, cloner ou déplacer des programmes de événement sous d&#39;autres types de programme. Cette fonctionnalité est désormais autorisée dans l’API des ressources.

* **Amélioration de l&#39;API** de Programme de suppression : Permet aux applications intégrées de supprimer des programmes contenant d’autres types de ressources, sans exiger des utilisateurs qu’ils le fassent manuellement à partir de l’Adobe Marketo Engage.

* **Appartenance** au programme : Les marketeurs peuvent requête tous les enregistrements de membres de programme pour un programme sélectionné selon différents critères, tels que l’état du membre de programme. Partagez ces informations avec une application externe, un outil de veille stratégique ou Adobe Experience Cloud afin d’améliorer la segmentation et de créer un engagement plus ciblé.

* **Extraction** d&#39;objet personnalisé en bloc : L&#39;exportation de données en bloc complète les capacités d&#39;importation dont disposent déjà les analystes de données dans les Marketo Engage d&#39;Adobe. Désormais, ils peuvent extraire en bloc les données stockées dans les objets personnalisés du Marketo Engage de premier niveau, les charger dans une autre application, dans un autre entrepôt de données ou dans un autre outil BI (Business Intelligence) afin de mieux comprendre les données de l’instance de Marketo Engage d’Adobe.  Le déplacement des données en vrac d’objets personnalisés est bidirectionnel et peut être planifié à un moment opportun.

* **API** de métadonnées des champs personnalisés : Gagnez du temps en automatisant la création de champs personnalisés lors de la configuration des intégrations de vos Marketo Engage d’Adobe avec une application tierce. Cette automatisation s’adresse en particulier aux clients disposant de plusieurs instances de Marketo Engage d’Adobe qui sont désormais en mesure de rationaliser la création de champs personnalisés qui nécessitaient un travail manuel dans chaque instance. Rationalisez la création de champs personnalisés et gagnez du temps sur cette activité gourmande en ressources.

* **API** d&#39;extraction d&#39;Activité en bloc : Contrôlez la quantité et le type de données lors des extractions en vrac. Filtrez les points de données inutiles et contrôlez le nombre d&#39;appels d&#39;API nécessaires pour extraire les données d&#39;activité en bloc.  Par exemple, sélectionnez des courriers électroniques ouverts, visitez une page Web ou modifiez le score de piste et laissez derrière vous d’autres changements de valeur que vous ne souhaitez pas analyser. Rationalisez le processus afin de réduire le nombre d’appels d’API et le nettoyage des données.

* **API** de piste : Identifiez les pistes dans les Marketo Engage d&#39;Adobe auxquelles l&#39;ECID d&#39;Adobe (ID d&#39;Experience Cloud) est associé.  Les clients Marketo Engage d&#39;Adobe peuvent créer une liste de pistes à partir d&#39;une campagne sélectionnée et utiliser les ECID (ID d&#39;Experience Cloud) pour créer un rapports dans Adobe Analytics pour cette liste spécifique. L&#39;intégration entre le Marketo Engage d&#39;Adobe et le Adobe Experience Cloud offre des possibilités illimitées de segmentation, de ciblage et de rapports.

* **API** d&#39;importation de piste en vrac : Contrôler l&#39;importation en vrac de plomb et les ressources nécessaires. Cette amélioration crée une association entre le prospect et la société pendant le processus d&#39;importation de piste en vrac. Augmentez l&#39;efficacité et l&#39;utilisation des données et diminuez l&#39;utilisation en cas d&#39;appel d&#39;API.

* **Intégration basée sur l&#39;API Web pour les clients** Microsoft Dynamics Online : MS Dynamics Web API a été introduit avec le protocole REST de la version 8.0 et implémente OData (Open Data Protocol) v4. OData est une norme de l&#39;OASIS (Organisation pour l&#39;avancement des normes d&#39;information structurée) pour la construction et la consommation de services RESTful sur des données riches. Les clients Marketo Engage d&#39;Adobes qui nécessitent une intégration à Microsoft Dynamics à l&#39;aide de cette méthode sont actuellement migrés vers une connexion basée sur l&#39;API Web à partir de SOAP (Simple Object Access Protocol).

## Environnement de données marketing {#marketing-data-environment}

* **Exportation** XLSX : Nous avons mis à niveau les capacités d&#39;exportation dans tout le produit pour prendre en charge XLSX au lieu de XLS. Cela signifie que partout où l’exportation XLS est actuellement prise en charge dans le produit, cette option sera remplacée par une option d’exportation vers XLSX. Cette modification aura une incidence sur les noms de fichier pour toutes les exportations Excel de rapports et d&#39;autres données provenant de l&#39;Adobe Marketo Engage.

* **Rechercher par ID** de piste : Accédez rapidement à la recherche des enregistrements de piste par ID de piste Marketo Engage d&#39;Adobe dans la base de données de piste ou la liste statique. Dans la fenêtre Recherche rapide, tapez simplement `[id]` avec le numéro correspondant, puis les informations de piste s&#39;affichent. Les utilisateurs peuvent rapidement consulter les détails des pistes, des sociétés ou des opportunités.

## Bizible {#bizible}

![](assets/star.png)

* **Intégration à LinkedIn Lead Gen Forms (bêta)** : Bénéficiez d&#39;une grande visibilité sur vos dépenses de canal LinkedIn et sur le retour sur investissement grâce à la solution d&#39;attribution de prime lisible. Grâce à la toute dernière intégration avec le Lead Gen Forms de LinkedIn, Bizible permet de mieux comprendre les formulaires qui ont été envoyés sur la plate-forme LinkedIn. Ces remplissages de formulaires sont comparés aux prospects de votre gestion de la relation client (Customer Relationship Management) ou instance de Marketo Engage d’Adobe afin qu’ils puissent être attribués et suivis par vos autres engagements marketing.

## Annonces {#announcements}

* **Plateformes** de commutation des documents produit Marketo : Nous sommes heureux d’annoncer que les Docs produit Marketo se joindront au Adobe Experience League le vendredi 7 mai. Vous pourrez toujours utiliser l’URL : docs.marketo.com et si vous avez des articles existants mis en signet, vous serez redirigé. Tous les produits actuels seront disponibles sur la nouvelle plate-forme et des améliorations sont prévues pour la fin de l&#39;année.

* **Administration des utilisateurs rationalisée et authentification unique optimisée par le système** d&#39;identité des Adobes : À partir de juillet 2021, les nouveaux clients Marketo Engage d’Adobe seront intégrés à l’aide des identifiants d’utilisateur d’Adobe. La migration des clients actuels vers le système d&#39;identité intégré n&#39;aura lieu qu&#39;à la mi-2022 et aucune action de la part des clients n&#39;est requise jusqu&#39;à nouvel ordre. L&#39;authentification unique permet aux administrateurs informatiques et de sécurité de gérer plusieurs instances de produit Marketo Engage d&#39;Adobe avec d&#39;autres solutions Experience Cloud et de configurer l&#39;authentification unique (organisation Shared Services) via une console commune. Les administrateurs peuvent facilement gérer les groupes d’utilisateurs et les droits d’utilisateur par l’intermédiaire d’un Admin Console commun.
