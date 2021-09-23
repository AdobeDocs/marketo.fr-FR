---
description: Notes de mise à jour - Jan 2021 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Jan 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 1%

---

# Notes de mise à jour : Jan 2021 {#release-notes-jan-21}

Les fonctionnalités suivantes sont incluses dans la version du 21 janvier. Vérifiez la disponibilité de votre édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![(star)](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **15 janvier 2021**.

## Expérience utilisateur de nouvelle génération {#next-generation-user-experience}

* Prise en charge des espaces de travail : L’expérience utilisateur de nouvelle génération Marketo Engage rassemble l’aspect et l’aspect de Adobe Experience Cloud avec des innovations en matière de productivité afin d’aider les professionnels du marketing à travailler plus rapidement et plus intelligemment. Dans la dernière version, nous ajoutons une prise en charge complète des espaces de travail et des partitions, y compris la possibilité de partager des dossiers entre les espaces de travail. Le canevas de droite propose un bouton bascule pour vous permettre de passer facilement d’une expérience à l’autre sans perdre de contexte. [Pour en savoir ](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) plus, consultez la FAQ sur l’expérience de nouvelle génération dans Marketing Nation.

## Personnalisation multicanal {#multi-channel-personalization}

* **[Phase](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)** de synchronisation de l’audience Adobe Experience Cloud : La fonctionnalité de synchronisation d’audience Adobe Experience Cloud (AEC) existante prend désormais en charge la synchronisation d’audience B2B continue et bidirectionnelle de Marketo Engage vers d’autres applications AEC, y compris les offres Adobe Experience Platform (AEP) telles que la plateforme de données client en temps réel et l’activation de Adobe Experience Platform.  À mesure que des pistes sont ajoutées et supprimées dans vos segments d’audience, Marketo Engage synchronise automatiquement l’audience mise à jour dans vos applications AEC connectées. Utilisez-le pour tirer parti des cas d’utilisation d’orchestration, de reciblage, de suppression d’audience, de personnalisation et de création de rapports multicanaux d’Adobe dans votre pile technologique AEC.
* **[Synchronisation continue de l’audience avec Google, Facebook et LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)** : La synchronisation automatisée continue avec un réseau publicitaire peut être activée sur une liste statique, mettant à jour le réseau publicitaire à mesure que l’adhésion à la liste change sans nécessiter l’intervention de l’utilisateur.
* **[Jetons pour les champs personnalisés des membres du programme](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)** : Nous avons étendu les fonctionnalités de champ personnalisé des membres du programme pour prendre en charge le framework de jeton. Les marketeurs peuvent insérer des jetons de champs personnalisés des membres du programme dans les emails, les landing pages, les SMS, les notifications push et les webhooks. Utilisez de nouveaux jetons dans les actions de flux de campagne pour modifier les valeurs des données, créer une tâche ou un moment intéressant.

## Pages de destination et formulaires {#landing-pages-and-forms}

* **API** de formulaire : Extrayez les informations de piste ou déclenchez des campagnes d’enrichissement tout en extrayant des données des formulaires non Marketo. Les formulaires non Marketo peuvent s’intégrer à Marketo Engage via l’API REST. La nouvelle API permet d’imiter l’envoi de formulaires de Marketo Engage avec toutes les fonctionnalités associées.
* **API** de pages d’entrée : Rationalisez les processus d’édition et de traduction dans les applications intégrées à l’aide de la nouvelle API d’aperçu de page d’entrée. Les fournisseurs tiers peuvent désormais générer des aperçus entièrement personnalisés des landing pages sans se connecter à Marketo Engage.  L’API d’aperçu de page d’entrée permet des processus de modification et de localisation de bout en bout dans des applications tierces intégrées.

## Marketing par e-mail {#email-marketing}

* **[Limites de récupération d’objets personnalisés augmentées](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)** : Les développeurs de scripts Velocity de courrier électronique peuvent rapidement augmenter le nombre d’objets personnalisés à 100 par le biais d’un remplacement en libre-service. Les marketeurs peuvent accroître l’efficacité des campagnes intelligentes en accédant à un plus grand nombre d’objets personnalisés de premier et de second niveau.

## Intégration de SalesForce CRM {#salesforce-crm-integration}

* [Authentification](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md) CRM Salesforce : Le protocole OAuth 2.0 est disponible pour la synchronisation des opérations entre Marketo Engage et Salesforce CRM. Pour les nouveaux abonnés, cette option est activée par défaut. Les abonnés actuels peuvent demander cette fonctionnalité en contactant l’assistance de Marketo.
* [Tableau de bord de synchronisation CRM Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md) : Les administrateurs peuvent rapidement consulter l’état de synchronisation CRM Salesforce à partir du tableau de bord. La durée du rapport de synchronisation des performances est passée de 2 heures à 5 jours.
* **Exportation des métadonnées** : Amélioration afin de prendre en charge les attributs d’objet d’opportunité, les comptes nommés, les champs standard et personnalisés des membres du programme.

## Administration {#administration}

* **Mise à jour de la page Mon compte** : Consultez les informations d’abonnement essentielles sur la page Mon compte . Les utilisateurs disposant de tous les niveaux d’accès peuvent afficher le nom de l’abonnement, l’identifiant du centre de données et l’identifiant Munchkin.

**_Sortie pendant tout le trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

## Sales Insight {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **[Amélioration des workflows de test des emails (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)** : Augmentez l’efficacité de votre équipe commerciale grâce aux workflows de messagerie de test Sales Insight améliorés. Les vendeurs peuvent envoyer des emails de test à des adresses email sélectionnées avant d’envoyer des emails en bloc à 200 destinataires maximum.
* **[Statistiques sur l’état des emails (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Un message d’avertissement s’affiche lorsqu’un utilisateur tente d’envoyer un courrier électronique à un ID de message électronique non valide ou à une adresse électronique désabonnée avant d’envoyer un courrier électronique.  Les statuts de diffusion des emails peuvent être vérifiés dans l’onglet Email de Sales Insight.
* **Envoyer des emails en bloc à partir de  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) Accountability and  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) OpportunityPanels (Salesforce CRM)** : Améliorez l’efficacité du workflow du vendeur et interagissez avec une liste complète de contacts de compte ou d’opportunité en utilisant de nouvelles fonctionnalités d’action en bloc. Envoyez des emails ou ajoutez des contacts à des campagnes Marketo Engage à l’aide de la nouvelle option déroulante des onglets Compte ou Opportunités au lieu de travailler avec des contacts individuels. Ajoutez des contacts de compte à une liste de contrôle afin de les avertir lorsque les prospects deviennent chauds.
* **[Sales Insight for Non Native Salesforce CRM Integrations](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)** : Les abonnements GA avec des intégrations CRM Salesforce personnalisées peuvent installer le package Sales Insight et aider les équipes commerciales à hiérarchiser et à interagir avec les prospects et opportunités les plus prometteurs.
* **[Meilleures améliorations des](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)** paris : Contactez rapidement les prospects à partir de l&#39;onglet Meilleurs paris en les envoyant par email ou en les ajoutant à une campagne Marketo Engage. Affichez une piste dans Marketo Engage ou ajoutez-la à votre liste de contrôle. Les actions en bloc et les options de tri sur l’onglet Meilleurs paris vous permettent de gagner du temps et d’améliorer l’efficacité de l’équipe commerciale.

## SalesConnect {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Limitation de la connexion par e-mail (version BÊTA)** : Améliorez la délivrabilité de vos emails et adaptez votre communication commerciale 1:1 avec le contrôle des connexions par e-mail pour Sales Connect. Notre nouvelle technologie de ralentissement gère automatiquement le délai d’envoi des emails afin de créer des expériences transparentes pour les utilisateurs d’Exchange et de Gmail. Réduire ou éliminer l’utilisation des applications tierces d’envoi de courriers électroniques en masse.
* **Email Connection Bounce Tracking** : Découvrez les performances des modèles de courrier électronique et de la qualité des prospects grâce au nouveau rapport de rebond des emails. Les utilisateurs d’Exchange et de Gmail peuvent choisir de recevoir des notifications de rebond qui seront cumulées au flux en direct, aux dossiers d’e-mail, à l’analyse des modèles et à Campaign Analytics.
* **Configuration de la page de profil** : Gérez facilement les préférences de l’utilisateur dans la nouvelle page de profil. Modifiez le mot de passe, modifiez la géolocalisation et les paramètres de langue, puis passez en revue les états des intégrations au même endroit.
* **Gestion des modèles** : Organisez les modèles d’email de vente en catégories avec une nouvelle fonction glisser-déposer afin d’accéder rapidement aux modèles pertinents et de réduire le temps de recherche.
* **Mises à jour de l’expérience utilisateur de Sales Connect** : Personnalisez la mise en page de la grille Sales Connect en redimensionnant et en réorganisant les colonnes. Vos préférences d’affichage sont automatiquement enregistrées.

**_Annonces et obsolescences_**

* Tous les utilisateurs doivent effectuer la mise à niveau vers la dernière version de Sales Insight **avant le 15 janvier 2021**. Si vous n’avez pas terminé la mise à niveau, vous serez invité à le faire lorsque vous vous connecterez à l’application. Suivez les instructions [de ce guide](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). La version mise à jour comprend un correctif pour une vulnérabilité de sécurité identifiée. Le correctif a été initialement publié le 6 avril 2016. Remarque : **Les versions 1.4363 ou ultérieures** n’ont pas besoin d’effectuer une mise à niveau.
* L’obsolescence du service Form 1.0 entrera en vigueur dans la version de **mai 2021**. Le service Forms 1.0 sera totalement obsolète, ce qui entraîne la perte de fonctionnalités de toutes les ressources Forms 1.0 restantes toujours utilisées. En outre, les envois de formulaire effectués par le biais de méthodes non prises en charge, telles que les POST de formulaire programmatique vers les points de terminaison leadCapture/save et leadCapture/save2, seront rejetés. Pour plus d’informations et de correctifs, reportez-vous à [notre publication dans Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* En 2021, Marketo Engage modifiera la structure des URL des landing pages, des formulaires, des images et des fichiers actifs. Pour les abonnements de Marketo Engage existants, nous allons commencer le déploiement progressif le 1er avril 2021. D’autres détails sur la date de déploiement seront publiés en mars 2021. Pour plus d’informations sur la modification de chaque type de ressource affecté, reportez-vous à [notre publication dans Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinaire sur la version du produit_**

Vous souhaitez en savoir plus sur ces fonctionnalités et améliorations ? Veillez à [vous inscrire maintenant](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) pour vous joindre à nous le 21 janvier à 13h00 PT / 16h00 ET pour un webinaire en direct avec notre équipe produit afin de découvrir plus en détail ces innovations.
