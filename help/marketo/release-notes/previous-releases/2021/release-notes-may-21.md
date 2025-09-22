---
description: Notes De Mise À Jour - Mai 2021 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Mai 2021
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 1%

---

# Notes de mise à jour : mai 2021 {#release-notes-may-21}

Les fonctionnalités suivantes sont incluses dans la version du 21 mai. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **7 mai 2021**.

## Expériences basées sur des comptes {#Account-based-eaperiences}

* **Listes dynamiques de compte (disponibilité générale)** ![](assets/yellow-star.png) : identifiez et qualifiez de manière dynamique les comptes avec les attributs de compte et de personne souhaités à cibler dans les campagnes marketing cross-canal et envoyez des alertes opportunes aux ventes pour conclure plus rapidement des affaires. Cette nouvelle fonctionnalité permet une automatisation robuste des stratégies marketing basées sur les comptes. Les listes dynamiques de comptes sont disponibles pour les clients disposant de la gestion de compte Target qui utilisent l’expérience utilisateur de nouvelle génération.

## Expérience utilisateur de nouvelle génération {#next-generation-user-experience}

Grâce à l’aperçu de la recherche globale, les marketeurs peuvent rapidement voir où se trouve une ressource partagée dans leur instance. Les onglets du navigateur affichent l’emplacement permettant d’améliorer la navigation dans [!UICONTROL Activités marketing] ou [!UICONTROL Design Studio]. Des filtres de recherche globaux et d’arborescence supplémentaires permettent d’affiner vos critères de recherche. La fonctionnalité de glisser-déposer dans l’arborescence a été rétablie, ce qui vous permet de déplacer rapidement et efficacement des dossiers et des ressources dans les zones principales de l’application. Les icônes nouvellement mises à jour (qui répondent aux normes d’accessibilité d’Adobe) et les badges d’état permettent aux spécialistes marketing de faire la distinction rapidement et facilement entre les dossiers et les ressources dans l’arborescence et d’identifier l’état des programmes et des ressources.

## Automatisation de l’expérience {#experience-automation}

* **Exécuter les étapes de flux de campagne** : rationalisez les workflows de création de campagne et améliorez les performances de la campagne grâce à une nouvelle étape de flux pour les campagnes intelligentes. Créez et enregistrez des campagnes modèles centralisées pour les tâches répétitives dans votre espace de travail, telles que la normalisation du code pays, à appeler et à exécuter à partir de toute campagne intelligente via la nouvelle étape de flux « Exécuter la campagne ». Les campagnes liées s’exécutent dans l’ordre indiqué et garantissent la réalisation de la tâche avant de passer à l’étape de flux suivante. Modifiez rapidement le flux dans une seule campagne centralisée afin de mettre à jour chaque campagne intelligente qui l’utilise pour rationaliser la gestion des données, la notation des prospects et les workflows de routage.

## Orchestration cross-canal {#cross-channel-orchestration}

* **Champs de données sensibles dans Forms** : protégez les informations d’identification personnelle (PII) du client de l’affichage dans les formulaires Adobe Marketo Engage en définissant les champs de données comme sensibles et en limitant le préremplissage de formulaire pour ces champs. Chaque fois qu’un visiteur consulte un formulaire sur la page de destination, les champs définis comme sensibles n’affichent aucune donnée préremplie.

* **Bloquer les envois de formulaires indésirables** : protégez votre base de données Adobe Marketo Engage des données indésirables qui peuvent entraîner des alertes non valides sur les ventes, déclencher des retards dans les campagnes et créer des activités indésirables. Le nouveau mécanisme de validation rejette les envois de formulaire non valides et arrête les attaques de robots. Vos données sont plus précises et vos campagnes marketing s&#39;exécutent comme prévu, ce qui réduit le risque d&#39;envoyer des prospects non qualifiés aux ventes.

