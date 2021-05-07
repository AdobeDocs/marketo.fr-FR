---
unique-page-id: 37357276
description: Notes de mise à jour - 20 juin - Marketo Docs - Documentation du produit
title: Notes de mise à jour - Juin 20
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
translation-type: tm+mt
source-git-commit: d44f5e6f3fb24a25678e4d15ee4c6361b658556b
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Notes de mise à jour : 20 juin {#release-notes-june}

Les fonctionnalités suivantes sont incluses dans la version du 20 juin. Consultez votre édition Marketo pour connaître la disponibilité des fonctionnalités.

>[!AVAILABILITY]
>
>Les fonctions signalées par une étoile (![](assets/yellow-star.png)) sont des modules complémentaires payants. Veuillez contacter votre représentant Marketo Engage pour en savoir plus.

**__** Versions trimestriellesLes fonctionnalités suivantes seront publiées le 5  **juin 2020**.

## Engagement Marketo de base {#core-marketo-engage}

* **[Audiences](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![ prédictives (étoile)](assets/yellow-star.png) : Les nouveaux filtres Smart Liste et Smart Campaign optimisés par Adobe Sensei vous permettent de créer des segments d’audience alimentés par l’IA pour les programmes de marketing par courriel, événement et webinaire. Utilisez l&#39;IA pour vous aider à segmenter les audiences en fonction de la probabilité de piste pour vous inscrire à un événement, participer à un événement ou vous désabonner. Créez des audiences semblables basées sur les programmes précédents pour reproduire efficacement les réussites précédentes. Réalisez des objectifs de conversion avec le suivi prédictif des objectifs et obtenez des recommandations sur la manière d&#39;affiner vos segments d&#39;audience pour les programmes de événement.
* **Optimisation** ![ du courrier électronique par lots (étoile)](assets/yellow-star.png) : Amélioration de notre fonctionnalité de marketing par courrier électronique qui vous permet d&#39;envoyer jusqu&#39;à 3 millions de courriers électroniques par heure. Nous avons réorganisé le traitement des campagnes par lots et des rapports par courriel afin d’améliorer les performances des programmes de courriel et des campagnes par lots. Cela se traduit par un délai d’envoi plus court et une meilleure exécution du programme. Configurez vos messages électroniques comme vous le feriez normalement, il n&#39;y a aucune complexité supplémentaire. Cette amélioration est disponible sous la forme d’un module complémentaire de produit qui inclut également un pack de lancement Diffusion Services, des outils de Diffusion électronique et plusieurs adresses IP dédiées.
* **[Intégration de l&#39;Audience à Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)** : Nouvelle intégration Adobe Experience Cloud (AEC) qui vous permet de synchroniser des listes statiques de pistes connues provenant de Marketo Engage avec plusieurs applications AEC afin d’améliorer les programmes existants, de déverrouiller de nouveaux cas d’utilisation et d’orchestrer des campagnes à canaux multiples. Cette intégration comprend Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager et Adobe Advertising Cloud.
* **[Champs](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)** personnalisés des membres de programme : Capturez et utilisez des champs personnalisés sur un membre de programme. Utilisez ces nouveaux champs dans vos formulaires Marketo Engage, vues-les dans la liste membre d’un programme, exploitez-les dans des filtres et déclencheurs de Liste intelligente, et incluez-les dans une nouvelle action Smart Campaign Flow pour une automatisation améliorée et une personnalisation plus granulaire. Ils peuvent également être importés et exportés via l’interface utilisateur et les API. Amélioration de la fonctionnalité des champs et objets de données personnalisés.
* **Décrivez le membre** du Programme : Récupérez les métadonnées de membre de Programme, ce qui vous permet d&#39;importer et d&#39;exporter des données de champ personnalisé de membre de Programme à l&#39;aide de l&#39;API REST. Amélioration de notre API.
* **[Créer une Tâche dans Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)** : Créez des tâches pour les ventes dans Microsoft Dynamics à l&#39;aide d&#39;une nouvelle action de flux basée sur le comportement des clients capturé dans le Marketo Engage. Amélioration de notre intégration native de Microsoft Dynamics CRM.
* **Obtenir le formulaire utilisé par le point de terminaison** de l&#39;API des ressources de Liste : Récupérez une liste de ressources qui dépend d’un formulaire. Amélioration de notre API.
* **Définir l’en-tête de courriel via l’API** : Activez la traduction automatique et la localisation des champs d’en-tête de courriel. Amélioration de notre API.
* **Mise en cache** des images et des fichiers : Nous améliorons la stabilité du serveur Marketo Engage en diffusant les fichiers Image et File à partir d’un cache de 60 secondes.

## Account-Based Marketing {#account-based-marketing}

![(étoile)](assets/yellow-star.png)

* **Nouvelle découverte de compte généralement disponible**

   * La nouvelle découverte de comptes est une amélioration de notre fonctionnalité de profilage de comptes qui vous permet de découvrir des comptes de cible Net-new pour votre stratégie ABM basée sur votre modèle de profil client idéal optimisé par l&#39;IA. Vue, sélectionnez et importez les nouveaux comptes recommandés, ainsi que leurs indicateurs d’ajustement et d’intention basés sur l’IA.

<br> 

**_Libération au cours du trimestre_**

Les fonctionnalités suivantes sont présentées sur un cycle non trimestriel et seront publiées au cours des prochains mois.

## Bizible {#bizible}

![(étoile)](assets/yellow-star.png)

* **Intégration** des Programmes Marketo Engage : Récupérez les données de programme directement du Marketo Engage pour créer des points de contact le long du parcours d’attribution dans Bizible afin de créditer correctement les programmes d’engagement et d’e-mail. Amélioration de notre intégration Marketo Engage.
* **Intégration des Activités Marketo Engage (BETA)** : Placez les données d’activité Marketo Engage directement dans la bibliothèque prête à l’emploi pour créer des points de contact sur le parcours client et tous les modèles d’attribution. Par exemple, les changements de score de piste, les moments intéressants, les clics par courriel ou toute activité personnalisée. Amélioration de notre intégration Marketo Engage.
* **Intégration des attributs client B2B (Bizible) (BETA)** : Il s&#39;agit d&#39;une intégration Adobe Experience Cloud avec Adobe Analytics qui vous permet d&#39;apporter directement des données lisibles à Adobe Analytics pour une analyse plus approfondie. Par exemple, le trafic du site basé sur le compte et l’analyse du contenu par nom de société, les attributs de compte, les opportunités de gestion de la relation client et les personnes à forte valeur ajoutée, comme défini par les recettes attribuées et l’étape de l’entonnoir.
* **Bizible Discover Filtres and Enhancements** : Analysez vos données à l’aide de filtres de canal, de sous-canal, de campagne et de segments sur plusieurs tableaux de bord. Améliorez la visibilité des données grâce à des attributs plus détaillés. Il s’agit d’une amélioration pour nos panoramas Discover.
* **Synchronisation des Activités pour Microsoft Dynamics** : Attribuez les interactions de vente en apportant les activités Microsoft Dynamics CRM au parcours de points de contact et en suivant les événements tels que les appels, les rendez-vous ou les tâches associés à vos prospects ou contacts. Amélioration de notre intégration Microsoft Dynamics CRM.

## Sales Insight {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **[Tableau de bord Insights pour Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)** : Nous réinventons notre fonctionnalité Sales Insight avec une nouvelle visibilité sur les événements et campagnes marketing à venir afin de donner aux vendeurs la possibilité de formuler des recommandations plus pertinentes pour les clients et les prospects en fonction de leurs besoins et de leurs intérêts. Les vendeurs peuvent également vue à l&#39;Activité des contacts et des comptes dans le délai imparti et accéder facilement à d&#39;autres détails sur l&#39;activité. Pour plus d&#39;informations sur la mise à niveau de votre paquet [ici](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/configuration-for-existing-customers.md).

<br> 

## Annonces {#announcements}

* **Mise à jour** RTP ITP 2.1+ : En raison des modifications apportées à la stratégie des cookies pour Safari, la capacité des cookies RTP à effectuer le suivi des utilisateurs entre les sessions sur le même domaine sera limitée par ITP à 1 ou 7 jours en fonction du navigateur et de la version du navigateur utilisés par le visiteur. Pour ce faire, nous mettons en oeuvre un nouveau service Web pour permettre la définition de cookies RTP avec un en-tête Set-Cookie via la réponse HTTP. Vous trouverez plus d&#39;informations [ici](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Changements** d&#39;infrastructure par lots Campaign : Nous mettons à niveau nos services de campagne par lots tout au long de l&#39;année. Il s’agira d’une mise à jour transparente qui n’affectera aucune campagne par lot en cours et n’entraînera aucun changement de comportement. Aucune action n’est requise. Pour plus d&#39;informations, consultez cet [article de Nation](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Dépréciations {#deprecations}

* **[Munchkin Responsable](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** associé : À partir de la version 159 de Munchkin JS, un avertissement de désapprobation sera consigné dans la console du navigateur lorsque la méthode Associer le prospect sera appelée, indiquant que la fonction sera supprimée dans une prochaine version.  Le calendrier complet d&#39;abandon sera annoncé à une date ultérieure.

**_Webinaire_** [sur la version des produitsRegardez l&#39;](https://engage.marketo.com/June-Release-2020-On-Demand.html) enregistrement de notre webinaire sur les innovations de la version des produits du 20 juin.
