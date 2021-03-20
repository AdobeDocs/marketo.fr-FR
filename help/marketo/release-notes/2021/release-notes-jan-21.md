---
description: Notes de mise à jour - Janvier 2021 - Documents marketing - Documentation du produit
title: Notes de mise à jour - Janvier 2021
translation-type: tm+mt
source-git-commit: 073b73255d49f859c32c8b4793e6798f02f7a5c4
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---


# Notes de mise à jour : Jan 2021 {#release-notes-jan-21}

Les fonctionnalités suivantes sont incluses dans la version du 21 janvier. Vérifiez la disponibilité des fonctionnalités de votre édition Marketing.

>[!AVAILABILITY]
>
>Les fonctions signalées par une étoile ( ![(star)](assets/star-yellow.svg)) sont des modules complémentaires payants. Veuillez contacter votre représentant Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **15 janvier 2021**.

## Expérience utilisateur de nouvelle génération {#next-generation-user-experience}

* Prise en charge des espaces de travail : La nouvelle génération d&#39;utilisateurs Marketo Engage rassemble l&#39;apparence de Adobe Experience Cloud avec des innovations en matière de productivité pour aider les spécialistes du marketing à travailler plus rapidement et plus intelligemment. Dans la dernière version, nous ajoutons une prise en charge complète des espaces de travail et des partitions, y compris la possibilité de partager des dossiers entre les espaces de travail. Le canevas à droite offre un commutateur à bascule pour vous permettre de transition harmonieuse entre les expériences anciennes et nouvelles par fonction sans perdre de contexte. [En savoir ](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) plus sur la FAQ sur l’expérience de la prochaine génération sur Marketing Nation.

## Personnalisation à plusieurs Canaux {#multi-channel-personalization}

* **[Phase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)** de la synchronisation des Audiences Adobe Experience Cloud : La fonctionnalité de synchronisation des Audiences Adobe Experience Cloud (AEC) existante prend désormais en charge la synchronisation continue et bidirectionnelle des audiences B2B du Marketo Engage à d’autres applications AEC, y compris les offres Adobe Experience Platform (AEP) telles que la plateforme de données client en temps réel et la Activation Adobe Experience Platform.  À mesure que des pistes sont ajoutées et supprimées dans vos segments d’audience, le Marketo Engage synchronise automatiquement l’audience mise à jour dans vos applications AEC connectées. Utilisez-la pour tirer parti des cas d’orchestration, de reciblage, de suppression d’audiences, de personnalisation et d’utilisation de rapports multicanaux de l’Adobe dans votre pile technologique AEC.
* **[Synchronisation continue des Audiences avec Google, Facebook et LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)** : La synchronisation automatisée continue avec un réseau publicitaire peut être activée sur une liste statique, mettant à jour le réseau publicitaire à mesure que l’adhésion à la liste change sans que l’utilisateur n’ait à intervenir.
* **[Jetons pour les champs](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)** personnalisés des membres de Programme : Nous avons étendu les fonctionnalités de champ personnalisé des membres de programme pour prendre en charge la structure des jetons. Les marketeurs peuvent insérer des jetons de champs personnalisés de membres de programme dans des courriers électroniques, des landings page, des messages SMS, des notifications Push et des hameçons Web. Utilisez de nouveaux jetons dans les actions de flux de campagne pour modifier les valeurs des données, créer une tâche ou un moment intéressant.

## landings page et Forms {#landing-pages-and-forms}

* **API** de formulaire : Tirez parti des informations de piste ou déclenchez des campagnes de promotion tout en extrayant les données des formulaires non liés au marketing. Les formulaires non liés au marketing peuvent s’intégrer au Marketo Engage via l’API REST. La nouvelle API permet d’imiter l’envoi de Marketo Engage de formulaires avec toutes les fonctionnalités associées.
* **API** landings page : Rationalisez les workflows de modification et de traduction dans les applications intégrées grâce à la nouvelle API Landing page Prévisualisation. Les fournisseurs tiers peuvent désormais rendre des prévisualisations de landings page entièrement personnalisées sans se connecter au Marketo Engage.  L&#39;API Landing page Prévisualisation permet des workflows de modification et de localisation de bout en bout dans des applications intégrées tierces.

