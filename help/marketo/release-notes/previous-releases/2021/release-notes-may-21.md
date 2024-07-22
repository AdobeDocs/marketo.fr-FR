---
description: Notes de mise à jour - Mai 2021 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Mai 2021
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1450'
ht-degree: 0%

---

# Notes de mise à jour : mai 2021 {#release-notes-may-21}

Les fonctionnalités suivantes sont incluses dans la version du 21 mai. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **7 mai 2021**.

## Expériences basées sur un compte {#Account-based-eaperiences}

* **Listes dynamiques de compte (disponibilité générale)** ![](assets/yellow-star.png) : identifiez et qualifiez de manière dynamique les comptes avec les attributs de compte et de personne à cibler dans les campagnes marketing cross-canal et envoyez des alertes opportunes aux ventes pour conclure plus rapidement les offres. Cette nouvelle fonctionnalité permet une automatisation robuste des stratégies marketing basées sur les comptes. Les listes dynamiques de compte sont disponibles pour les clients disposant de la gestion de compte Target qui bénéficient de la nouvelle génération d’utilisateurs.

## Expérience utilisateur de nouvelle génération {#next-generation-user-experience}

Avec l’aperçu de la recherche globale, les marketeurs peuvent rapidement voir où se trouve une ressource partagée dans leur instance. Les onglets du navigateur affichent l’emplacement pour améliorer la navigation dans les activités marketing ou dans Design Studio. D’autres filtres de recherche globale et arborescente permettent d’affiner vos critères de recherche. La fonctionnalité de glisser-déposer dans l’arborescence a été rétablie, ce qui vous permet de déplacer des dossiers et des ressources rapidement et efficacement dans les zones principales de l’application. Les icônes nouvellement mises à jour (qui répondent aux normes d’accessibilité d’Adobe) et les badges d’état permettent aux marketeurs de distinguer rapidement et facilement les dossiers et les ressources dans l’arborescence et d’identifier l’état des programmes et des ressources.

## Automatisation de l’expérience {#experience-automation}

* **Exécuter les étapes de flux de campagne** : simplifiez les workflows de création de campagne et améliorez les performances des campagnes grâce à une nouvelle étape de flux pour les campagnes dynamiques. Créez et enregistrez des campagnes modèles centralisées pour les tâches répétitives dans votre espace de travail, telles que la normalisation des codes de pays, à appeler et exécuter à partir de n’importe quelle campagne dynamique via la nouvelle étape de flux &quot;Exécuter la campagne&quot;. Les campagnes liées s’exécutent dans l’ordre indiqué et assurent la fin de la tâche avant de passer à l’étape de flux suivante. Modifiez rapidement le flux en une seule campagne centralisée pour mettre à jour chaque campagne dynamique qui l’utilise afin de rationaliser la gestion des données, la notation des prospects et les workflows de routage.

## Orchestration cross-canal {#cross-channel-orchestration}

* **Champs de données sensibles dans Forms** : les informations d’identification personnelle du client Protect ne s’affichent pas dans les formulaires Adobe Marketo Engage en définissant les champs de données comme sensibles et en restreignant le préremplissage des formulaires pour ces champs. Lorsqu’un visiteur affiche un formulaire sur la landing page, les champs définis comme sensibles n’affichent aucune donnée préremplie.

* **Bloquer les envois de formulaires indésirables** : Protect votre base de données Adobe Marketo Engage à partir de données indésirables pouvant entraîner des alertes non valides pour les ventes, déclencher des retards de campagne et créer des activités indésirables. Le nouveau mécanisme de validation rejette les envois de formulaire non valides et arrête les attaques de robots. Vos données sont plus propres et vos campagnes marketing s’exécutent comme prévu, ce qui réduit le risque d’envoyer des prospects non qualifiés vers les ventes.

