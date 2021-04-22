---
unique-page-id: 17727823
description: Notes de mise à jour - Hiver 19 - Marketo Docs - Documentation sur le produit
title: Notes de mise à jour - Hiver 19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 3%

---

# Notes de mise à jour : Hiver 19 {#release-notes-winter}

Les fonctionnalités suivantes sont incluses dans la version de l’hiver 19. Consultez votre édition Marketo pour connaître la disponibilité des fonctionnalités.

Veuillez cliquer sur les liens de titre vers les articles détaillés de la vue pour chaque fonction, le cas échéant.

>[!NOTE]
>
>Facebook a désormais besoin d’un compte Business Manager pour tirer parti de l’intégration de votre Audience personnalisée. Votre service Facebook LaunchPoint *doit* être associé à un compte Business Manager, sinon **votre intégration ne fonctionnera plus après le 14 janvier 2019**. Pour configurer un compte Business Manager, consultez l&#39;[Aide de Facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft encourage tous les clients en ligne à effectuer la mise à niveau vers la dernière version de Microsoft Dynamics. Si vous intégrez votre instance Marketo à Dynamics Online, vous devrez [mettre à niveau vers la dernière version de la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) avant le **31 janvier 2019** pour vous assurer que votre intégration continuera à fonctionner.