## Marketing par courriel {#email-marketing}

* **[Limites de récupération des objets personnalisés augmentées](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)** : Les développeurs de scripts Velocity de messagerie peuvent rapidement augmenter le nombre d’objets personnalisés à 100 par remplacement en libre-service. Les marketeurs peuvent accroître l’efficacité des campagnes dynamiques en accédant à un plus grand nombre d’objets personnalisés de premier et de second niveau.

## Intégration de la gestion de la relation client Salesforce {#salesforce-crm-integration}

* [Authentification](/help/marketo/product-docs/crm-sync/salesforce-sync/setting-up-oauth-2-0.md) CRM Salesforce : Le protocole OAuth 2.0 est disponible pour la synchronisation d&#39;opérations entre la gestion de la relation client Marketo Engage et Salesforce. Pour les nouveaux abonnés, cette option est activée par défaut. Les abonnés actuels peuvent demander cette fonctionnalité en contactant le service d’assistance marketing.
* [Tableau de bord](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md) de synchronisation de la gestion de la relation client Salesforce : Les administrateurs peuvent rapidement vérifier l’état de synchronisation de la gestion de la relation client Salesforce à partir du tableau de bord. Le délai du rapport de performance de synchronisation a été augmenté de 2 heures à 5 jours.
* **Exportation** des métadonnées : Amélioration de la prise en charge des attributs d’objet d’opportunité, des comptes nommés, des champs standard et personnalisés des membres de programme.

## Administration {#administration}

* **Mise à jour de la page** Mon compte : Consultez les informations essentielles sur l&#39;abonnement sur la page Mon compte. Les utilisateurs disposant de tous les niveaux d’accès peuvent vue le nom de l’abonnement, l’identifiant du centre de données et l’identifiant Munchkin.

**_Libération au cours du trimestre_**

Les fonctionnalités suivantes sont présentées sur un cycle non trimestriel et seront publiées au cours des prochains mois.

## Sales Insight {#sales-insight}

![(étoile)](assets/star-yellow.svg)

* **[Workflows de messagerie électronique de test améliorés (CRM Salesforce)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)** : Augmentez l&#39;efficacité de votre équipe commerciale grâce aux workflows électroniques de test Sales Insight améliorés. Les vendeurs peuvent envoyer des e-mails de test à certaines adresses électroniques avant d&#39;envoyer des e-mails en masse à 200 destinataires au maximum.
* **[Informations sur le statut du courriel (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)** : Les utilisateurs voient un message d’avertissement lorsqu’ils tentent d’envoyer un courrier électronique à un ID de courrier électronique non valide ou à une adresse électronique non enregistrée avant d’envoyer un courrier électronique.  Les états des diffusions électroniques peuvent être vérifiés dans l&#39;onglet Courriel de Sales Insight.
* **Envoyer des e-mails en masse à partir des  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) panneaux Comptable et  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) OpportunityPanels (Salesforce CRM)** : Améliorer l&#39;efficacité du workflow du vendeur et interagir avec une liste complète de contact de compte ou d&#39;opportunité en utilisant de nouvelles fonctionnalités d&#39;action en masse. Envoyez des courriers électroniques ou ajoutez des contacts aux campagnes des Marketo Engage en utilisant la nouvelle option de liste déroulante dans les onglets de compte ou d&#39;opportunité au lieu de travailler avec des contacts individuels. Ajoutez des contacts de compte à une liste de contrôle pour être averti lorsque les pistes deviennent actives.
* **[Sales Insight for Non Native Salesforce CRM Integrations](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)** : Les abonnements GA dotés d&#39;intégrations CRM Salesforce personnalisées peuvent installer le module Sales Insight et aider les équipes commerciales à établir des priorités et à interagir avec les pistes et opportunités les plus prometteuses.
* **[Améliorations](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)** des meilleurs paris : Contactez rapidement les pistes actives à partir de l&#39;onglet Meilleurs résultats en les envoyant par courriel ou en les ajoutant à un Campaign Marketo Engage. Vue d&#39;une piste dans le Marketo Engage ou l&#39;ajoutez à votre liste de contrôle. Les actions en masse et les options de tri sur l&#39;onglet Meilleurs paris vous permettent de gagner du temps et d&#39;améliorer l&#39;efficacité de l&#39;équipe commerciale.

