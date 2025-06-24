---
description: Notes De Mise À Jour - Août 2021 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Août 2021
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Notes De Mise À Jour : Août 2021 {#release-notes-aug-21}

Les fonctionnalités suivantes sont incluses dans la version d’août 2021. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Adobe Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **20 août 2021**.

## Automatisation de l’expérience {#experience-automation}

* **Authentification des utilisateurs Marketo Engage via Adobe Identity** : bientôt, de nouveaux utilisateurs Marketo Engage avec des packages Enterprise seront intégrés à l’aide des informations d’identification d’utilisateur Adobe ID. La migration des utilisateurs actuels vers le système d’identités intégré n’aura pas lieu avant la mi-2022 et aucune action n’est requise jusqu’à nouvel ordre. L’authentification des utilisateurs d’identité Adobe permet aux administrateurs informatiques et de sécurité de gérer plusieurs instances de produit Marketo Engage ainsi que d’autres solutions Experience Cloud, et de configurer la connexion unique via une console commune. Les administrateurs peuvent facilement gérer les groupes d’utilisateurs et les droits des utilisateurs au même endroit.

* **Imbrication de campagnes exécutables** : les campagnes exécutables peuvent désormais appeler d’autres campagnes exécutables, ce qui vous permet de les imbriquer jusqu’à trois niveaux de profondeur. Cela permet de consolider davantage les flux opérationnels courants et d’améliorer la gestion des campagnes intelligentes.

* **Action de flux unique dans la page des détails d’une personne** (disponible avant le 9 septembre) : exécutez des actions de flux telles que l’envoi d’un e-mail, le changement de propriétaire de personne ou toute autre action de campagne intelligente sur des personnes à partir de la page des détails de la personne à l’aide du menu d’action de flux sans passer à la vue de grille de la base de données.

* **[Exportation d’activités personnalisées](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)** : l’exportation des métadonnées prend désormais en charge tous les objets et les métadonnées respectives qui peuvent être utilisés pour partager, analyser et concevoir le modèle de données d’abonnement.

## Améliorations de l’API {#api-enhancements}

* **API de formulaire d’envoi** : lorsqu’une adresse e-mail est dupliquée dans plusieurs enregistrements de prospect, nous mettons à jour l’enregistrement « dernière mise à jour » au lieu de l’ignorer complètement. Fournit la parité avec l’API Forms 2.0.

* **API Email** : récupération des ressources d’e-mail championnes ou challenger. Récupérez les ressources d’e-mail à l’aide du filtre de période.

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes font l’objet d’un cycle non trimestriel et seront publiées au cours des prochains mois.

## [!DNL Sales Insight] {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **Visibilité accrue des activités liées aux leads, aux contacts, aux comptes et aux opportunités pour les utilisateurs de Salesforce CRM** : l’engagement des prospects au cours des longs cycles de vente est plus éclairé en raison du nombre accru d’enregistrements d’engagement dans [!DNL Sales Insight]. Les onglets Moments intéressants, Activité web, E-mail et Score affichent jusqu’à 400 activités pour les objets Lead, Contact, Compte et Opportunité.

## [!DNL Sales Connect] {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Limitation de la connexion aux e-mails (Beta)** : améliorez la délivrabilité des e-mails et mettez à l’échelle la communication commerciale personnalisée grâce à la limitation de la connexion aux e-mails pour Sales Connect. Cette nouvelle technologie gère automatiquement le délai d’envoi des e-mails afin de créer des expériences transparentes pour les utilisateurs d’[!DNL Exchange] et de Gmail. Réduisez ou éliminez l&#39;utilisation des applications tierces d&#39;envoi d&#39;emails en masse et envoyez tous vos emails depuis [!DNL Sales Connect] en toute confiance.

>[!NOTE]
>
>La limitation des e-mails est désormais disponible dans Beta. [En savoir plus](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Enhanced Sales Activity Insights** : permet de capturer et d’activer un engagement personnalisé en fonction des activités précédentes de votre équipe des ventes. De nouveaux attributs tels que le lien d’enregistrement des appels commerciaux, le nom de la campagne commerciale et l’objet de l’e-mail commercial peuvent être utilisés dans les listes dynamiques Marketo Engage.  Ces activités peuvent être exportées et signalées via l’API REST Marketo Engage ou l’exportation en bloc. Elles sont disponibles sur les filtres et les déclencheurs en tant que contraintes supplémentaires pour les listes dynamiques.

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* **[!DNL Bizible][!DNL LinkedIn] intégration de Forms génération de leads** : les marketeurs peuvent désormais effectuer l’attribution des revenus sur les conversions qui se produisent lorsque [!DNL LinkedIn] capture les remplissages de formulaires par le biais de leurs unités publicitaires de Forms génération de leads. Ces informations peuvent ensuite être utilisées pour optimiser les performances des formulaires et les investissements payants dans les médias. [!DNL LinkedIn] Lead Gen Forms est l’une des offres de médias payants à la croissance la plus rapide de [!DNL LinkedIn]. Cette nouvelle fonctionnalité est incluse dans notre intégration [!DNL LinkedIn] Ads existante à [!DNL Bizible]. 
 
* **Tableau de bord de vitesse amélioré** : nous avons ajouté une nouvelle mesure de vitesse et un nouveau filtre de tableau de bord pour obtenir des informations plus détaillées. Ce tableau de bord est utilisé par les spécialistes marketing pour comprendre le lead étape par étape, la vitesse des opportunités et l’efficacité de différentes formes d’engagement en matière de marketing et de vente.

* **Nouveau tableau de bord de Parcours de cascade de cohortes** : il permettra aux professionnels du marketing d’afficher la progression d’une cohorte sélectionnée à travers un ensemble classique d’étapes de « cascade de demandes », ce qui permettra une compréhension rapide des taux de conversion et de la causalité de conversion implicite d’une étape à l’autre.

## Intégration d’[!DNL Bizible] à Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Cette section comprend de nouvelles fonctionnalités pour les utilisateurs de Bizible qui ont terminé leur migration vers Adobe Identity Management System (IMS). Si vous avez fait l’objet d’une migration, votre nouvelle Adobe ID s’affichera dans [!DNL Bizible] Paramètres sous l’onglet Adobe ID . Tous les comptes devraient faire l’objet d’une migration d’ici fin 2021.

* Intégration d’**[!DNL Bizible]à Adobe Privacy Service** (disponible en septembre 2021) : l’intégration d’[!DNL Bizible] à Adobe Privacy Service centralise la conformité aux réglementations critiques en matière de confidentialité des données (telles que le RGPD) dans les applications Adobe Experience Cloud. Vous pouvez désormais tirer parti de ce service et gérer toutes les demandes d’accès à des informations personnelles de manière centralisée, de sorte que les demandes de modification arrivant dans [!DNL Bizible] et d’autres produits Adobe soient prises en compte dans toutes les applications.

* **[!DNL Bizible]sur Adobe Unified Shell** : l’adoption d’Adobe Unified Shell par [!DNL Bizible] donne aux utilisateurs de nouvelles fonctionnalités qui s’afficheront dans la barre d’en-tête de l’application [!DNL Bizible] et comprennent un meilleur accès aux ressources de prise en charge et au changement d’application. Adobe Unified Shell permet de créer une expérience cohérente entre [!DNL Bizible] et les autres applications Adobe Experience Cloud.

* **[!DNL Bizible]la propriété de domaine et l’auto-gestion** : [!DNL Bizible] utilisateurs peuvent utiliser Adobe Admin Console pour gérer les domaines qu’ils [!DNL Bizible] suivre. Cela apporte du libre-service à un processus manuel précédent et fournit une expérience cohérente dans la manière dont la propriété et le suivi des domaines sont gérés dans les applications Adobe Experience Cloud.

## Annonces {#announcements}

* **Mise à jour des paramètres d’ID d’abonnement universel** : pour prendre en charge l’intégration d’identité Marketo Engage et Adobe à venir pour les utilisateurs existants, tous les abonnements Marketo Engage seront unifiés afin d’activer la prise en charge d’ID universel. Vous trouverez plus d’informations [ici](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinaire de mise à jour du produit_**

[Webinaire De Mise À Jour De Marketo Engage D’Août 2021](https://engage.marketo.com/August21_Release_Webinar.html)
