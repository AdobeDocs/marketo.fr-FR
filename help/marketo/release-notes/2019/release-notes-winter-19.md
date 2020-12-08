---
unique-page-id: 17727823
description: Notes de mise à jour - Hiver 19 - Documentation sur le marketing - Documentation sur le produit
title: Notes de mise à jour - Hiver 19
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---


# Notes de mise à jour : Hiver 19 {#release-notes-winter}

Les fonctionnalités suivantes sont incluses dans la version de l’hiver 19. Vérifiez la disponibilité des fonctionnalités de votre édition Marketing.

Veuillez cliquer sur les liens de titre vers les articles détaillés de la vue pour chaque fonction, le cas échéant.

>[!NOTE]
>
>Facebook a désormais besoin d’un compte Business Manager pour tirer parti de votre intégration d’Audiences personnalisées. Votre service LaunchPoint Facebook *doit* être associé à un compte Business Manager, sinon **votre intégration ne fonctionnera plus après le 14 janvier 2019**. Pour configurer un compte Business Manager, reportez-vous à l’aide [de](https://www.facebook.com/business/help/1710077379203657)Facebook.

>[!NOTE]
>
>Microsoft encourage tous les clients en ligne à effectuer la mise à niveau vers la dernière version de Microsoft Dynamics. Si vous intégrez votre instance de Marketo à Dynamics Online, vous devrez [mettre à niveau la dernière version de la solution](../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md) Marketo avant le 31 **janvier 2019** pour vous assurer que votre intégration continuera à fonctionner.

>[!NOTE]
>
>Marketo met à niveau la version OAuth pour GoToWebinar de 1.0 à 2.0. La prise en charge d’OAuth 1.0 sera abandonnée en janvier 2019. Si vous êtes un client GoToWebinar, vous devrez réauthentifier vos connexions par le biais de LaunchPoint (dans la zone d’administration) d’ici le 31 **janvier 2019** pour vous assurer que votre intégration continuera à fonctionner. Pour plus de détails, veuillez consulter notre page [](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)Communauté .

## Améliorations des plates-formes principales {#core-platform-enhancements}

** [Courrier électronique CC pour les courriels](../../product-docs/email-marketing/general/email-cc.md)marketing**

Inclure jusqu’à cinq adresses CC par destinataire dans les courriers électroniques envoyés via Marketo.

**API**

* **Prise en charge de domaines de marque multiple pour l’API de ressources :** L’approbation et le clonage des ressources produisent les mêmes résultats dans l’API et l’interface utilisateur.
* **Prise en charge de CC par courrier électronique pour l’API** de ressources : Les utilisateurs clonant, approuvant et traitant les courriers électroniques via l’API conservent la parité avec les paramètres de l’interface utilisateur.

** [Munchkin v155 (Beta)](http://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Mode** API uniquement : Les utilisateurs peuvent désormais déterminer quand et comment effectuer le suivi des membres de leur base de données en permettant aux applications Web d’une seule page d’appeler explicitement lorsqu’elles souhaitent enregistrer une visite de page Web au lieu de compter sur le suivi automatique de Marketo.
* **Gestion** des exclusions : Gérez facilement les exclusions en faisant correspondre le domaine du cookie d’exclusion au domaine du cookie de suivi Munchkin.
* **Paramètre** de décideur au niveau du domaine : Domaines à deux lettres (c.-à-d. &quot; [site web.io](http://website.io)&quot;) sera automatiquement suivi dans Marketo sans configuration supplémentaire requise.

## Engagement commercial {#marketo-sales-engage}

* **Profil** personnalisé Salesforce : L&#39;activité commerciale prend désormais en charge un nombre illimité de profils personnalisés.

* **Personnalisation** de Salesforce : En supprimant les champs d&#39;activité personnalisée non critiques, les utilisateurs peuvent configurer plus efficacement Sales Engager dans la plate-forme CRM.
* **Service** de messagerie : Bénéficiez d&#39;une meilleure délivrabilité et d&#39;un suivi des réponses amélioré, de la fonctionnalité de courriel planifié et de la fonctionnalité de courriel en masse en vous connectant à Microsoft Outlook (via Office365 ou On-Prem via l&#39;onglet Connexion par courriel).
* **Nouveaux paramètres** d’administration : Deux pages d&#39;administration ont été ajoutées pour optimiser votre instance d&#39;engagement commercial

   * *Team Management* prend en charge un processus transparent de configuration de compte en permettant aux administrateurs de modifier des abonnements et des équipes.
   * *Les paramètres* d’administration de Salesforce aident les équipes à configurer leur synchronisation SFDC plus rapidement et plus facilement que jamais.

* **Module externe OWA pour Windows**: Avec un seul module complémentaire, tous les clients Windows Office365 seront pris en charge dans Sales Engage, ce qui leur permettra d&#39;utiliser Live Feed dans Outlook. Le nouveau module externe sera disponible dans le Microsoft Store.
* **Activités Pusher**: Synchroniser les ventes Interagir avec la plate-forme principale du marché pour exploiter les informations marketing en temps réel.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Les versions des Marketo Sky se produisent à une cadence plus fréquente. Les fonctionnalités et améliorations suivantes devraient être publiées à la fin du 4e trimestre/début du 1er trimestre. Pour plus de détails et de mises à jour, consultez notre documentation [](https://help.marketo.com/hc/en-us/articles/360012858573)Sky.

* **Expérience** par défaut facultative : Les utilisateurs du marketing peuvent définir le Marketo Sky comme expérience par défaut s’ils ont reçu un accès d’un administrateur.

* **Repensed My Marketo**: Personnalisez votre expérience en ajoutant des widgets qui fournissent des informations essentielles, des notifications et des liens vers les zones les plus visitées.

* **Design Studio Listes Vues &amp; pages** de détails : Bénéficiez d&#39;un niveau d&#39;organisation et de précision accru grâce aux vues de liste filtrables et indexables de courriels, de landings page et de formulaires. Détails du fichier Les pages fournissent des informations clés sur chaque fichier, notamment les programmes d’utilisation du fichier, le nombre d’extraits de code utilisés, etc.

* **Recherche** globale : Marketo offre désormais une fonction de recherche globale plus rapide et plus robuste sur la plate-forme. Les requêtes de recherche s’exécutent désormais sur tous les espaces de travail accessibles et peuvent rechercher des ressources (principales et archivées), des étiquettes, des campagnes et des programmes. Les résultats de la recherche sont fournis par le biais d’une incrustation et chaque résultat inclut son journal d’emplacement de fichier pour spécifier l’emplacement de la ressource.

* **Interface** utilisateur améliorée : De nouvelles icônes, modèles et boutons, ainsi qu’une nouvelle palette de couleurs pour refléter l’actualisation de notre marque et rendre le Marketo Sky encore plus étonnant et fonctionnel.

* **Améliorations** de la convivialité des Programmes électroniques : Nous continuons de progresser vers la parité dans la fonctionnalité de Programme de courriel entre notre plate-forme classique de gestion des pistes de marketing et la nouvelle expérience Marketo Sky.
* **Programmes**&#x200B;événement avec webinaire : Les programmes événement avec webinaire sont maintenant disponibles en Marketo Sky (remarque : seule GoToWebinar sera prise en charge dans cette version, avec d&#39;autres intégrations établies au fil du temps).

## Marketing basé sur le compte {#account-based-marketing}

** Segmentation et filtrage [basés sur la personnalité](../../product-docs/account-based-marketing/using-personas.md)ABM**

Personnalisez vos campagnes ABM pour des personnes spécifiques dans des comptes nommés. La fonction Personnalité ABM crée un titre de tâche par défaut basé sur la segmentation des pistes et permet de configurer d’autres segments de personne.

## Analytics {#analytics}

**Bizible**

* **Champs** calculés personnalisés : Utilisez n’importe quel attribut visible pour créer des champs personnalisés qui peuvent être utilisés pour le rapports et la segmentation des tableaux de bord.

* **Certification** de type II du COS II : La nouvelle certification en matière de sécurité et de protection des renseignements personnels s&#39;appuie sur l&#39;accréditation de type I qui a été délivrée plus tôt cette année.

## Personnalisation Web {#web-personalization}

**[Ajouter des sous-domaines dans les paramètres du compte](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Pour mieux gérer les domaines et sous-domaines, les utilisateurs peuvent désormais ajouter des sous-domaines à leurs paramètres de compte RTP.

## Engagement marketing pour mobile (MME) {#marketo-mobile-engagement-mme}

**Mise à jour du kit de développement logiciel MME (SDK) pour Android**

Nous avons mis à jour notre SDK pour Android vers un cadre plus moderne, stable et évolutif qui offre davantage de flexibilité et de nouvelles fonctionnalités d&#39;ingénierie. Les développeurs d’applications Android peuvent désormais utiliser directement [Firebase Cloud Messaging](http://firebase.google.com/docs/cloud-messaging/) (FCM) de Google avec ce nouveau SDK.

* [Instructions pour le développeur](http://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [FAQ destinée aux développeurs](http://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Les développeurs d’applications **doivent** effectuer la mise à jour vers la nouvelle version avant le 31 mars 2019. Si vous ne mettez pas à jour votre SDK avant le 31 mars 2019, tout nouvel utilisateur qui télécharge votre application après cette date ne pourra pas recevoir de notifications Push tant que vous n’aurez pas effectué la mise à jour vers la dernière version du SDK. La mise à jour du SDK n’exigera pas que les utilisateurs actuels de votre application mobile téléchargent à nouveau une nouvelle version de votre application.

## Autres mises à jour {#additional-updates}

**Plateforme Web extensible**

Outre la publication de nos produits, notre équipe de partenaires travaille sur un nouveau cadre qui permet aux fournisseurs de webinaires de créer et de gérer leurs propres intégrations avec Marketo, offrant une plus grande flexibilité dans la mise à jour et l’amélioration de leurs solutions tout en permettant aux spécialistes du marketing de tirer le meilleur parti de leurs intégrations choisies.

Nous prévoyons de déployer notre nouvelle plate-forme avec les fournisseurs au cas par cas. Pour plus d&#39;informations, consultez les détails [de notre](https://www.marketo.com/why-marketo/partners/technology/) programme ou communiquez avec votre contact Marketing.