>[!NOTE]
>
>Marketo met à niveau la version OAuth pour GoToWebinar de 1.0 à 2.0. La prise en charge d’OAuth 1.0 sera abandonnée en janvier 2019. Si vous êtes un client GoToWebinar, vous devrez réauthentifier vos connexions par le biais de LaunchPoint (dans la zone Admin) d’ici le **31 janvier 2019** pour vous assurer que votre intégration continuera à fonctionner. Pour plus de détails, veuillez consulter notre [page communautaire](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Améliorations principales de la plateforme {#core-platform-enhancements}

**[Courriel CC pour les courriels Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Ajoutez jusqu’à cinq adresses Cc par destinataire sur les e-mails envoyés via Marketo. 

**API**

* **Prise en charge de domaines de marque multiple pour l’API des ressources :** l’approbation et le clonage des ressources produisent les mêmes résultats dans l’API et l’interface utilisateur.
* **Prise en charge de CC par courrier électronique pour l’API** de ressources : Les utilisateurs clonant, approuvant et traitant les courriers électroniques via l’API conservent la parité avec les paramètres de l’interface utilisateur.

**[Munchkin v155 (bêta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Mode** API uniquement : Les utilisateurs peuvent désormais déterminer quand et comment suivre les membres de leur base de données en autorisant les applications Web d’une seule page à appeler explicitement lorsqu’ils souhaitent enregistrer une visite de page Web au lieu de compter sur le suivi automatique Marketo.
* **Gestion** des exclusions : Gérez facilement les exclusions en faisant correspondre le domaine du cookie d’exclusion au domaine du cookie de suivi Munchkin.
* **Paramètre** de décideur au niveau du domaine : Domaines à deux lettres (c.-à-d. &quot;  [site web.io](https://website.io)&quot;) sera automatiquement suivi dans Marketo sans configuration supplémentaire requise.

## Marketo Sales Engage {#marketo-sales-engage}

* **Profil** personnalisé Salesforce : L&#39;activité commerciale prend désormais en charge un nombre illimité de profils personnalisés.

* **Personnalisation** de Salesforce : En supprimant les champs d&#39;activité personnalisée non critiques, les utilisateurs peuvent configurer plus efficacement Sales Engager dans la plate-forme CRM.
* **Service** de messagerie : Bénéficiez d&#39;une meilleure délivrabilité et d&#39;un suivi des réponses amélioré, de la fonctionnalité de courriel planifié et de la fonctionnalité de courriel en masse en vous connectant à Microsoft Outlook (via Office365 ou On-Prem via l&#39;onglet Connexion par courriel).
* **Nouveaux paramètres** d’administration : Deux pages d&#39;administration ont été ajoutées pour optimiser votre instance d&#39;engagement commercial

   * _Team_ Management prend en charge un processus transparent de configuration de compte en permettant aux administrateurs de modifier des abonnements et des équipes.
   * _Les équipes des_ restaurants d’administration de Salesforce ont configuré leur synchronisation SFDC plus rapidement et plus facilement que jamais.

* **Module externe OWA pour Windows** : Avec un seul module complémentaire, tous les clients Windows Office365 seront pris en charge dans Sales Engage, ce qui leur permettra d&#39;utiliser Live Feed dans Outlook. Le nouveau module externe sera disponible dans le Microsoft Store.
* **Activités Pusher** : Synchroniser les ventes Interagir avec la plate-forme principale de Marketo pour tirer parti des informations marketing en temps réel.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Les versions des Marketo Sky se produisent à une cadence plus fréquente. Les fonctionnalités et améliorations suivantes devraient être publiées à la fin du 4e trimestre/début du 1er trimestre. Pour plus de détails et de mises à jour, consultez notre [documentation Sky](https://help.marketo.com/).

* **Expérience** par défaut facultative : Les utilisateurs de Marketo peuvent définir le Marketo Sky comme expérience par défaut s’ils ont reçu un accès d’un administrateur.

* **Rethinking My Marketo** : Personnalisez votre expérience en ajoutant des widgets qui fournissent des informations essentielles, des notifications et des liens vers les zones les plus visitées.

* **Design Studio Listes Vues &amp; pages** de détails : Bénéficiez d&#39;un niveau d&#39;organisation et de précision accru grâce aux vues de liste filtrables et indexables de courriels, de landings page et de formulaires. Détails du fichier Les pages fournissent des informations clés sur chaque fichier, notamment les programmes d’utilisation du fichier, le nombre d’extraits de code utilisés, etc.

* **Recherche** globale : Marketo offre désormais une fonction de recherche globale plus rapide et plus robuste sur l’ensemble de la plate-forme. Les requêtes de recherche s’exécutent désormais sur tous les espaces de travail accessibles et peuvent rechercher des ressources (principales et archivées), des étiquettes, des campagnes et des programmes. Les résultats de la recherche sont fournis par le biais d’une incrustation et chaque résultat inclut son journal d’emplacement de fichier pour spécifier l’emplacement de la ressource.

* **Interface** utilisateur améliorée : De nouvelles icônes, modèles et boutons, ainsi qu’une nouvelle palette de couleurs pour refléter l’actualisation de notre marque et rendre le Marketo Sky encore plus étonnant et fonctionnel.

* **Améliorations** de la convivialité des Programmes électroniques : Nous continuons de progresser vers la parité dans la fonctionnalité de Programme de courriel entre notre plate-forme classique de gestion des pistes de Marketo et la nouvelle expérience Marketo Sky.
* **Programmes** événement avec webinaire : Les programmes événement avec webinaire sont maintenant disponibles en Marketo Sky (remarque : seule GoToWebinar sera prise en charge dans cette version, avec d&#39;autres intégrations établies au fil du temps).

## Account-Based Marketing {#account-based-marketing}

**[Segmentation et filtrage basés sur la personnalité ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personnalisez vos campagnes ABM pour des personnes spécifiques dans des comptes nommés. La fonction Personnalité ABM crée un titre de tâche par défaut basé sur la segmentation des pistes et permet de configurer d’autres segments de personne.

## Analyses {#analytics}

**Bizible**

* **Champs** calculés personnalisés : Utilisez n’importe quel attribut visible pour créer des champs personnalisés qui peuvent être utilisés pour le rapports et la segmentation des tableaux de bord.

* **Certification** de type II du COS II : La nouvelle certification en matière de sécurité et de protection des renseignements personnels s&#39;appuie sur l&#39;accréditation de type I qui a été délivrée plus tôt cette année.

## personnalisation Web {#web-personalization}

**[Ajouter des sous-domaines dans Paramètres de compte](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Pour mieux gérer les domaines et sous-domaines, les utilisateurs peuvent désormais ajouter des sous-domaines à leurs paramètres de compte RTP.

## Engagement mobile de Marketo (EMM) {#marketo-mobile-engagement-mme}

**Mise à jour du kit de développement logiciel MME (SDK) pour Android**

Nous avons mis à jour notre SDK pour Android vers un cadre plus moderne, stable et évolutif qui offre davantage de flexibilité et de nouvelles fonctionnalités d&#39;ingénierie. Les développeurs d’applications Android peuvent désormais utiliser directement [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) de Google avec ce nouveau SDK.

* [Instructions pour le développeur](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [FAQ destinée aux développeurs](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Les développeurs d’applications **doivent** mettre à jour leur nouvelle version avant le 31 mars 2019. Si vous ne mettez pas à jour votre SDK avant le 31 mars 2019, tout nouvel utilisateur qui télécharge votre application après cette date ne pourra pas recevoir de notifications Push tant que vous n’aurez pas effectué la mise à jour vers la dernière version du SDK. La mise à jour du SDK n’exigera pas que les utilisateurs actuels de votre application mobile téléchargent à nouveau une nouvelle version de votre application.

## Mises à jour supplémentaires {#additional-updates}

**Plateforme Web extensible**

En plus de la publication de nos produits, notre équipe de partenaires travaille sur un nouveau cadre qui permet aux fournisseurs de webinaires de créer et de maintenir leurs propres intégrations avec Marketo, offrant plus de flexibilité pour mettre à jour et améliorer leurs solutions tout en permettant aux spécialistes du marketing de tirer le meilleur parti de leurs intégrations choisies.

Nous prévoyons de déployer notre nouvelle plate-forme avec les fournisseurs au cas par cas. Pour plus d&#39;informations, consultez nos [détails du programme](https://www.marketo.com/why-marketo/partners/technology/) ou contactez votre contact Marketo.
