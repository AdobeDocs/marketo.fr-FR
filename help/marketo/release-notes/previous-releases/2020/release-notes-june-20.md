---
unique-page-id: 37357276
description: Notes de mise à jour - 20 juin - Documentation Marketo - Documentation du produit
title: Notes de mise à jour - Juin 20
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---

# Notes de mise à jour : 20 juin {#release-notes-june}

Les fonctionnalités suivantes sont incluses dans la version du 20 juin. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_** Les fonctionnalités suivantes seront publiées le **5 juin 2020**.

## Engagement Marketo de base {#core-marketo-engage}

* **[Predictive Audiences](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![(étoile)](assets/yellow-star.png) : les nouveaux filtres de liste dynamique et de campagne dynamique proposés par Adobe Sensei vous permettent de créer des segments d’audience optimisés par l’IA pour les programmes de marketing par e-mail, d’événement et de webinaire. Utilisez l’IA pour vous aider à segmenter les audiences en fonction de la probabilité d’enregistrement de piste pour un événement, de participation ou de désabonnement. Créez des audiences semblables basées sur des programmes précédents afin de répliquer efficacement les performances précédentes. Réalisez des objectifs de conversion avec un suivi prédictif des objectifs et obtenez des recommandations sur la manière d’affiner vos segments ciblés pour les programmes d’événement.
* **Batch Email Boost** ![(star)](assets/yellow-star.png) : amélioration de notre fonctionnalité de marketing par e-mail qui vous permet d’envoyer jusqu’à 3 millions d’e-mails par heure. Nous avons recréé la conception de notre campagne par lots et de notre traitement des rapports par courrier électronique afin d’améliorer les performances des programmes de courrier électronique et des campagnes par lots. Cela se traduit par un délai d’exécution plus court pour l’envoi, ainsi qu’une amélioration du délai d’achèvement. Configurez vos envois d’emails comme vous le feriez normalement. Il n’y a aucune complexité supplémentaire. Cette amélioration est disponible sous la forme d’un module complémentaire de produit qui comprend également un pack de lancement des services de diffusion, des outils de diffusion par e-mail et plusieurs adresses IP dédiées.
* **[Intégration d’audience avec Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)** : nouvelle intégration de Adobe Experience Cloud (AEC) qui vous permet de synchroniser des listes statiques de pistes connues à partir de Marketo Engage avec plusieurs applications AEC afin d’améliorer les programmes existants, de déverrouiller de nouveaux cas d’utilisation et d’orchestrer des campagnes multicanaux. Cette intégration comprend Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager et Adobe Advertising Cloud.
* **[Champs personnalisés d’un membre de programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)** : capturez et utilisez des champs personnalisés à propos d’un membre de programme. Utilisez ces nouveaux champs dans vos formulaires de Marketo Engage, affichez-les dans la liste des membres d’un programme, exploitez-les dans les filtres et déclencheurs de liste dynamique et incluez-les dans une nouvelle action de flux de campagne dynamique pour une automatisation améliorée et une personnalisation plus granulaire. Ils peuvent également être importés et exportés via l’interface utilisateur et les API. Amélioration de la fonctionnalité des champs et des objets de données personnalisés.
* **Décrire le membre du programme** : récupérez les métadonnées du membre du programme, ce qui vous permet d’importer et d’exporter des données de champ personnalisé de membre du programme à l’aide de l’API REST. Amélioration de notre API.
* **[Créer une tâche dans Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)** : créez des tâches pour les ventes dans Microsoft Dynamics à l’aide d’une nouvelle action de flux basée sur le comportement client capturé dans Marketo Engage. Amélioration de notre intégration CRM Microsoft Dynamics native.
* **Obtenir le formulaire utilisé par le point de terminaison de l’API List Asset** : récupérez une liste de ressources qui dépendent d’un formulaire. Amélioration de notre API.
* **Définir l’en-tête d’email via l’API** : activez la traduction automatique et la localisation des champs de pré-en-tête d’email. Amélioration de notre API.
* **Mise en cache d’images et de fichiers** : nous améliorons la stabilité du serveur du Marketo Engage en diffusant des ressources image et fichier à partir d’un cache de 60 secondes.

## Account-Based Marketing {#account-based-marketing}

![(star)](assets/yellow-star.png)

* **Nouvelle détection de compte généralement disponible**

   * La nouvelle détection de compte est une amélioration de notre fonctionnalité de profilage de compte qui vous permet de découvrir de nouveaux comptes cibles nets pour votre stratégie ABM en fonction de votre modèle de profil client idéal optimisé par l’IA. Affichez, sélectionnez et importez les nouveaux comptes recommandés, ainsi que leurs indicateurs de données d’ajustement et d’intention basés sur l’IA.

<br> 

**_Mise à jour tout au long du trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

## Bizible {#bizible}

![(star)](assets/yellow-star.png)

* **Intégration des programmes Marketo Engage** : extrayez les données de programme directement de Marketo Engage pour créer des points de contact le long du parcours d’attribution dans Bizible afin de créditer de manière appropriée les programmes de messagerie et d’engagement. Amélioration de l’intégration de notre Marketo Engage.
* **Intégration des activités de Marketo Engage (BETA)** : import direct des données d’activité de Marketo Engage dans Bizible pour créer des points de contact sur le parcours client et tous les modèles d’attribution. Par exemple, les changements de score de piste, les moments intéressants, les clics par courrier électronique ou toute activité personnalisée. Amélioration de l’intégration de notre Marketo Engage.
* **Intégration des attributs du client Bizible B2B (BETA)** : il s’agit d’une intégration Adobe Experience Cloud avec Adobe Analytics qui vous permet d’importer directement des données Bizible dans Adobe Analytics pour une analyse plus approfondie. Par exemple, l’analyse du trafic et du contenu d’un site basé sur un compte par nom de société, attributs de compte, opportunités de gestion de la relation client et individus à forte valeur ajoutée, comme défini par le chiffre d’affaires attribué Bizible et l’étape d’entonnoir.
* **Filtres et améliorations de Discover Bizible** : analysez vos données avec des filtres de canal, de sous-canal, de campagne et de segment dans les tableaux de bord. Renforcez la visibilité des données avec davantage d’attributs d’analyse. Il s’agit d’une amélioration de nos panoramas Discover .
* **Synchronisation des activités pour Microsoft Dynamics** : attribuez les interactions de vente en amenant les activités Microsoft Dynamics CRM au parcours de point de contact et suivez les événements tels que les appels, les rendez-vous ou les tâches associés à vos prospects ou contacts. Amélioration de l’intégration de Microsoft Dynamics CRM.

## Sales Insight {#sales-insight}

![(star)](assets/yellow-star.png)

* **[Tableau de bord des statistiques pour Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)** : nous sommes en train de repenser notre fonctionnalité de statistiques sur les ventes avec une nouvelle visibilité sur les événements et campagnes marketing à venir afin de donner aux vendeurs la possibilité de formuler des recommandations plus pertinentes pour les clients et les prospects en fonction de leurs besoins et de leurs intérêts. Les vendeurs peuvent également afficher l’activité Contact et Activité du compte dans la chronologie et accéder facilement aux détails supplémentaires de l’activité. Pour plus d&#39;informations sur la mise à niveau de votre package [ici](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## Annonces {#announcements}

* **Mise à jour RTP ITP 2.1+** : en raison de modifications apportées à la politique des cookies pour Safari, la capacité des cookies RTP à effectuer le suivi des utilisateurs entre les sessions sur le même domaine sera limitée par ITP à 1 ou 7 jours en fonction de la version du navigateur et de la version du navigateur utilisée par le visiteur. Pour ce faire, nous mettons en oeuvre un nouveau service Web pour permettre aux cookies RTP d’être définis avec un en-tête Set-Cookie via une réponse HTTP. Vous trouverez plus d&#39;informations [ici](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Changements d’infrastructure de campagne par lots** : nous mettons à niveau nos services de campagne par lots tout au long du reste de l’année. Il s’agit d’une mise à jour transparente qui n’affectera aucune campagne par lots en cours et qui n’entraînera pas de changement de comportement. Aucune action n’est requise. Pour en savoir plus, consultez cette [publication de nation](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Obsolescence {#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** : à partir de la version 159 de Munchkin JS, un avertissement d’obsolescence sera consigné dans la console du navigateur lors de l’appel de la méthode Associate Lead, indiquant que la fonctionnalité sera supprimée dans une prochaine version.  Le calendrier complet d’obsolescence sera annoncé ultérieurement.

**_Webinaire sur les versions de produit_** [Regardez l’enregistrement](https://engage.marketo.com/June-Release-2020-On-Demand.html) de notre webinaire sur les innovations de versions de produit du 20 juin.
