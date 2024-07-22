---
description: Notes de mise à jour - Août 2021 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Août 2021
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# Notes de mise à jour : août 2021 {#release-notes-aug-21}

Les fonctionnalités suivantes sont incluses dans la version du 21 août. Pour connaître la disponibilité des fonctionnalités, consultez l’édition de votre Marketo Engage .

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Adobe Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **20 août 2021**.

## Automatisation de l’expérience {#experience-automation}

* **Authentification de l’utilisateur Marketo Engage via l’identité d’Adobe** : bientôt, les nouveaux utilisateurs Marketo Engage avec des packages d’entreprise seront intégrés à l’aide des informations d’identification de l’utilisateur Adobe ID. La migration des utilisateurs actuels vers le système d’identité intégré ne se fera pas avant la mi-2022 et aucune action n’est requise avant avis préalable. L’authentification des utilisateurs de l’identité Adobe permet aux administrateurs informatiques/de sécurité de gérer plusieurs instances de produit de Marketo Engage avec d’autres solutions Experience Cloud, ainsi que de configurer la connexion unique par le biais d’une console commune. Les administrateurs peuvent facilement gérer les groupes d’utilisateurs et les droits des utilisateurs au même endroit.

* **Imbrication de campagne exécutable** : les campagnes exécutables peuvent désormais également appeler d’autres campagnes exécutables, ce qui vous permet de les imbriquer jusqu’à trois niveaux de profondeur. Cela permet de consolider davantage les flux opérationnels communs et d&#39;améliorer la gestion dynamique des campagnes.

* **Action de flux unique dans la page Détails de la personne** (Disponible d’ici le 9 septembre) : exécutez les actions de flux comme l’envoi d’un courrier électronique, le changement de propriétaire ou toute autre action de campagne dynamique sur des personnes à partir de la page Détails de la personne à l’aide du menu d’actions de flux sans passer en vue de la grille de base de données.

* **[Exportation d’activités personnalisées](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)** : l’exportation de métadonnées prend désormais en charge tous les objets et métadonnées respectifs qui peuvent être utilisés pour partager, analyser et concevoir votre modèle de données d’abonnement.

## Améliorations des API {#api-enhancements}

* **API Submit Form** : lorsqu’une adresse électronique est dupliquée dans plusieurs enregistrements de piste, nous mettons à jour l’enregistrement &quot;dernière mise à jour&quot; au lieu de l’ignorer complètement. Fournit une parité avec l’API Forms 2.0.

* **API email** : récupérez les ressources email du champion ou du challenger. Récupérez les ressources par e-mail à l’aide du filtre de période.

**_Mise à jour tout au long du trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

## Sales Insight {#sales-insight}

![(star)](assets/yellow-star.png)

* **Amélioration de la visibilité des activités de prospect, contact, compte et opportunité pour les utilisateurs de Salesforce CRM** : l&#39;engagement avec les prospects durant les longs cycles de vente est plus informé en raison d&#39;un nombre accru d&#39;enregistrements d&#39;engagement dans Sales Insight. Les onglets Moments intéressants, Activité web, Courrier électronique et Score affichent jusqu’à 400 activités dans les objets de piste, de contact, de compte et d’opportunité.

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **Limitation de la connexion par e-mail (Beta)** : améliorez la délivrabilité des e-mails et réduisez la communication personnalisée sur les ventes grâce au ralentissement de la connexion par e-mail pour Sales Connect. Cette nouvelle technologie gère automatiquement le délai d’envoi des emails afin de créer des expériences transparentes pour les utilisateurs d’Exchange et de Gmail. Réduisez ou supprimez l’utilisation des applications tierces d’envoi de courriers électroniques en masse et envoyez tous vos courriers électroniques à Sales Connect en toute confiance.

