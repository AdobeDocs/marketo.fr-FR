---
unique-page-id: 17727823
description: Notes de mise à jour - Hiver 2019 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Hiver 2019
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 3%

---

# Notes de mise à jour : Hiver 19 {#release-notes-winter}

Les fonctionnalités suivantes sont incluses dans la version de l’hiver 19. Vérifiez la disponibilité de votre édition Marketo.

Cliquez sur les liens de titre pour afficher des articles détaillés pour chaque fonction, le cas échéant.

>[!NOTE]
>
>Facebook nécessite désormais un compte Business Manager pour tirer parti de votre intégration d’audience personnalisée. Votre service Facebook LaunchPoint *must* être associé à un compte Business Manager ; ou **votre intégration ne fonctionnera plus après le 14 janvier 2019.**. Pour configurer un compte Business Manager, reportez-vous à la section [Aide de facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft incite tous les clients en ligne à effectuer la mise à niveau vers la dernière version de Microsoft Dynamics. Si vous intégrez votre instance Marketo à Dynamics Online, vous devez [mise à niveau vers la dernière version de la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) before **31 janvier 2019** pour vous assurer que votre intégration continuera à fonctionner.

>[!NOTE]
>
>Marketo met à niveau la version OAuth pour GoToWebinar de la version 1.0 à la version 2.0. La prise en charge d’OAuth 1.0 sera abandonnée en janvier 2019. Si vous êtes client GoToWebinar, vous devrez réauthentifier vos connexions par le biais de LaunchPoint (dans la zone d’administration) par **31 janvier 2019** pour vous assurer que votre intégration continuera à fonctionner. Pour plus de détails, reportez-vous à notre [Page de la communauté](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Améliorations principales de la plateforme {#core-platform-enhancements}

**[Email CC pour les emails Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Ajoutez jusqu’à cinq adresses Cc par destinataire sur les e-mails envoyés via Marketo. 

**API**

* **Prise en charge de domaines de marque multiple pour l’API Asset :** L’approbation et le clonage des ressources produisent les mêmes résultats au sein de l’API et de l’interface utilisateur.
* **Prise en charge de la messagerie électronique pour l’API Asset**: Les utilisateurs qui clonent, approuvent et traitent les emails via l’API conservent la parité avec les paramètres de l’interface utilisateur.

**[Munchkin v155 (bêta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Mode API uniquement**: Les utilisateurs peuvent désormais déterminer quand et comment suivre les membres de leur base de données en autorisant les applications web d’une seule page à appeler explicitement lorsqu’ils souhaitent enregistrer une visite de page web au lieu de compter sur le suivi automatique Marketo.
* **Gestion des exclusions**: Gérez facilement les exclusions en faisant correspondre le domaine du cookie d’exclusion au domaine du cookie de suivi Munchkin.
* **Paramètre du décideur au niveau du domaine**: Domaines à deux lettres (c’est-à-dire &quot; [website.io](https://website.io)&quot;) effectue automatiquement le suivi dans Marketo sans configuration supplémentaire requise.

## Marketo Sales Engage {#marketo-sales-engage}

* **Profil personnalisé Salesforce**: Sales Engage prend désormais en charge un nombre illimité de profils personnalisés.

* **Personnalisation de Salesforce**: En supprimant les champs d’activité personnalisés non critiques, les utilisateurs peuvent configurer plus efficacement Sales Engage dans la plateforme CRM.
* **Service de messagerie électronique**: Bénéficiez d’une meilleure délivrabilité, ainsi que d’une fonctionnalité améliorée de suivi des réponses, de messagerie planifiée et de messagerie en masse, en vous connectant à Microsoft Outlook (par le biais d’Office365 ou d’On-Prem via l’onglet Connexion par e-mail).
* **Nouveaux paramètres d’administration**: Deux pages d’administration ont été ajoutées pour optimiser votre instance Sales Engage.

   * _Gestion des équipes_ prend en charge un processus transparent de configuration de compte en permettant aux administrateurs de modifier les abonnements et les équipes.
   * _Paramètres d’administration Salesforce_ aide les équipes à configurer leur synchronisation SFDC plus rapidement et plus facilement que jamais auparavant.

* **Module externe OWA pour Windows**: Avec un seul module complémentaire, tous les clients Windows Office365 seront pris en charge dans Sales Engage, ce qui leur permettra d’utiliser le flux dynamique dans Outlook. Le nouveau module externe sera disponible dans Microsoft Store.
* **Opérateur d’activités**: Synchronisation des ventes : interagissez avec la plateforme Marketo principale pour exploiter les informations marketing en temps réel.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Les versions de Marketo Sky se produisent plus fréquemment. Les fonctionnalités et améliorations suivantes devraient être publiées à la fin du 4e trimestre/début du 1er trimestre. Pour plus d’informations et de mises à jour, consultez notre [Documentation du ciel](https://help.marketo.com/).

* **Expérience par défaut facultative**: Les utilisateurs de Marketo peuvent définir Marketo Sky comme expérience par défaut s’ils disposent d’un accès d’administrateur.

* **Réimagination de mon Marketo**: Personnalisez votre expérience en ajoutant des widgets qui fournissent des informations critiques, des notifications et des liens vers vos zones les plus fréquemment visitées.

* **Pages de détails et vues de liste de Design Studio**: Bénéficiez d’un niveau d’organisation et d’une précision accrus grâce aux affichages de listes filtrables et consultables d’emails, de landing pages et de formulaires. Détails de la ressource Les pages contiennent des informations clés sur chaque ressource, notamment les programmes utilisés par la ressource, le nombre d’extraits de code utilisés, etc.

* **Recherche globale**: Marketo offre désormais une fonction de recherche globale plus rapide et plus robuste sur la plateforme. Les requêtes de recherche s’exécutent désormais sur tous les espaces de travail accessibles et peuvent rechercher des ressources (principales et archivées), des étiquettes, des campagnes et des programmes. Les résultats de recherche sont fournis par le biais d’une superposition et chaque résultat inclut son journal d’emplacement de fichier pour spécifier l’emplacement de la ressource.

* **Interface utilisateur améliorée**: Nouvelles icônes, modèles et boutons, ainsi qu’une nouvelle palette de couleurs pour refléter l’actualisation de notre marque et rendre notre Marketo Sky encore plus étonnant et fonctionnel.

* **Améliorations de l’utilisation du programme de messagerie électronique**: Nous continuons à évoluer vers la parité des fonctionnalités du programme de messagerie électronique entre notre plateforme de gestion des pistes Marketo classique et la nouvelle expérience du Marketo Sky.
* **Programmes Event-With-Webinar**: Les programmes Event-With-Webinar sont désormais disponibles en Marketo Sky (remarque : Seul GoToWebinar sera pris en charge dans cette version, avec d’autres intégrations établies au fil du temps).

## Account-Based Marketing {#account-based-marketing}

**[Segmentation et filtrage basées sur ABM Persona](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personnalisez vos campagnes ABM pour des personnes spécifiques dans des comptes nommés. La fonction personnage ABM crée un titre de tâche par défaut basé sur la segmentation des pistes et permet de configurer des segments de persona supplémentaires.

## Analytics {#analytics}

**Bizible**

* **Champs calculés personnalisés**: Utilisez n’importe quel attribut Bizible pour créer des champs personnalisés qui peuvent être utilisés pour la création de rapports et la segmentation du tableau de bord.

* **Certification de type II SOC**: La nouvelle certification en matière de sécurité et de confidentialité s’appuie sur l’accréditation de type I au début de l’année.

## Personnalisation Web {#web-personalization}

**[Ajouter des sous-domaines dans Paramètres de compte](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Pour gérer plus efficacement les domaines et les sous-domaines, les utilisateurs peuvent désormais ajouter des sous-domaines aux paramètres de leur compte RTP.

## Engagement mobile de Marketo (EMM) {#marketo-mobile-engagement-mme}

**Mise à jour du SDK (Software Development Kit) MME pour Android**

Nous avons mis à jour notre SDK pour Android vers un framework plus moderne, stable et évolutif qui contient plus de flexibilité et de nouvelles fonctionnalités d’ingénierie. Les développeurs d’applications Android peuvent désormais utiliser directement le [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) avec ce nouveau SDK.

* [Instructions pour les développeurs](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [FAQ destiné aux développeurs](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Développeurs d’applications **must** mise à jour vers la nouvelle version avant le 31 mars 2019. Si vous ne mettez pas à jour votre SDK avant le 31 mars 2019, tout nouvel utilisateur qui télécharge votre application après cette date ne pourra pas recevoir de notifications push tant que vous n’aurez pas effectué la mise à jour vers la dernière version du SDK. La mise à jour du SDK ne nécessite pas que les utilisateurs actuels de l’application mobile téléchargent à nouveau une nouvelle version de l’application.

## Mises à jour supplémentaires {#additional-updates}

**Plateforme de webinaire extensible**

En plus de notre version de produit, notre équipe de partenaires travaille sur un nouveau cadre qui permet aux fournisseurs de webinaires de créer et de gérer leurs propres intégrations avec Marketo, offrant plus de flexibilité pour mettre à jour et améliorer leurs solutions tout en permettant aux marketeurs de tirer le meilleur parti de leurs intégrations sélectionnées.

Nous prévoyons de déployer notre nouvelle plate-forme avec les fournisseurs au cas par cas. Pour plus d’informations, voir notre [détails du programme](https://www.marketo.com/why-marketo/partners/technology/) ou contactez votre contact Marketo.