* **Avertissement d’approbation du programme d’e-mail** : empêchez l’envoi d’e-mails erronés lorsque de nouvelles modifications ont été apportées à un programme précédemment approuvé.  Cet avertissement sert de mécanisme de sécurisation lorsqu’un spécialiste marketing applique des modifications à un e-mail qui est déjà approuvé, mais oublie ensuite d’approuver les dernières modifications et envoie l’e-mail à une audience importante sans contenu, avec un contenu incorrect ou un ancien contenu.

* **Filtrer l’activité des robots d’e-mail** : prévenez les alertes de ventes involontaires et les rapports d’e-mail inexacts grâce à la nouvelle fonctionnalité de filtrage d’activité des robots d’e-mail. Identifiez et filtrez les ouvertures et les clics qui peuvent être associés aux robots de messagerie qui inspectent les liens menant à de faux déclencheurs et à des alertes de ventes, ou à des rapports incorrects.

## Améliorations de l’API {#api-enhancements}

Plusieurs mises à jour critiques des API Bulk et Lead, notamment la possibilité d’exporter des données d’objet personnalisées en bloc, d’associer la société au lead en bloc, la possibilité de filtrer l’extraction d’activité en bloc en fonction d’un attribut principal et la possibilité de créer et de mettre à jour l’appartenance à un programme.

* **Imbriquer des programmes d’événement** : dans Adobe Marketo Engage, vous pouvez créer, cloner ou déplacer des programmes d’événement sous d’autres types de programmes. Cette fonctionnalité est désormais autorisée dans l’API Assets.

* **API Enhanced Delete Program** : permet aux applications intégrées de supprimer des programmes contenant des types de ressources supplémentaires, sans que les utilisateurs aient à le faire manuellement à partir de Adobe Marketo Engage.

* **Appartenance à un programme** : les marketeurs peuvent interroger tous les enregistrements des membres du programme pour un programme sélectionné en fonction de différents critères, tels que le statut de membre du programme. Partagez ces informations avec une application externe, un outil de Business Intelligence ou Adobe Experience Cloud afin d’améliorer la segmentation et de créer des engagements plus ciblés.

* **Extraction d’objet personnalisé en bloc** : l’exportation de données en bloc complète les fonctionnalités d’importation dont bénéficient déjà les analystes de données dans Adobe Marketo Engage. Désormais, ils peuvent extraire en bloc les données stockées dans les objets personnalisés Adobe Marketo Engage de premier niveau, charger ces données dans une autre application, un entrepôt de données ou un autre outil de BI (Business Intelligence) pour obtenir de meilleures informations sur les données de l’instance Adobe Marketo Engage.  Le mouvement des données en masse d’objets personnalisés est bidirectionnel et peut être planifié à un moment opportun.

* **API de métadonnées de champs personnalisés** : gagnez du temps en automatisant la création de champs personnalisés lors de la configuration de vos intégrations Adobe Marketo Engage avec une application tierce. Cette automatisation bénéficie tout particulièrement aux clients disposant de plusieurs instances Adobe Marketo Engage qui peuvent désormais rationaliser la création de champs personnalisés qui nécessitait auparavant un travail manuel dans chaque instance. Rationalisez la création de champs personnalisés et gagnez du temps sur cette activité gourmande en ressources.

* **API Bulk Activity Extract** : contrôlez la quantité et le type de données lors des extractions en bloc. Filtrez les points de données inutiles et contrôlez le nombre d’appels API nécessaires pour extraire les données d’activité en bloc.  Par exemple, sélectionnez ouvrir les e-mails, visiter une page web ou modifier le score du prospect et laisser derrière vous d’autres modifications de valeur que vous ne souhaitez pas analyser. Rationalisez le processus pour réduire le nombre d’appels API et le nettoyage des données.

* **API de lead** : identifier les leads dans Adobe Marketo Engage auxquels un ECID Adobe (ID Experience Cloud) est associé.  Les clients Adobe Marketo Engage peuvent créer une liste de prospects à partir d’une campagne sélectionnée et utiliser les ECID (Experience Cloud ID) pour créer des rapports dans Adobe Analytics pour cette liste spécifique. L’intégration entre Adobe Marketo Engage et Adobe Experience Cloud offre des possibilités illimitées de segmentation, de ciblage et de création de rapports.

