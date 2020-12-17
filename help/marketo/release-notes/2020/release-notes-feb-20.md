---
unique-page-id: 37355826
description: Notes de mise à jour - Février 20 - Documentation sur le marketing - Documentation sur le produit
title: Notes de mise à jour - Fév '20
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---


# Notes de mise à jour : 20 février {#release-notes-feb}

Les fonctionnalités suivantes sont incluses dans la version du 20 février. Vérifiez la disponibilité des fonctionnalités de votre édition Marketing.

>[!NOTE]
>
>**Disponibilité**
>
>Les fonctions signalées par une étoile ( ![(star)](assets/star-yellow.svg)) sont des modules complémentaires payants. Veuillez contacter votre représentant Marketo Engage pour en savoir plus.

****** Versions trimestriellesLes fonctionnalités suivantes ont été publiées le 21  **février 2020**.

## Marketo Engage principal {#core-marketo-engage}

* **Action** de flux Microsoft Dynamics &quot;Change Owner in Microsoft&quot; : Conserver le contrôle de vos données Microsoft Dynamics CRM avec la possibilité de modifier un responsable/contact directement du Marketo Engage. Il s’agit d’une amélioration de notre fonctionnalité d’intégration CRM native.
* **API de gestion des utilisateurs : **Automatisez la gestion des utilisateurs et des rôles grâce à des systèmes de gestion des identités et des organisations externes. Il s&#39;agit d&#39;une amélioration de notre fonctionnalité Appels d&#39;API.
* **API de Schéma d’objets personnalisés : **Gérez et provisionnez automatiquement des schémas d’objets personnalisés dans les instances du Marketo Engage afin de conserver la cohérence des modèles de données entre vos outils de vente et marketing. Grâce à cette API, vous pouvez définir et tester des objets personnalisés dans un sandbox ou un centre d’excellence et fournir autant d’instances que nécessaire. Il s’agit d’une amélioration de la fonctionnalité Appels d’API. Veuillez contacter votre représentant Marketo Engage pour savoir comment accéder à cette amélioration.
* **API** de règles de redirection de landing page : Automatisez la gestion des règles de redirection de landing page. Il s&#39;agit d&#39;une amélioration de notre fonctionnalité Appels d&#39;API.
* **Mise en cache** du descripteur de formulaire : Nous réduisons le temps de chargement des formulaires incorporés et améliorons la stabilité générale des applications en mettant en cache les formulaires sous forme de ressources. Veuillez noter que les approbations apportées aux formulaires incorporés peuvent prendre jusqu&#39;à quatre minutes pour réfléchir sur le Web. Il s’agit d’une amélioration de nos capacités de Landings page et de Forms.

<br> 

**

***Libération au cours du trimestre***

Les fonctionnalités suivantes sont présentées sur un cycle non trimestriel et seront publiées au cours des prochains mois.
**Bizible ![(star)](assets/star-yellow.svg)

**

* **Segmentation** basée sur un compte : Analyser l&#39;attribution au niveau du compte en ayant la possibilité de créer des segments et des filtres pour les panoramas Discover en fonction des attributs du compte. Utilisez ces segments pour analyser en détail les performances marketing basées sur votre compte.
* **Enregistrement des Filtres** : Enregistrez des filtres spécifiques à chaque tableau de bord, propres à chaque utilisateur, afin d’analyser vos tableaux de bord de manière rapide et cohérente.
* **Exporter au format PDF** : Partagez des informations précieuses sur votre entreprise en exportant des Tableaux de bord visibles au format PDF.

## Connexion commerciale {#sales-connect}

* **Composer les mises à jour** de la fenêtre : Nous avons rationalisé le processus de sélection des modèles et d&#39;envoi de courriers électroniques via Sales Connect. Utilisez la fenêtre Composer de notre client Web et de Salesforce comme guichet unique pour les vendeurs, avec la possibilité d&#39;enregistrer des catégories de modèles, de planifier des e-mails, d&#39;envoyer des e-mails en masse et d&#39;envoyer des e-mails avec vue et suivi des clics.
* **Mises à jour** du Centre de commandes : Nous sommes en train de reconstruire le centre de commandes de Sales Connect afin de donner aux vendeurs un aperçu de tous leurs courriels, appels et Tâches lancés à partir de Sales Connect. Ils peuvent également vue des informations, telles que l&#39;engagement par courrier électronique et la délivrabilité, à partir du Centre de commandes.

<br> 

## Annonces {#announcements}

* **Centre** de réussite des Marketo Engage : Nous lançons le centre de réussite Marketo en février 2020. Le centre de réussite est un centre d&#39;aide intégré qui vous permet de rechercher des documents produit et la communauté, de lancer des guides pratiques, d&#39;accéder au contenu d&#39;adoption tel que l&#39;Université Marketo et des vidéos des meilleures pratiques d&#39;évaluation, etc., directement depuis votre instance de Marketo Engage. **Remarque** : Cette fonctionnalité sera lancée en version bêta en ANZ et sera déployée en Amérique du Nord plus tard dans le trimestre.

## Dépréciations {#deprecations}

* **Paramètre** de l&#39;API de ressource &quot;_method&quot; : Après septembre 2020, les points de terminaison de l’API Asset n’accepteront plus &quot;_method&quot; pour transmettre les paramètres de Requête dans un corps de POST afin de contourner les limitations de longueur d’URI. Pour répondre aux demandes qui nécessitaient ce paramètre, la limite d’URI pour les API d’actifs sera augmentée de 6KiB à 65KiB, de sorte que les URI de demande longue puissent être envoyés.
* **Dépréciation** de la prise en charge d&#39;Internet Explorer : À compter de notre version du 31 juillet 2020, l’interface utilisateur du Marketo Engage ne sera plus prise en charge dans Internet Explorer.

***Webinaire*** [sur la version du produitRejoignez ](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) le 3 mars à 11h00 PT / 14h00 ET pour un webinaire en direct hébergé par notre équipe produit et découvrez les fonctionnalités de cette version.