## Connexion commerciale {#sales-connect}

![(étoile)](assets/star-yellow.svg)

* **Limitation de la connexion par courriel (BETA)** : Améliorez la délivrabilité de vos e-mails et redimensionnez votre communication commerciale 1:1 avec le contrôle des connexions par e-mail pour Sales Connect. Notre nouvelle technologie de limitation de vitesse gère automatiquement le délai d&#39;envoi des courriers électroniques pour créer des expériences homogènes pour les utilisateurs d&#39;Exchange et de Gmail. Réduire ou éliminer l&#39;utilisation des applications d&#39;envoi de courrier électronique en masse tierces.
* **Suivi des retours** de connexion par courriel : Découvrez la qualité des pistes et les performances des modèles de courrier électronique grâce au nouveau rapport de rebonds de courrier électronique. Les utilisateurs d’Exchange et de Gmail peuvent choisir de recevoir des notifications de rebonds qui seront cumulées au flux en direct, aux dossiers de courrier électronique, à l’analyse des modèles et à Campaign Analytics.
* **Configuration** de la page de profil : Gérez facilement les préférences des utilisateurs dans la nouvelle page de profil. Modifiez le mot de passe, modifiez les paramètres de géolocalisation et de langue et vérifiez les états des intégrations au même endroit.
* **Gestion** des modèles : Organisez les modèles d&#39;e-mail de vente en catégories avec une nouvelle fonction de glisser-déposer afin d&#39;accéder rapidement aux modèles appropriés et de réduire le temps de recherche.
* **Mises à jour** de l&#39;expérience utilisateur de Sales Connect : Personnalisez la mise en page de la grille Sales Connect en redimensionnant et en réordonnant les colonnes. Vos préférences d’affichage sont automatiquement enregistrées.

**_Annonces et dépréciations_**

* Tous les utilisateurs doivent effectuer la mise à niveau vers la dernière version de Sales Insight **avant le 15 janvier 2021**. Si vous n’avez pas effectué la mise à niveau, vous serez invité à le faire lors de votre connexion à l’application. Suivez les instructions [de ce guide](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). La version mise à jour comprend un correctif pour une vulnérabilité de sécurité identifiée. Le correctif a été initialement publié le 6 avril 2016. Remarque : **Les versions 1.4363 ou ultérieures** n&#39;ont pas besoin d&#39;effectuer une mise à niveau.
* L’obsolescence du service Form 1.0 entrera en vigueur dans la version de **mai 2021**. Le service Forms 1.0 est totalement obsolète, ce qui entraîne la perte de fonctionnalités de tous les actifs Forms 1.0 restants encore en cours d’utilisation. En outre, les soumissions de formulaires effectuées par des méthodes non prises en charge, telles que les POST de formulaire programmatique aux points de terminaison leadCapture/save et leadCapture/save2, seront rejetées. Pour plus d’informations et de correctifs, consultez [notre publication dans Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* En 2021, le Marketo Engage apportera des modifications à la structure des URL pour les ressources de landings page, de formulaires, d’images et de fichiers. Pour les abonnements Marketo Engage existants, nous commencerons le déploiement progressif le 1er avril 2021. D&#39;autres détails sur le calendrier de déploiement seront publiés en mars 2021. Pour plus d’informations sur la manière dont chaque type de ressource affecté va changer, consultez [notre publication dans Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinaire sur la version du produit_**

Vous souhaitez en savoir plus sur ces fonctionnalités et améliorations ? Veillez à [vous inscrire dès maintenant](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) pour vous joindre à nous le 21 janvier à 13h00 PT / 16h00 ET pour un webinaire en direct avec notre équipe produit afin de plonger plus profondément dans ces innovations.