* **API Bulk Lead Import** : contrôlez l’importation de leads en bloc et les ressources qu’elle nécessite. Cette amélioration crée une association entre le prospect et l’entreprise pendant le processus d’importation de prospect en bloc. Augmentation de l’efficacité et de l’utilisation des données et diminution de l’utilisation des appels API.

* **Intégration basée sur les API web pour les clients [!DNL Microsoft Dynamics Online]** : [!DNL MS Dynamics] API web a été introduite avec le protocole REST version 8.0 et implémente OData (Open Data Protocol) v4. OData est une norme de l’OASIS (Organization for the Advancement of Structured Information Standards) qui permet de créer et d’utiliser des services RESTful sur des données riches. Les clients Adobe Marketo Engage qui nécessitent une intégration à [!DNL Microsoft Dynamics] à l’aide de cette méthode sont actuellement migrés vers une connexion basée sur l’API Web à partir de SOAP (Simple Object Access Protocol).

## Environnement de données marketing {#marketing-data-environment}

* **Exportation XLSX** : nous avons mis à niveau les fonctionnalités d’exportation dans l’ensemble du produit afin de prendre en charge XLSX au lieu de XLS. Cela signifie que n’importe où dans le produit où l’exportation XLS est actuellement prise en charge, cette option sera remplacée par une option permettant d’exporter vers XLSX à la place. Cette modification affectera les noms de fichiers pour toutes les exportations Excel de rapports et d’autres données à partir de Adobe Marketo Engage.

* **Recherche par ID de lead** : accédez rapidement à la recherche d’enregistrements de lead par ID de lead Adobe Marketo Engage dans la base de données de lead ou la liste statique. Dans la fenêtre Recherche rapide, tapez simplement `[id]` avec le numéro correspondant, puis les informations sur le prospect s’affichent. Les utilisateurs peuvent rapidement consulter les détails du prospect, de l’entreprise ou de l’opportunité.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Intégration à [!DNL LinkedIn] Forms de génération de leads (Beta)** : bénéficiez d’une visibilité approfondie sur vos dépenses de canal [!DNL LinkedIn] et votre retour sur investissement avec la solution d’attribution Premium Bizible. Grâce à la dernière intégration avec Forms de génération de leads d’[!DNL LinkedIn], Bizible intègre insight aux formulaires qui ont été envoyés dans la plateforme [!DNL LinkedIn]. Ces remplissages de formulaires sont associés aux prospects de votre instance CRM (Gestion de la relation client) ou Adobe Marketo Engage afin qu’ils soient éligibles à l’attribution et puissent être suivis par rapport à vos autres engagements marketing.

## Annonces {#announcements}

* **Marketo Product Docs Switching Platforms** : nous sommes ravis d’annoncer que Marketo Product Docs a rejoint Adobe Experience League depuis le vendredi 7 mai. Vous pourrez toujours utiliser l’URL : docs.marketo.com, et si des articles existants sont marqués d’un signet, vous serez redirigé. Tous les documents sur les produits sont disponibles sur la nouvelle plateforme et des améliorations sont prévues pour plus tard dans l’année.

* **Administration rationalisée des utilisateurs et authentification unique proposée par le système d’identités Adobe** : à compter de juillet 2021, les nouveaux clients Adobe Marketo Engage seront intégrés à l’aide des informations d’identification d’utilisateur Adobe. La migration des clients actuels vers le système d’identités intégré n’aura pas lieu avant la mi-2022 et aucune action client n’est requise jusqu’à nouvel ordre. L’authentification unique permet aux administrateurs informatiques et de sécurité de gérer plusieurs instances de produit Adobe Marketo Engage ainsi que d’autres solutions Experience Cloud et de configurer l’authentification unique (organisation de services partagés) par le biais d’une console commune. Les administrateurs peuvent gérer facilement les groupes d’utilisateurs et les droits des utilisateurs via une Admin Console commune.

**_Webinaire de mise à jour du produit_**

[Webinaire de mise à jour de Marketo Engage de mai 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