* **Avertissement d’approbation de programme de messagerie électronique** : empêchez l’envoi d’emails en erreur lorsque de nouvelles modifications ont été apportées à un programme précédemment approuvé.  L’avertissement sert de garde-fous lorsqu’un marketeur applique des modifications à un email déjà approuvé, mais oublie ensuite d’approuver les dernières modifications et envoie le courriel à une large audience sans contenu, sans contenu incorrect ou contenu obsolète.

* **Filtrer l’activité des robots de messagerie** : évitez les alertes de vente involontaires et les rapports par e-mail inexacts grâce à la nouvelle fonctionnalité de filtrage des activités de robots de messagerie. Identifiez et filtrez les ouvertures et les clics pouvant être associés à des robots de messagerie électronique, en examinant les liens qui génèrent de faux déclencheurs et des alertes de vente ou des rapports incorrects.

## Améliorations des API {#api-enhancements}

Plusieurs mises à jour critiques des API Bulk et Lead, notamment la possibilité d’exporter des données d’objet personnalisé en bloc, d’associer l’entreprise au prospect en bloc, de filtrer l’extraction d’activité en bloc en fonction d’un attribut principal et de créer et de mettre à jour l’appartenance au programme.

* **Nest Event Programmes** : dans Adobe Marketo Engage, vous pouvez créer, cloner ou déplacer des programmes d’événement sous d’autres types de programmes. Cette fonctionnalité est désormais autorisée dans l’API Assets.

* **API de programme de suppression améliorée** : permet aux applications intégrées de supprimer des programmes contenant des types de ressources supplémentaires, sans que les utilisateurs aient à le faire manuellement à partir de Adobe Marketo Engage.

* **Adhésion au programme** : les marketeurs peuvent interroger tous les enregistrements de membres du programme pour un programme sélectionné selon différents critères, tels que le statut du membre du programme. Partagez ces informations avec une application externe, un outil de Business Intelligence ou Adobe Experience Cloud afin d’améliorer la segmentation et de créer un engagement plus ciblé.

* **Extraction d’objets personnalisés en bloc** : l’exportation de données en bloc complète les fonctionnalités d’importation dont bénéficient déjà les analystes de données dans Adobe Marketo Engage. Désormais, ils peuvent extraire en bloc des données stockées dans des objets personnalisés Adobe Marketo Engage de premier niveau, puis les charger dans une autre application, un autre entrepôt de données ou un autre outil de BI (Business Intelligence) pour obtenir de meilleures informations sur les données de l’instance Adobe Marketo Engage.  Le déplacement massif de données d’objet personnalisé est bidirectionnel et peut être planifié à un moment opportun.

* **API de métadonnées de champs personnalisés** : gagnez du temps en automatisant la création de champs personnalisés lors de la configuration de vos intégrations Adobe Marketo Engage avec une application tierce. Cette automatisation est particulièrement bénéfique pour les clients disposant de plusieurs instances Adobe Marketo Engage qui peuvent désormais rationaliser la création de champs personnalisés qui nécessitaient un travail manuel dans chaque instance. Rationalisez la création de champs personnalisés et gagnez du temps sur cette activité gourmande en ressources.

* **API d’extraction d’activité en bloc** : contrôlez la quantité et le type de données lors d’extractions en masse. Filtrez les points de données inutiles et contrôlez le nombre d’appels API nécessaires pour extraire en masse les données d’activité.  Par exemple, sélectionnez des emails ouverts, consultez une page web ou modifiez le score de piste et laissez derrière d’autres modifications de valeur que vous ne souhaitez pas analyser. Rationalisez le processus pour réduire le nombre d’appels API et de tâches de nettoyage des données.

* **API de piste** : identifiez les pistes dans Adobe Marketo Engage associées à un Adobe ECID (identifiant Experience Cloud).  Les clients Adobe Marketo Engage peuvent créer une liste de pistes à partir d’une campagne sélectionnée et utiliser les ECID (identifiant Experience Cloud) pour créer des rapports dans Adobe Analytics pour cette liste spécifique. L’intégration entre Adobe Marketo Engage et Adobe Experience Cloud offre un nombre illimité d’opportunités de segmentation, de ciblage et de création de rapports.

