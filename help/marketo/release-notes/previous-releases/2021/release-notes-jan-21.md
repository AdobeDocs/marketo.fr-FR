---
description: Notes de mise à jour - Jan 2021 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Jan 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 1%

---

# Notes de mise à jour : janvier 2021 {#release-notes-jan-21}

Les fonctionnalités suivantes sont incluses dans la version du 21 janvier. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![(étoile)](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **15 janvier 2021**.

## Expérience utilisateur de nouvelle génération {#next-generation-user-experience}

* Prise en charge des espaces de travail : l’expérience utilisateur de nouvelle génération du Marketo Engage associe l’aspect et l’aspect de Adobe Experience Cloud aux innovations en matière de productivité afin d’aider les professionnels du marketing à travailler plus rapidement et plus intelligemment. Dans la dernière version, nous ajoutons une prise en charge complète des espaces de travail et des partitions, y compris la possibilité de partager des dossiers entre les espaces de travail. Le canevas de droite propose un bouton bascule pour vous permettre de passer facilement d’une expérience à l’autre sans perdre de contexte. [En savoir plus](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) à partir de la FAQ sur l’expérience de nouvelle génération sur Marketing Nation.

## Personalization multicanal {#multi-channel-personalization}

* **[Phase de synchronisation de l’audience Adobe Experience Cloud 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)** : la fonctionnalité de synchronisation de l’audience Adobe Experience Cloud (AEC) existante prend désormais en charge la synchronisation continue de l’audience B2B bidirectionnelle de Marketo Engage vers d’autres applications AEC, y compris les offres Adobe Experience Platform (AEP) telles que Real-time Customer Data Platform et Adobe Experience Platform Activation.  À mesure que des pistes sont ajoutées et supprimées dans vos segments d’audience, Marketo Engage synchronise automatiquement l’audience mise à jour dans vos applications AEC connectées. Utilisez-le pour tirer parti des cas d’utilisation d’orchestration, de reciblage, de suppression d’audience, de personnalisation et de création de rapports multicanaux d’Adobe dans votre tech stack AEC.
* **[Synchronisation continue de l’audience avec Google, Facebook et LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)** : la synchronisation automatisée continue avec un réseau publicitaire peut être activée sur une liste statique, mettant à jour le réseau publicitaire en tant que modification de l’adhésion à la liste sans nécessiter l’intervention de l’utilisateur.
* **[Jetons pour les champs personnalisés des membres du programme](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)** : nous avons étendu les fonctionnalités de champ personnalisé des membres du programme pour prendre en charge la structure de jeton. Les marketeurs peuvent insérer des jetons de champs personnalisés des membres du programme dans les emails, les landing pages, les SMS, les notifications push et les webhooks. Utilisez de nouveaux jetons dans les actions de flux de campagne pour modifier les valeurs des données, créer une tâche ou un moment intéressant.

## Pages de destination et formulaires {#landing-pages-and-forms}

* **API de formulaire** : extraire des informations de piste ou déclencher des campagnes de sensibilisation tout en extrayant des données de formulaires non Marketo. Les formulaires non Marketo peuvent s’intégrer à Marketo Engage via l’API REST. La nouvelle API permet d’imiter l’envoi de formulaires de Marketo Engage avec toutes les fonctionnalités associées.
* **API Pages d’entrée** : simplifiez les processus d’édition et de traduction dans les applications intégrées avec la nouvelle API d’aperçu de page d’entrée. Les fournisseurs tiers peuvent désormais générer des aperçus entièrement personnalisés des landing pages sans se connecter à Marketo Engage.  L’API d’aperçu de page d’entrée permet des processus de modification et de localisation de bout en bout dans des applications tierces intégrées.

## Marketing par e-mail {#email-marketing}

* **[Limites de récupération d’objets personnalisés augmentées](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)** : les développeurs de script Velocity de courrier électronique peuvent rapidement augmenter le nombre d’objets personnalisés à 100 par remplacement en libre-service. Les marketeurs peuvent accroître l’efficacité des campagnes intelligentes en accédant à un plus grand nombre d’objets personnalisés de premier et de second niveau.

## Intégration de SalesForce CRM {#salesforce-crm-integration}

* [Authentification CRM Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md) : le protocole OAuth 2.0 est disponible pour la synchronisation des opérations entre le CRM Marketo Engage et Salesforce. Pour les nouveaux abonnés, cette option est activée par défaut. Les abonnés actuels peuvent demander cette fonctionnalité en contactant l’assistance de Marketo.
* [Tableau de bord de synchronisation CRM Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md) : les administrateurs peuvent rapidement consulter l’état de synchronisation CRM Salesforce à partir du tableau de bord. La durée du rapport de synchronisation des performances est passée de 2 heures à 5 jours.
* **Exportation de métadonnées** : améliorée pour la prise en charge des attributs d’objet d’opportunité, des comptes nommés, des champs standard et personnalisés des membres du programme.

## Administration {#administration}

* **Mise à jour de la page Mon compte** : consultez les informations d’abonnement essentielles sur la page Mon compte. Les utilisateurs disposant de tout niveau d’accès peuvent afficher le nom de l’abonnement, l’identifiant du centre de données et l’identifiant Munchkin.

**_Mise à jour tout au long du trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

## Sales Insight {#sales-insight}

![(star)](assets/yellow-star.png)

* **[Processus de courrier électronique de test amélioré (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)** : augmentez l’efficacité de votre équipe commerciale grâce aux workflows de courrier électronique de test Sales Insight améliorés. Les vendeurs peuvent envoyer des emails de test à des adresses email sélectionnées avant d’envoyer des emails en bloc à 200 destinataires maximum.
* **[Statistiques dans l’état de l’email (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)** : les utilisateurs voient un message d’avertissement lorsqu’ils tentent d’envoyer un email à un ID d’email non valide ou à une adresse email désabonnée avant d’envoyer un email.  Les statuts de diffusion des emails peuvent être vérifiés dans l’onglet Email de Sales Insight.
* **Envoyer des emails en bloc à partir des [panneaux Compte](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) et [Opportunité](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) (Salesforce CRM)** : améliorez l’efficacité du workflow du vendeur et écrivez avec une liste complète de contacts de compte ou d’opportunité en utilisant de nouvelles fonctionnalités d’action en bloc. Envoyez des emails ou ajoutez des contacts à des campagnes Marketo Engage à l’aide de la nouvelle option déroulante des onglets Compte ou Opportunités au lieu de travailler avec des contacts individuels. Ajoutez des contacts de compte à une liste de contrôle afin de les avertir lorsque les prospects deviennent chauds.
* **[Sales Insight for Non Native Salesforce CRM Integrations](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)** : les abonnements GA avec des intégrations CRM Salesforce personnalisées peuvent installer le package Sales Insight et aider les équipes commerciales à prioriser et à interagir avec les prospects et opportunités les plus prometteurs.
* **[Meilleures améliorations des paris](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)** : contactez rapidement les prospects de l’onglet Meilleurs paris en les envoyant par courrier électronique ou en les ajoutant à une campagne Marketo Engage. Affichez une piste dans Marketo Engage ou ajoutez-la à votre liste de contrôle. Les actions en bloc et les options de tri sur l’onglet Meilleurs paris vous permettent de gagner du temps et d’améliorer l’efficacité de l’équipe commerciale.

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **Limitation de la connexion par e-mail (BETA)** : améliorez la délivrabilité de vos e-mails et adaptez votre communication commerciale 1:1 avec limitation de la connexion par e-mail pour Sales Connect. Notre nouvelle technologie de ralentissement gère automatiquement le délai d’envoi des emails afin de créer des expériences transparentes pour les utilisateurs d’Exchange et de Gmail. Diminuez ou supprimez l’utilisation des applications tierces d’envoi de courriers électroniques en masse.
* **Email Connection Bounce Tracking** : profitez d’informations sur la qualité des prospects et les performances des modèles d’email avec le nouveau rapport de rebond des emails. Les utilisateurs d’Exchange et de Gmail peuvent choisir de recevoir des notifications de rebond qui seront cumulées au flux en direct, aux dossiers d’e-mail, à l’analyse des modèles et à Campaign Analytics.
* **Configuration de la page de profil** : gérez facilement les préférences de l’utilisateur dans la nouvelle page de profil. Modifiez le mot de passe, modifiez la géolocalisation et les paramètres de langue, puis passez en revue les états des intégrations au même endroit.
* **Gestion des modèles** : organisez les modèles d’email de vente en catégories avec une nouvelle fonctionnalité de glisser-déposer pour assurer un accès rapide aux modèles pertinents et réduire le temps de recherche.
* **Mises à jour de l’expérience utilisateur de Sales Connect** : personnalisez la disposition de la grille Sales Connect en redimensionnant et en réorganisant les colonnes. Vos préférences d’affichage sont automatiquement enregistrées.

**_Annonces et obsolescences_**

* Tous les utilisateurs doivent effectuer la mise à niveau vers la dernière version de Sales Insight **avant le 15 janvier 2021**. Si vous n’avez pas terminé la mise à niveau, vous serez invité à le faire lorsque vous vous connecterez à l’application. Suivez les instructions [de ce guide](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). La version mise à jour comprend un correctif pour une vulnérabilité de sécurité identifiée. Le correctif a été publié à l&#39;origine le 6 avril 2016. Remarque : **Les versions 1.4363 ou ultérieures** n’ont pas besoin d’effectuer une mise à niveau.
* L’obsolescence du service Form 1.0 entrera en vigueur dans la version de **mai 2021**. Le service Forms 1.0 sera totalement obsolète, ce qui entraîne la perte de fonctionnalités de toutes les ressources Forms 1.0 restantes toujours utilisées. En outre, les envois de formulaire effectués par le biais de méthodes non prises en charge, telles que les POST de formulaire programmatique vers les points de terminaison leadCapture/save et leadCapture/save2, seront rejetés. Pour plus d’informations et de correctifs, reportez-vous à [notre publication dans Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* En 2021, Marketo Engage modifiera la structure des URL des landing pages, des formulaires, des images et des fichiers actifs. Pour les abonnements de Marketo Engage existants, nous allons commencer le déploiement progressif le 1er avril 2021. D’autres détails sur la date de déploiement seront publiés en mars 2021. Pour plus d’informations sur la modification de chaque type de ressource affecté, reportez-vous à [notre publication dans Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinaire sur la version du produit_**

Vous souhaitez en savoir plus sur ces fonctionnalités et améliorations ? Veillez à [vous inscrire maintenant](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) pour vous joindre à nous le 21 janvier à 13h00 PT / 16h00 ET pour un webinaire en direct avec notre équipe produit afin de plonger plus profondément dans ces innovations.
