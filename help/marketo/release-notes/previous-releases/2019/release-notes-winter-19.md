---
unique-page-id: 17727823
description: Notes de mise à jour - Hiver 2019 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - hiver 19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 3%

---

# Notes de mise à jour : hiver 19 {#release-notes-winter}

Les fonctionnalités suivantes sont incluses dans la version de l’hiver 19. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Marketo.

Cliquez sur les liens de titre pour afficher des articles détaillés pour chaque fonction, le cas échéant.

>[!NOTE]
>
>Facebook a désormais besoin d’un compte Business Manager pour tirer parti de votre intégration d’audience personnalisée. Votre service Facebook LaunchPoint *doit* être associé à un compte Business Manager ou **votre intégration ne fonctionnera plus après le 14 janvier 2019**. Pour configurer un compte Business Manager, reportez-vous à l’ [aide de Facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft incite tous les clients en ligne à effectuer la mise à niveau vers la dernière version de Microsoft Dynamics. Si vous intégrez votre instance Marketo à Dynamics Online, vous devrez [mettre à niveau vers la dernière version de la solution Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) avant le **31 janvier 2019** pour vous assurer que votre intégration continuera à fonctionner.

>[!NOTE]
>
>Marketo met à niveau la version OAuth pour GoToWebinar de 1.0 à 2.0. La prise en charge d’OAuth 1.0 sera abandonnée en janvier 2019. Si vous êtes client GoToWebinar, vous devrez réauthentifier vos connexions par le biais de LaunchPoint (dans la zone d’administration) d’ici le **31 janvier 2019** pour vous assurer que votre intégration continuera à fonctionner. Pour plus de détails, consultez notre [page de la communauté](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Améliorations principales de la plateforme {#core-platform-enhancements}

**[Email CC pour les emails Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Ajoutez jusqu’à cinq adresses Cc par destinataire sur les e-mails envoyés via Marketo. 

**API**

* **Prise en charge de domaines de marque multiple pour l’API Asset :** L’approbation et le clonage de ressources produisent les mêmes résultats au sein de l’API et de l’interface utilisateur.
* **Prise en charge de la fonctionnalité Email CC pour l’API Asset** : les utilisateurs clonent, approuvent et traitent les emails via l’API maintiendront la parité avec les paramètres de l’interface utilisateur.

**[Munchkin v155 (Beta)](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking)**

* **Mode API uniquement** : les utilisateurs peuvent désormais déterminer quand et comment effectuer le suivi des membres de leur base de données en permettant aux applications web d’une seule page d’appeler explicitement lorsqu’elles souhaitent enregistrer une visite de page web au lieu de compter sur le suivi automatique Marketo.
* **Gestion de l’exclusion** : gérez facilement les exclusions en faisant correspondre le domaine du cookie d’exclusion au domaine du cookie de suivi Munchkin.
* **Paramètre de décideur au niveau du domaine** : les domaines à deux lettres (c’est-à-dire &quot; [site web.io](https://website.io)&quot;) seront automatiquement suivis dans Marketo sans configuration supplémentaire.

## Marketo Sales Engage {#marketo-sales-engage}

* **Profil personnalisé Salesforce** : Sales Engage prend désormais en charge un nombre illimité de profils personnalisés.

* **Personnalisation de Salesforce** : en supprimant les champs d’activité personnalisés non critiques, les utilisateurs peuvent configurer plus efficacement l’interaction des ventes avec la plateforme de gestion de la relation client.
* **Service de messagerie électronique** : profitez d’une meilleure délivrabilité, ainsi que d’un suivi des réponses amélioré, de la fonctionnalité de planification des e-mails et de la fonctionnalité d’e-mail en masse en vous connectant à Microsoft Outlook (par le biais d’Office365 ou d’On-Prem via l’onglet Connexion par e-mail).
* **Nouveaux paramètres d’administration** : deux pages d’administration ont été ajoutées pour optimiser votre instance Sales Engage.

   * _Gestion des équipes_ prend en charge un processus transparent de configuration de compte en permettant aux administrateurs de modifier les abonnements et les équipes.
   * _Paramètres d’administration Salesforce_ permet aux équipes de configurer leur synchronisation SFDC plus rapidement et plus facilement que jamais auparavant.

* **Module externe OWA pour Windows** : avec un seul module complémentaire, tous les clients Windows Office365 seront pris en charge dans Sales Engage, ce qui leur permettra d’utiliser le flux en direct dans Outlook. Le nouveau module externe sera disponible dans Microsoft Store.
* **Activity Pusher** : synchronisez les ventes interagissez avec la plateforme Marketo principale pour tirer parti des informations marketing en temps réel.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Les mises à jour de Marketo Sky se produisent plus fréquemment. Les fonctionnalités et améliorations suivantes devraient être publiées à la fin du 4e trimestre/début du 1er trimestre. Pour plus de détails et de mises à jour, consultez notre [documentation Sky](https://help.marketo.com/).

* **Expérience par défaut facultative** : les utilisateurs de Marketo peuvent définir Marketo Sky comme expérience par défaut s’ils disposent d’un accès d’administrateur.

* **Rethinking My Marketo** : personnalisez votre expérience en ajoutant des widgets qui fournissent des informations critiques, des notifications et des liens vers vos zones les plus fréquemment visitées.

* **Design Studio List Views &amp; Detail Pages** : profitez d’un niveau d’organisation et d’une précision accrus avec des vues de liste filtrables et consultables d’emails, de pages d’entrée et de formulaires. Détails de la ressource Les pages contiennent des informations clés sur chaque ressource, notamment les programmes utilisés par la ressource, le nombre d’extraits de code utilisés, etc.

* **Recherche globale** : Marketo offre désormais une fonction de recherche globale plus rapide et plus robuste sur la plateforme. Les requêtes de recherche s’exécutent désormais sur tous les espaces de travail accessibles et peuvent rechercher des ressources (actives et archivées), des libellés, des campagnes et des programmes. Les résultats de recherche sont fournis par le biais d’une superposition et chaque résultat inclut son journal d’emplacement de fichier pour spécifier l’emplacement de la ressource.

* **Interface utilisateur améliorée** : nouvelles icônes, maquettes et boutons, ainsi qu’une nouvelle palette de couleurs pour refléter l’actualisation de notre marque et rendre Marketo Sky encore plus étonnant et fonctionnel.

* **Améliorations de l’utilisation du programme de messagerie électronique** : nous continuons à évoluer vers la parité des fonctionnalités du programme de messagerie électronique entre notre plateforme Marketo Lead Management classique et la nouvelle expérience du Marketo Sky.
* **Programmes Event-With-Webinar** : les programmes Event-With-Webinar sont désormais disponibles en Marketo Sky (remarque : seul GoToWebinar sera pris en charge dans cette version, avec d’autres intégrations établies au fil du temps).

## Account-Based Marketing {#account-based-marketing}

**[Segmentation et filtrage basées sur ABM Persona](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personnalisez vos campagnes ABM pour des personnes spécifiques dans des comptes nommés. La fonction personnage ABM crée un titre de tâche par défaut basé sur la segmentation des pistes et permet de configurer des segments de persona supplémentaires.

## Analytics {#analytics}

**Bizible**

* **Champs calculés personnalisés** : utilisez n’importe quel attribut Bizible pour créer des champs personnalisés qui peuvent être utilisés pour la création de rapports et la segmentation dans les tableaux de bord.

* **Certification de type II SOC II** : nouvelle certification de sécurité et de confidentialité reposant sur l’accréditation de type I au début de l’année.

## Personnalisation Web {#web-personalization}

**[Ajouter des sous-domaines dans Paramètres de compte](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Pour gérer plus efficacement les domaines et les sous-domaines, les utilisateurs peuvent désormais ajouter des sous-domaines aux paramètres de leur compte RTP.

## Engagement mobile de Marketo (EMM) {#marketo-mobile-engagement-mme}

**MME Software Development Kit (SDK) mis à jour pour Android**

Nous avons mis à jour notre SDK pour Android vers un framework plus moderne, stable et évolutif qui contient plus de flexibilité et de nouvelles fonctionnalités d’ingénierie. Les développeurs d’applications Android peuvent désormais utiliser directement le service Google [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) avec ce nouveau SDK.

* [Instructions pour les développeurs]https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android)

>[!NOTE]
>
>Les développeurs d’applications **doivent** mettre à jour la nouvelle version avant le 31 mars 2019. Si vous ne mettez pas à jour votre SDK avant le 31 mars 2019, tout nouvel utilisateur qui télécharge votre application après cette date ne pourra pas recevoir de notifications push tant que vous n’aurez pas effectué la mise à jour vers la dernière version du SDK. La mise à jour du SDK ne nécessite pas que les utilisateurs actuels de l’application mobile téléchargent à nouveau une nouvelle version de l’application.

## Mises à jour supplémentaires {#additional-updates}

**Plateforme de webinaire extensible**

En plus de notre version de produit, notre équipe de partenaires travaille sur un nouveau cadre qui permet aux fournisseurs de webinaires de créer et de gérer leurs propres intégrations avec Marketo, offrant plus de flexibilité pour mettre à jour et améliorer leurs solutions tout en permettant aux marketeurs de tirer le meilleur parti de leurs intégrations sélectionnées.

Nous prévoyons de déployer notre nouvelle plate-forme avec les fournisseurs au cas par cas. Pour plus d’informations, consultez nos [détails du programme](https://www.marketo.com/why-marketo/partners/technology/) ou contactez votre contact Marketo.