* **API d’importation de pistes en bloc** : contrôlez l’importation de pistes en bloc et les ressources nécessaires. Cette amélioration crée une association entre le prospect et l’entreprise lors du processus d’importation de prospect en bloc. Augmentez l’efficacité et l’utilisation des données et réduisez l’utilisation des appels API.

* **Intégration basée sur l’API web pour les clients en ligne Microsoft Dynamics** : l’API web MS Dynamics a été introduite avec le protocole REST version 8.0 et implémente OData (Open Data Protocol) v4. OData est une norme OASIS (Organisation pour l’avancement des normes d’information structurée) destinée à la création et à la consommation de services RESTful par rapport à des données riches. Les clients Adobe Marketo Engage qui nécessitent une intégration avec Microsoft Dynamics à l’aide de cette méthode sont actuellement migrés vers une connexion basée sur l’API Web à partir de SOAP (Simple Object Access Protocol).

## Environnement de données marketing {#marketing-data-environment}

* **Exportation XLSX** : nous avons mis à niveau les fonctionnalités d’exportation dans tout le produit pour prendre en charge XLSX au lieu de XLS. Cela signifie que partout dans le produit où l’exportation XLS est actuellement prise en charge, cette option sera remplacée par une option d’exportation vers XLSX à la place. Cette modification aura une incidence sur les noms de fichier pour toutes les exportations Excel des rapports et d’autres données provenant de Adobe Marketo Engage.

* **Recherche par identifiant de piste** : accédez rapidement à la recherche d’enregistrements de piste par identifiant de piste Adobe Marketo Engage dans la base de données de piste ou la liste statique. Dans la fenêtre Recherche rapide, il vous suffit de taper `[id]` avec le numéro correspondant pour afficher les informations de piste. Les utilisateurs peuvent rapidement consulter les détails des prospects, des entreprises ou des opportunités.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Intégration avec LinkedIn Lead Gen Forms (Beta)** : profitez d’une grande visibilité sur les dépenses et le retour sur investissement de vos canaux LinkedIn avec la solution d’attribution Premium Bizible. Grâce à la dernière intégration avec le Forms Lead Gen de LinkedIn, Bizible obtient des informations sur les formulaires qui ont été envoyés dans la plateforme LinkedIn. Ces remplissages de formulaires sont comparés aux prospects de votre instance CRM (Customer Relationship Management) ou Adobe Marketo Engage afin qu’ils soient éligibles à l’attribution et puissent être suivis par rapport à vos autres engagements marketing.

## Annonces {#announcements}

* **Marketo Product Docs Swching Platforms** : nous sommes heureux d’annoncer que les Product Docs de Marketo ont rejoint Adobe Experience League à partir du vendredi 7 mai. Vous pourrez toujours utiliser l’URL : docs.marketo.com. Si des articles existants sont marqués, vous serez redirigé. Toutes les documents produit sont disponibles sur la nouvelle plateforme. Des améliorations sont prévues pour la fin de l’année.

* **Administration simplifiée des utilisateurs et authentification unique optimisée par Adobe Identity System** : à compter de juillet 2021, les nouveaux clients Adobe Marketo Engage seront intégrés à l’aide des informations d’identification d’utilisateur d’Adobe. La migration des clients actuels vers le système d’identité intégré n’aura lieu qu’à la mi-2022 et aucune action du client n’est requise jusqu’à nouvel ordre. L’authentification unique permet aux administrateurs informatiques et de sécurité de gérer plusieurs instances de produit Adobe Marketo Engage, ainsi que d’autres solutions Experience Cloud, et de configurer l’authentification unique (organisation des services partagés) à l’aide d’une console commune. Les administrateurs peuvent facilement gérer les groupes d’utilisateurs et les droits des utilisateurs par le biais d’un Admin Console commun.

**_Webinaire sur la version du produit_**

[Webinaire de mise à jour du Marketo Engage de mai 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
