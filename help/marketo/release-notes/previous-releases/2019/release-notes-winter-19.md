---
unique-page-id: 17727823
description: Notes De Mise À Jour - Hiver 19 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Hiver 19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 3%

---

# Notes de mise à jour : hiver 19 {#release-notes-winter}

Les fonctionnalités suivantes sont incluses dans la version d’hiver 19. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

Cliquez sur les liens de titre pour consulter les articles détaillés de chaque fonctionnalité, le cas échéant.

>[!NOTE]
>
>[!DNL Facebook] nécessite désormais un compte Business Manager pour tirer parti de votre intégration d’audience personnalisée. Votre service [!DNL Facebook] LaunchPoint *doit* être associé à un compte Business Manager ou **votre intégration ne fonctionnera plus après le 14 janvier 2019**. Pour configurer un compte Business Manager, reportez-vous à [[!DNL Facebook] Aide](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft incite tous les clients en ligne à effectuer une mise à niveau vers la dernière version de [!DNL Microsoft Dynamics]. Si vous intégrez votre instance Marketo à [!DNL Dynamics Online], vous devrez effectuer la [mise à niveau vers la dernière version de la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) avant le 31 **janvier 2019** pour vous assurer que votre intégration continuera à fonctionner.

>[!NOTE]
>
>Marketo met à niveau la version OAuth de 1.0 vers 2.0 pour GoToWebinar. La prise en charge d’OAuth 1.0 sera abandonnée en janvier 2019. Si vous êtes un client GoToWebinar, vous devrez réauthentifier vos connexions via LaunchPoint (dans la zone d’administration) d’ici le **31 janvier 2019** pour vous assurer que votre intégration continuera de fonctionner. Pour plus de détails, reportez-vous à notre [page Communauté](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Améliorations principales de la plateforme {#core-platform-enhancements}

**[Email CC pour les e-mails Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Ajoutez jusqu’à cinq adresses Cc par destinataire sur les e-mails envoyés via Marketo. 

**API**

* **Prise en charge de domaines multi-marques pour l’API de ressources :** l’approbation et le clonage des ressources produisent les mêmes résultats dans l’API et l’interface utilisateur.
* **Prise en charge de la fonctionnalité CC par e-mail pour l’API de ressources** : les utilisateurs qui clonent, approuvent et traitent des e-mails via l’API conserveront la parité avec les paramètres de l’interface utilisateur.

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Mode API uniquement** : les utilisateurs peuvent désormais déterminer quand et comment effectuer le suivi des membres de leur base de données en permettant aux applications web monopages d’appeler explicitement lorsqu’ils souhaitent enregistrer une visite de page web au lieu de compter sur le suivi automatique de Marketo.
* **Gestion des processus d’opt-out** : gérez facilement les processus d’opt-out en faisant correspondre le domaine du cookie d’opt-out avec le domaine du cookie de suivi [!DNL Munchkin].
* **Paramètre de décision au niveau du domaine** : les domaines à deux lettres (c’est-à-dire « [website.io](https://website.io) ») feront automatiquement l’objet d’un suivi dans Marketo sans exigences de configuration supplémentaires.

## Marketo Sales Engage {#marketo-sales-engage}

* **[!DNL Salesforce]profil personnalisé** : Sales Engage prend désormais en charge un nombre illimité de profils personnalisés.

* Personnalisation de l’**[!DNL Salesforce]: en supprimant les champs d’activité personnalisés non critiques** les utilisateurs et les utilisatrices peuvent configurer plus efficacement Sales Engage dans la plateforme CRM.
* **Service de messagerie électronique** : bénéficiez d&#39;une meilleure délivrabilité ainsi que d&#39;un meilleur suivi des réponses, de fonctionnalités de messagerie planifiée et de fonctionnalités de messagerie en masse en vous connectant à [!DNL Microsoft Outlook] (soit via Office365, soit On-Prem via l&#39;onglet Connexion par e-mail).
* **Nouveaux paramètres d’administration** : deux pages d’administration ont été ajoutées pour optimiser votre instance Sales Engage

   * _Team Management_ prend en charge un processus de configuration de compte transparent en permettant aux administrateurs de modifier les abonnements et les équipes.
   * _Paramètres d’administration Salesforce_ aide les équipes à configurer leur synchronisation SFDC plus rapidement et plus facilement que jamais auparavant.

* **Module externe OWA pour[!DNL Windows]** : avec un seul module complémentaire, tous les clients [!DNL Windows Office365] seront pris en charge dans Sales Engage, ce qui permet d’utiliser le flux en direct dans Outlook. Le nouveau plug-in sera disponible dans la boutique Microsoft.
* **Activités de promotion** : synchronisez Sales Engage à la plateforme Marketo de base pour tirer parti des informations marketing en temps réel.

## [!DNL Marketo Sky] {#marketo-sky}

>[!NOTE]
>
>Les publications de [!DNL Marketo Sky] se produisent à une cadence plus fréquente. Les fonctionnalités et améliorations suivantes devraient être publiées vers la fin du 4e trimestre et le début du 1er trimestre. Pour plus d’informations et de mises à jour, consultez notre [documentation Sky](https://help.marketo.com/).

* **Expérience par défaut facultative** : les utilisateurs de Marketo peuvent définir [!DNL Marketo Sky] comme expérience par défaut s’ils ont reçu l’accès d’un administrateur.

* **Mon Marketo repensé** : personnalisez votre expérience en ajoutant des widgets qui fournissent des informations essentielles, des notifications et des liens vers les zones que vous visitez le plus souvent.

* **Pages de détails et vues de liste de Design Studio** : bénéficiez d’un niveau accru d’organisation et de précision grâce à des vues de liste filtrables et interrogeables des e-mails, des pages de destination et des formulaires. Les pages Détails des ressources fournissent des informations clés sur chaque ressource, notamment les programmes qui l’utilisent, le nombre de fragments de code utilisés, etc.

* **Recherche globale** : Marketo offre désormais une fonction de recherche globale plus rapide et plus robuste sur l’ensemble de la plateforme. Les requêtes de recherche s’exécutent désormais sur tous les espaces de travail accessibles et peuvent rechercher des ressources (actives et archivées), des libellés, des campagnes et des programmes. Les résultats de la recherche sont fournis via une superposition et chaque résultat inclut son journal d’emplacement de fichier pour spécifier l’emplacement de la ressource.

* **Interface utilisateur améliorée** : nouvelles icônes, modèles et boutons, ainsi qu’une nouvelle palette de couleurs pour refléter le renouvellement de notre marque et [!DNL Marketo Sky] rendre encore plus époustouflant et fonctionnel.

* **Améliorations de l’utilisation du programme de messagerie électronique** : nous continuons à progresser vers la parité des fonctionnalités du programme de messagerie entre notre plateforme Marketo Lead Management classique et la nouvelle expérience [!DNL Marketo Sky].
* **Programmes Event-With-Webinar** : les programmes Event-With-Webinar sont désormais disponibles dans [!DNL Marketo Sky] (remarque : seul GoToWebinar sera pris en charge dans cette version, avec d’autres intégrations établies au fil du temps).

## Account-Based Marketing {#account-based-marketing}

**[Segmentation et filtrage basés sur les personas ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personnalisez vos campagnes ABM pour des personnages spécifiques dans des comptes nommés. La fonction Persona AEM crée un titre de poste par défaut en fonction de la segmentation des prospects et permet de configurer des segmentations de personas supplémentaires.

## Analytics {#analytics}

**[!DNL Bizible]**

* **Champs calculés personnalisés** : utilisez n’importe quel attribut [!DNL Bizible] pour créer des champs personnalisés utilisables pour la segmentation et les rapports des tableaux de bord.

* **Certification SOC II de type II** : la nouvelle certification en matière de sécurité et de confidentialité s’appuie sur l’accréditation de type I du début de l’année.

## [!DNL Web Personalization] {#web-personalization}

**[Ajouter des sous-domaines dans Paramètres de compte](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Pour gérer plus efficacement les domaines et les sous-domaines, les utilisateurs peuvent désormais ajouter des sous-domaines aux paramètres de leur compte RTP.

## Engagement mobile de Marketo (EMM) {#marketo-mobile-engagement-mme}

**Mise à jour du kit de développement logiciel MME (SDK) pour Android**

Nous avons mis à jour notre SDK pour Android vers un framework plus moderne, stable et évolutif, qui offre plus de flexibilité et de nouvelles fonctionnalités d’ingénierie. Les développeurs d’applications Android peuvent désormais utiliser directement la [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) de Google avec ce nouveau SDK.

* [Instructions de développement](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [FAQ pour les développeurs](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Les développeurs d’applications **doivent** à jour vers la nouvelle version avant le 31 mars 2019. Si vous ne mettez pas à jour votre SDK d’ici le 31 mars 2019, tout nouvel utilisateur qui télécharge votre application après cette date ne pourra pas recevoir de notifications push tant que vous n’aurez pas effectué la mise à jour vers la dernière version de SDK. La mise à jour de SDK n’exigera pas que les utilisateurs actuels de votre application mobile téléchargent à nouveau une nouvelle version de votre application.

## Mises à jour supplémentaires {#additional-updates}

**Plateforme de webinaire extensible**

Outre notre mise à jour de produit, notre équipe de partenaires travaille sur un nouveau cadre qui permet aux fournisseurs de webinaires de créer et de gérer leurs propres intégrations avec Marketo, offrant ainsi plus de flexibilité pour mettre à jour et améliorer leurs solutions tout en permettant aux marketeurs de tirer le meilleur parti de leurs intégrations sélectionnées.

Nous prévoyons de déployer notre nouvelle plateforme auprès des fournisseurs au cas par cas. Pour plus d’informations, consultez nos [détails du programme](https://www.marketo.com/why-marketo/partners/technology/) ou contactez votre contact Marketo.
