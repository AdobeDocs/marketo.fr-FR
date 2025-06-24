---
description: Notes De Mise À Jour - Janvier 2021 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Janvier 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# Notes De Mise À Jour : Janvier 2021 {#release-notes-jan-21}

Les fonctionnalités suivantes sont incluses dans la version de janvier 2021. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![(étoile)](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **15 janvier 2021**.

## Expérience utilisateur de nouvelle génération {#next-generation-user-experience}

* Prise en charge des espaces de travail : l’expérience client de nouvelle génération Marketo Engage associe l’aspect de Adobe Experience Cloud à des innovations de productivité pour aider les professionnels du marketing à travailler plus rapidement et plus intelligemment. Dans la dernière version, nous ajoutons une prise en charge complète des espaces de travail et des partitions, y compris la possibilité de partager des dossiers entre les espaces de travail. La zone de travail de droite propose un bouton bascule pour vous permettre de passer facilement d’une expérience ancienne à une nouvelle sans perdre de contexte. [Apprenez-en davantage](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) en consultant la FAQ sur l’expérience de nouvelle génération dans Marketing Nation.

## Personalization Multicanal {#multi-channel-personalization}

* **[Phase 3 de synchronisation des audiences Adobe Experience Cloud](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)** : la fonctionnalité de synchronisation des audiences Adobe Experience Cloud (AEC) prend désormais en charge la synchronisation continue et bidirectionnelle des audiences B2B de Marketo Engage vers d’autres applications AEC, y compris les offres de Adobe Experience Platform (AEP) telles que Real-time Customer Data Platform et Adobe Experience Platform Activation.  À mesure que des prospects sont ajoutés et supprimés à vos segments d’audience, Marketo Engage synchronise automatiquement l’audience mise à jour dans toutes vos applications AEC connectées. Utilisez-le pour tirer parti des cas d’utilisation d’Adobe en matière d’orchestration multicanal, de reciblage, de suppression d’audience, de personnalisation et de création de rapports dans votre tech stack AEC.
* **[Synchronisation continue de l’audience avec Google,  [!DNL Facebook] et [!DNL LinkedIn]](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)** : la synchronisation automatisée continue avec un réseau publicitaire peut être activée sur une liste statique, ce qui met à jour le réseau publicitaire à mesure que l’appartenance à la liste change sans nécessiter d’intervention de l’utilisateur.
* **[Jetons pour les champs personnalisés des membres de programme](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)** : nous avons étendu les fonctionnalités de champ personnalisé des membres de programme pour prendre en charge le framework de jetons. Les marketeurs peuvent insérer des jetons de champs personnalisés de membres de programme dans les e-mails, les landing pages, les SMS, les notifications push et les webhooks. Utilisez les nouveaux jetons dans les actions de flux de campagne pour modifier les valeurs des données, créer une tâche ou un moment intéressant.

## Pages de destination et formulaires {#landing-pages-and-forms}

* **API Form** : extrayez des informations de prospect ou déclenchez des campagnes d’éducation lors de l’extraction de données à partir de formulaires non Marketo. Les formulaires non Marketo peuvent s’intégrer à Marketo Engage via l’API REST. La nouvelle API permet d’imiter l’envoi de formulaire Marketo Engage avec toutes les fonctionnalités associées.
* **API Landing Pages** : rationalisez les workflows d’édition et de traduction dans les applications intégrées avec la nouvelle API d’aperçu de page de destination. Les fournisseurs tiers peuvent désormais générer des aperçus entièrement personnalisés des pages de destination sans se connecter à Marketo Engage.  L’API de prévisualisation de la page de destination permet des workflows de modification et de localisation de bout en bout dans des applications intégrées tierces.

## Marketing par e-mail {#email-marketing}

* **[Limites de récupération d’objets personnalisés augmentées](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)** : les développeurs de script de vélocité d’e-mail peuvent rapidement augmenter le nombre d’objets personnalisés à 100 par remplacement en libre-service. Les marketeurs peuvent augmenter l&#39;efficacité des campagnes intelligentes en accédant à un plus grand nombre d&#39;objets personnalisés de premier et deuxième niveau.

## Intégration [!DNL Salesforce] CRM {#salesforce-crm-integration}

* [[!DNL Salesforce] Authentification CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md) : le protocole OAuth 2.0 est disponible pour la synchronisation des opérations entre Marketo Engage et [!DNL Salesforce] CRM. Pour les nouveaux abonnés, cette option est activée par défaut. Les abonnés actuels peuvent demander cette fonctionnalité en contactant le support technique de Marketo.
* [[!DNL Salesforce] Tableau de bord de synchronisation CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md) : les administrateurs peuvent rapidement consulter [!DNL Salesforce] statut de synchronisation CRM à partir du tableau de bord. La durée du rapport de performances de synchronisation a été augmentée de 2 heures à 5 jours.
* **Exportation de métadonnées** : amélioré pour prendre en charge les attributs d’objet d’opportunité, les comptes nommés, les champs standard et personnalisés des membres du programme.

## Administration {#administration}

* **Page Mon compte mise à jour** : consultez les informations essentielles relatives à l’abonnement sur la page Mon compte. Les utilisateurs disposant de n’importe quel niveau d’accès peuvent afficher le nom de l’abonnement, l’identifiant du centre de données et l’identifiant du [!DNL Munchkin].

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes font l’objet d’un cycle non trimestriel et seront publiées au cours des prochains mois.

## [!DNL Sales Insight] {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **[Workflows d’e-mail de test améliorés ([!DNL Salesforce] CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)** : améliorez l’efficacité de votre équipe de vente grâce à des workflows d’e-mail de test [!DNL Sales Insight] améliorés. Les vendeurs peuvent envoyer des e-mails de test à des adresses e-mail sélectionnées avant d’envoyer des e-mails en masse à 200 destinataires maximum.
* **[Informations sur le statut des e-mails ([!DNL Salesforce] CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)** : les utilisateurs voient un message d’avertissement lorsqu’ils essaient d’envoyer un e-mail à un ID d’e-mail non valide ou à une adresse e-mail de désabonnement avant d’envoyer un e-mail.  Vous pouvez consulter les statuts de diffusion des e-mails dans l’onglet E-mail de [!DNL Sales Insight].
* **Envoi d’e-mails en masse depuis les panneaux [Compte](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) et [Opportunité](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) ([!DNL Salesforce] CRM)** : améliorez l’efficacité du workflow du vendeur et interagissez avec l’ensemble de la liste de contacts d’un compte ou d’une opportunité à l’aide de nouvelles fonctionnalités d’action en masse. Envoyez des e-mails ou ajoutez des contacts aux campagnes Marketo Engage à l’aide de la nouvelle option déroulante dans les onglets compte ou opportunité au lieu de travailler avec des contacts individuels. Ajouter des contacts de compte à une watchlist pour être averti lorsque les leads deviennent chauds.
* **[[!DNL Sales Insight] pour les intégrations CRM  [!DNL Salesforce]  natives](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)** : les abonnements GA avec des intégrations CRM Salesforce personnalisées peuvent installer le package [!DNL Sales Insight] et aider les équipes commerciales à prioriser et à interagir avec les prospects et les opportunités les plus prometteuses.
* **[Améliorations des meilleurs résultats](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)** : contactez rapidement les prospects de l’onglet Meilleurs résultats en les envoyant par e-mail ou en les ajoutant à une campagne Marketo Engage. Affichez un prospect dans Marketo Engage ou ajoutez-le à votre liste de surveillance. Les actions en masse et les options de tri sur l’onglet [!UICONTROL &#x200B; Meilleurs résultats &#x200B;] permettent de gagner du temps et d’améliorer l’efficacité de l’équipe commerciale.

## [!DNL Sales Connect] {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Limitation de la connexion aux e-mails (BETA)**: améliorez la délivrabilité de vos e-mails et mettez à l’échelle votre communication commerciale 1:1 à l’aide de la limitation de la connexion aux e-mails pour [!DNL Sales Connect]. Notre nouvelle technologie de limitation gère automatiquement le délai d’envoi des e-mails afin de créer des expériences transparentes pour les utilisateurs d’[!DNL Exchange] et de Gmail. Réduire ou éliminer l’utilisation d’applications tierces d’envoi d’e-mails en masse
* insight **Suivi des rebonds de connexions aux e-mails** : gagnez en qualité de lead et en performances de modèle d’e-mail avec le nouveau rapport sur les rebonds d’e-mails. Les utilisateurs d’[!DNL Exchange] et de Gmail peuvent choisir de recevoir des notifications de rebond qui seront cumulées dans les flux en direct, les dossiers d’e-mails, les modèles d’analyse et Campaign Analytics.
* **Configuration de la page de profil** : gérez facilement les préférences utilisateur dans la nouvelle page de profil. Modifiez le mot de passe, la géolocalisation et les paramètres de langue, ainsi que les statuts d’intégration à un seul endroit.
* **Gestion des modèles** : organisez les modèles d’e-mail de vente en catégories à l’aide d’une nouvelle fonctionnalité de glisser-déposer afin d’assurer un accès rapide aux modèles pertinents et de réduire le temps de recherche.
* **[!DNL Sales Connect]mises à jour de l’expérience utilisateur** : personnalisez [!DNL Sales Connect] disposition de grille en redimensionnant et en réorganisant les colonnes. Vos préférences de visionnage sont automatiquement enregistrées.

**_Annonces et abandons_**

* Tous les utilisateurs doivent effectuer la mise à niveau vers la dernière version de Sales Insight **avant le 15 janvier 2021**. Si vous n’avez pas terminé la mise à niveau, vous serez invité à le faire lors de la connexion à l’application. Suivez les instructions [dans ce guide](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). La version mise à jour comprend un correctif pour une vulnérabilité de sécurité identifiée. Le correctif a été initialement publié le 6 avril 2016. Remarque : les **versions 1.4363 ou ultérieures** n’ont pas besoin d’effectuer de mise à niveau.
* L’obsolescence du service Form 1.0 prendra effet dans la version **mai 2021**. Le service Forms 1.0 sera complètement obsolète, ce qui entraînera la perte de fonctionnalités des ressources Forms 1.0 restantes encore en cours d’utilisation. En outre, les envois de formulaire effectués par le biais de méthodes non prises en charge, telles que les publications de formulaire programmatiques aux points d’entrée leadCapture/save et leadCapture/save2, seront rejetés. Pour plus d&#39;informations et de mesures correctives, consultez [notre article dans Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* En 2021, Marketo Engage apportera des modifications à la structure de l’URL pour les pages de destination, les formulaires, les images et les fichiers. Pour les abonnements Marketo Engage existants, le déploiement progressif commencera le 1er avril 2021. De plus amples détails sur le calendrier de déploiement seront publiés en mars 2021. Pour plus d’informations sur les modifications apportées à chaque type de ressource affecté, reportez-vous à [notre article dans Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinaire de mise à jour du produit_**

Vous souhaitez en savoir plus sur ces fonctionnalités et améliorations ? N’oubliez pas de vous [inscrire dès maintenant](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) pour vous joindre à nous le 21 janvier à 13 h (heure de Paris) / 16 h (heure de Paris) pour un webinaire en direct avec notre équipe produit afin d’approfondir l’étude de ces innovations.
