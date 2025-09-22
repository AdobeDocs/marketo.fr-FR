---
unique-page-id: 37357276
description: Notes De Mise À Jour -20 Juin - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Juin 2020
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 1%

---

# Notes de mise à jour : juin 2020 {#release-notes-june}

Les fonctionnalités suivantes sont incluses dans la version du 20 juin. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

**_Versions trimestrielles_** Les fonctionnalités suivantes seront publiées le **5 juin 2020**.

## Engagement Marketo de base {#core-marketo-engage}

* **[Audiences prédictives](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=fr#predictive-audiences)** ![(étoile)](assets/yellow-star.png) : les nouveaux filtres de liste dynamique et de campagne dynamique optimisés par Adobe Sensei vous permettent de créer des segments d’audience optimisés par l’IA pour les programmes marketing d’e-mail, d’événement et de webinaire. Utilisez l’IA pour segmenter les audiences en fonction de la probabilité de prospect de vous inscrire à un événement, d’y assister ou de vous désinscrire. Créez des audiences semblables en fonction de programmes précédents afin de répliquer efficacement les succès précédents. Atteignez les objectifs de conversion avec un suivi des objectifs prédictif et obtenez des recommandations sur la manière d’affiner vos segments d’audience pour les programmes d’événement.
* **Boost d’e-mail par lots** ![(étoile)](assets/yellow-star.png) : amélioration de notre fonctionnalité de marketing par e-mail qui vous permet d’envoyer jusqu’à 3 millions d’e-mails par lot et par heure. Nous avons repensé le traitement des campagnes par lots et des rapports par e-mail afin d’améliorer les performances des programmes de messagerie et des campagnes par e-mail par lots. Le délai d’envoi est ainsi réduit et le temps d’achèvement amélioré. Configurez vos envois d’e-mail comme vous le feriez normalement, cela n’ajoute aucune complexité. Cette amélioration est disponible sous la forme d’un module complémentaire de produit qui comprend également un pack de lancement des services de diffusion, des outils de diffusion par e-mail et plusieurs adresses IP dédiées.
* **[Audience Integration with Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)** : nouvelle intégration de Adobe Experience Cloud (AEC) qui vous permet de synchroniser les listes statiques de prospects connus de Marketo Engage avec plusieurs applications AEC afin d’améliorer les programmes existants, de déverrouiller de nouveaux cas d’utilisation et d’orchestrer des campagnes multicanal. Cette intégration inclut Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager et Adobe Advertising Cloud.
* **[Champs personnalisés du membre de programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)** : capturez et utilisez les champs personnalisés relatifs à un membre de programme. Utilisez ces nouveaux champs dans vos formulaires Marketo Engage, affichez-les dans la liste des membres d’un programme, exploitez-les dans les filtres et les déclencheurs de liste dynamique et incluez-les dans une nouvelle action de flux de campagne dynamique pour une automatisation améliorée et une personnalisation plus granulaire. Ils peuvent également être importés et exportés via l’interface utilisateur et les API. Amélioration de notre fonctionnalité d’objets et de champs de données personnalisés.
* **Décrire le membre de programme** : récupérez les métadonnées du membre de programme, ce qui vous permet d’importer et d’exporter des données de champ personnalisé de membre de programme à l’aide de l’API REST. Amélioration de notre API.
* **[Créer une tâche dans [!DNL Microsoft Dynamics]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)** : créez des tâches pour les ventes dans [!DNL Microsoft Dynamics] à l’aide d’une nouvelle action de flux basée sur le comportement du client capturé dans Marketo Engage. Amélioration de notre intégration native [!DNL Microsoft Dynamics] CRM.
* **Obtenir le formulaire utilisé par le point d’entrée de l’API List Asset** : récupérez une liste de ressources qui dépendent d’un formulaire. Amélioration de notre API.
* **Définir le pré-titre de l’e-mail via l’API** : activer la traduction et la localisation automatiques des champs de pré-titre des e-mails. Amélioration de notre API.
* **Mise en cache des images et des fichiers** : nous améliorons la stabilité du serveur Marketo Engage en diffusant des ressources d’images et de fichiers à partir d’un cache de 60 secondes.

## Account-Based Marketing {#account-based-marketing}

![(étoile)](assets/yellow-star.png)

* **Nouvelle découverte de compte généralement disponible**

   * La détection de nouveaux comptes est une amélioration de notre fonctionnalité de profilage des comptes qui vous permet de découvrir de nouveaux comptes cibles pour votre stratégie ABM en fonction de votre modèle de profil client idéal optimisé par l’IA. Affichez, sélectionnez et importez les nouveaux comptes recommandés, ainsi que leurs indicateurs de données d’ajustement et d’intention basés sur l’IA.

<br> 

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes font l’objet d’un cycle non trimestriel et seront publiées au cours des prochains mois.

## [!DNL Bizible] {#bizible}

![(étoile)](assets/yellow-star.png)

* **Intégration des programmes Marketo Engage** : extrayez les données du programme directement depuis Marketo Engage pour créer des points de contact le long du parcours d’attribution [!DNL Bizible] de créditer de manière appropriée les programmes d’e-mail et d’engagement. Amélioration de notre intégration Marketo Engage.
* **Intégration des activités Marketo Engage (BETA)** : importez les données d’activité Marketo Engage directement dans [!DNL Bizible] pour créer des points de contact sur le parcours client et tous les modèles d’attribution. Par exemple, les modifications du score du prospect, les moments intéressants, les clics sur un e-mail ou toute activité personnalisée. Amélioration de notre intégration Marketo Engage.
* **[!DNL Bizible]intégration des attributs du client B2B (BETA)** : il s’agit d’une intégration de Adobe Experience Cloud à Adobe Analytics qui vous permet d’importer directement certaines données Bizible dans Adobe Analytics pour une analyse plus approfondie. Par exemple, le trafic sur le site basé sur les comptes et l’analyse du contenu par nom de société, les attributs de compte, les opportunités CRM et les individus à forte valeur ajoutée, tels que définis par [!DNL Bizible] niveau de chiffre d’affaires attribué et d’entonnoir.
* **[!DNL Bizible]Découvrir les filtres et les améliorations** : analysez vos données à l’aide de filtres de canal, de sous-canal, de campagne et de segment sur les tableaux de bord. Renforcez la visibilité des données avec des attributs plus détaillés. Il s’agit d’une amélioration de nos tableaux Discover.
* **Synchronisation des activités pour les[!DNL Microsoft Dynamics]** : attribuez des interactions de vente en apportant des activités de gestion de la relation client (CRM) [!DNL Microsoft Dynamics] au parcours de points de contact et suivez des événements tels que des appels, des rendez-vous ou des tâches associées à vos prospects ou contacts. Amélioration de notre intégration CRM [!DNL Microsoft Dynamics].

## [!DNL Sales Insight] {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **[Tableau de bord d’informations pour Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)** : nous réimaginons notre fonctionnalité [!DNL Sales Insight] avec une nouvelle visibilité sur les événements et campagnes marketing à venir, afin de permettre aux vendeurs de faire des recommandations plus pertinentes pour les clients et les prospects en fonction de leurs besoins et de leurs intérêts. Les vendeurs peuvent également afficher les activités de contact et de compte dans la chronologie et accéder facilement aux détails des activités supplémentaires. Pour plus d’informations sur la mise à niveau de votre package, cliquez [ici](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## Annonces {#announcements}

* **ITP 2.1+ RTP Update** : en raison des modifications apportées à la politique des cookies pour [!DNL Safari], la capacité des cookies RTP à suivre les utilisateurs entre les sessions sur le même domaine sera limitée par ITP à 1 ou 7 jours en fonction du navigateur et de la version du navigateur utilisés par le visiteur. Pour en tenir compte, nous mettons en œuvre un nouveau service web pour permettre la définition des cookies RTP avec un en-tête Set-Cookie via une réponse HTTP. Vous trouverez plus d’informations [ici](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Modifications de l’infrastructure de campagnes par lots** : nous mettons à niveau nos services de campagnes par lots pour le reste de l’année. Il s’agira d’une mise à jour transparente qui n’affectera aucune campagne par lots en cours et n’entraînera aucun changement de comportement. Aucune action n’est requise. Retrouvez plus de détails dans ce billet [Nation](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Obsolescence {#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** : à partir de la version 159 de [!DNL Munchkin] JS, un avertissement d’obsolescence est consigné dans la console du navigateur lorsque la méthode Associate Lead est appelée, indiquant que la fonctionnalité sera supprimée dans une version ultérieure.  La planification complète d’abandon sera annoncée ultérieurement.

**_Webinaire sur la mise à jour des produits_** [Regardez l’enregistrement](https://engage.marketo.com/June-Release-2020-On-Demand.html) de notre webinaire sur les innovations de mise à jour des produits du 20 juin.