>[!NOTE]
>
>Le ralentissement des emails est désormais disponible dans Beta. [En savoir plus](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Statistiques sur les activités de vente améliorées** : capturez et activez l’engagement personnalisé en fonction des activités antérieures de votre équipe commerciale. De nouveaux attributs tels que le lien d’enregistrement des appels commerciaux, le nom de la campagne commerciale et l’objet du courrier électronique commercial peuvent être utilisés dans les listes dynamiques de Marketo Engage.  Ces activités peuvent être exportées et consignées par le biais de l’API REST du Marketo Engage ou de l’exportation en bloc. Elles sont disponibles sur les filtres et les déclencheurs en tant que contraintes supplémentaires pour les listes dynamiques.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Intégration de Forms de génération de piste Bizible LinkedIn** : les marketeurs peuvent désormais attribuer des recettes sur les conversions survenant lorsque LinkedIn capture les formulaires via leurs unités publicitaires de génération de pistes Forms. Ces informations peuvent ensuite être utilisées pour optimiser les performances des formulaires et les investissements dans les médias payants. LinkedIn Lead Gen Forms est l’une des offres de médias payants les plus dynamiques de LinkedIn. Cette nouvelle fonctionnalité est incluse dans notre intégration LinkedIn Ads existante avec Bizible.

* **Tableau de bord Velocity amélioré** : nous avons ajouté une nouvelle mesure de vitesse et un nouveau filtre de tableau de bord pour obtenir des informations plus approfondies. Ce tableau de bord est utilisé par les marketeurs pour comprendre la vitesse des prospects et des opportunités, ainsi que l’efficacité de différentes formes d’engagement marketing et commercial.

* **Nouveau tableau de bord du Parcours de cascade de cohortes** : permet aux spécialistes du marketing de visualiser la progression d’une cohorte sélectionnée au moyen d’un ensemble d’étapes classiques de &quot;chute d’eau de la demande&quot;, ce qui permet de comprendre rapidement les taux de conversion et la causalité de conversion implicite étape par étape.

## Intégration de Bizible à Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Cette section comprend de nouvelles fonctionnalités pour les utilisateurs Bizible qui ont terminé leur migration Adobe Identity Management System (IMS). Si vous avez été migré, votre nouvelle Adobe ID s’affiche dans les paramètres Bizible sous l’onglet Adobe ID. Tous les comptes doivent être migrés d&#39;ici fin 2021.

* **Intégration Bizible avec Adobe Privacy Service** (disponible en septembre 2021) : l’intégration de Bizible à l’Adobe Privacy Service centralise la conformité avec les réglementations de confidentialité des données critiques (telles que le RGPD) dans les applications Adobe Experience Cloud. Vous pouvez désormais tirer parti de ce service et gérer toutes les demandes d’accès à des informations personnelles de manière centralisée afin que les demandes de modification arrivant dans Bizible et d’autres produits Adobe soient répercutées dans toutes les applications.

* **Bizible sur l’interface de Adobe Experience Cloud** : l’adoption de l’interface Adobe Experience Cloud par Bizible offre aux utilisateurs de nouvelles fonctionnalités qui apparaîtront dans la barre d’en-tête de l’application Bizible, ainsi qu’un meilleur accès aux ressources de prise en charge et au changement d’application. L’interface Experience Cloud permet de créer une expérience cohérente entre Bizible et d’autres applications Adobe Experience Cloud.

* **Propriété du domaine Bizible et auto-gestion** : les utilisateurs Bizible peuvent tirer parti de Adobe Admin Console pour gérer les domaines dont Bizible doit effectuer le suivi. Cela permet d’accéder en libre-service à un processus manuel précédent et offre une expérience cohérente de la gestion de la propriété et du suivi des domaines dans les applications Adobe Experience Cloud.

## Annonces {#announcements}

* **Mise à jour des paramètres d’ID universel d’abonnement** : pour prendre en charge l’intégration du prochain Marketo Engage et de l’identité d’Adobe pour les utilisateurs existants, tous les abonnements du Marketo Engage seront unifiés dans le cadre de la prise en charge de l’ID universel. Vous trouverez plus d&#39;informations [ici](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinaire sur la version du produit_**

[Webinaire de mise à jour du Marketo Engage d’août 2021](https://engage.marketo.com/August21_Release_Webinar.html)
