---
title: 2019
description: 2019 - Documents Marketo - Documentation Du Produit
feature: Release Information
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e2290edd-b061-4880-9d79-dee306cf5aa9id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: d5c7388a-594e-4d15-9b39-98d6ce479e8bid: de9e3aa9-f002-4fe1-897b-09ee3c55114bid: df8eb12b-4f82-491f-acbb-d74012ca5654id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: bbbea26f-9621-49eb-9ab8-e06fb3bbce8cid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: d095671a-1355-40aa-8b5f-06c33c68080bid: e0eb8757-182f-49f3-94a4-1587d16f5094id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 1e70b9383bf3a1cd30715df4379d440c4efb1abd
workflow-type: tm+mt
source-wordcount: 2528
ht-degree: 3%

---

# 2019

## Hiver 2019 {#winter}

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

## Améliorations principales de la plateforme

**[Email CC pour les e-mails Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Ajoutez jusqu’à cinq adresses Cc par destinataire sur les e-mails envoyés via Marketo.

**API**

* **Prise en charge de domaines multi-marques pour l’API de ressources :** l’approbation et le clonage des ressources produisent les mêmes résultats dans l’API et l’interface utilisateur.
* **Prise en charge de la fonctionnalité CC par e-mail pour l’API de ressources** : les utilisateurs qui clonent, approuvent et traitent des e-mails via l’API conserveront la parité avec les paramètres de l’interface utilisateur.

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Mode API uniquement** : les utilisateurs peuvent désormais déterminer quand et comment effectuer le suivi des membres de leur base de données en permettant aux applications web monopages d’appeler explicitement lorsqu’ils souhaitent enregistrer une visite de page web au lieu de compter sur le suivi automatique de Marketo.
* **Gestion des processus d’opt-out** : gérez facilement les processus d’opt-out en faisant correspondre le domaine du cookie d’opt-out avec le domaine du cookie de suivi [!DNL Munchkin].
* **Paramètre de décision au niveau du domaine** : les domaines à deux lettres (c’est-à-dire « [website.io](https://website.io) ») feront automatiquement l’objet d’un suivi dans Marketo sans exigences de configuration supplémentaires.

## Marketo Sales Engage

* **[!DNL Salesforce]profil personnalisé** : Sales Engage prend désormais en charge un nombre illimité de profils personnalisés.

* Personnalisation de l’**[!DNL Salesforce]: en supprimant les champs d’activité personnalisés non critiques** les utilisateurs et les utilisatrices peuvent configurer plus efficacement Sales Engage dans la plateforme CRM.
* **Service de messagerie électronique** : bénéficiez d&#39;une meilleure délivrabilité ainsi que d&#39;un meilleur suivi des réponses, de fonctionnalités de messagerie planifiée et de fonctionnalités de messagerie en masse en vous connectant à [!DNL Microsoft Outlook] (soit via Office365, soit On-Prem via l&#39;onglet Connexion par e-mail).
* **Nouveaux paramètres d’administration** : deux pages d’administration ont été ajoutées pour optimiser votre instance Sales Engage

   * *Team Management* prend en charge un processus de configuration de compte transparent en permettant aux administrateurs de modifier les abonnements et les équipes.
   * *Paramètres d’administration Salesforce* aide les équipes à configurer leur synchronisation SFDC plus rapidement et plus facilement que jamais auparavant.

* **Module externe OWA pour[!DNL Windows]** : avec un seul module complémentaire, tous les clients [!DNL Windows Office365] seront pris en charge dans Sales Engage, ce qui permet d’utiliser le flux en direct dans Outlook. Le nouveau plug-in sera disponible dans la boutique Microsoft.
* **Activités de promotion** : synchronisez Sales Engage à la plateforme Marketo de base pour tirer parti des informations marketing en temps réel.

## [!DNL Marketo Sky]

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

## Account-Based Marketing

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

Nous avons mis à jour notre SDK pour Android vers un framework plus moderne, stable et évolutif, qui offre plus de flexibilité et de nouvelles fonctionnalités d’ingénierie. Les développeurs d’applications Android peuvent désormais utiliser directement Google [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) avec ce nouveau SDK.

* [Instructions pour le développeur](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [FAQ destinée aux développeurs](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Les développeurs d’applications **doivent** à jour vers la nouvelle version avant le 31 mars 2019. Si vous ne mettez pas à jour votre SDK d’ici le 31 mars 2019, tout nouvel utilisateur qui télécharge votre application après cette date ne pourra pas recevoir de notifications push tant que vous n’aurez pas effectué la mise à jour vers la dernière version de SDK. La mise à jour de SDK n’exigera pas que les utilisateurs actuels de votre application mobile téléchargent à nouveau une nouvelle version de votre application.

## Mises à jour supplémentaires {#additional-updates}

**Plateforme de webinaire extensible**

Outre notre mise à jour de produit, notre équipe de partenaires travaille sur un nouveau cadre qui permet aux fournisseurs de webinaires de créer et de gérer leurs propres intégrations avec Marketo, offrant ainsi plus de flexibilité pour mettre à jour et améliorer leurs solutions tout en permettant aux marketeurs de tirer le meilleur parti de leurs intégrations sélectionnées.

Nous prévoyons de déployer notre nouvelle plateforme auprès des fournisseurs au cas par cas. Pour plus d’informations, consultez nos [détails du programme](https://www.marketo.com/why-marketo/partners/technology/) ou contactez votre contact Marketo.

## Printemps 2019 {#spring}

Les fonctionnalités suivantes sont incluses dans la version du printemps 19. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

Cliquez sur les liens de titre pour consulter les articles détaillés de chaque fonctionnalité, le cas échéant.

***Versions trimestrielles_**

Les fonctionnalités suivantes ont été publiées le 15 mars 2019.

## Améliorations principales de la plateforme

* **Sur liste d’attente :** nouveau statut de programme/événement pour placer en liste d’attente un membre lorsque vous souhaitez [le mettre en attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) jusqu’à l’ouverture d’un poste vacant. Cela s’applique aux canaux associés aux programmes Événement dans Marketo Classic, ainsi qu’aux programmes Événement et Événement avec webinaire dans [!DNL Marketo Sky]. Par défaut, Waitlisted a la même valeur d’étape que Registered.
* **[Limite de communication personnalisée](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)** : les administrateurs peuvent désormais définir des limites de communication personnalisées quotidiennes ou hebdomadaires.
* **[API de ressources de campagne intelligente](https://developers.marketo.com/rest-api/assets/smart-campaigns/)** : enrichissez vos analyses en dehors de Marketo avec la récupération d’enregistrements de campagne intelligente par date et ID mis à jour.
* **Liens de suivi HTTPS pour les e-mails :** pour les clients qui ont acheté « Domaines sécurisés pour les liens de suivi », les liens de suivi de marque peuvent désormais être affichés dans vos e-mails en tant que HTTPS.
* **Mises à jour du Powerpack relatives à la délivrabilité des e-mails** : possibilité de marquer et de commenter des résultats de test spécifiques, de partager les résultats avec les parties prenantes par le biais d’une URL et de suivre les modifications pour voir l’évolution d’un e-mail à mesure que les parties prenantes modifient le contenu.

Account-Based Marketing

**[AccountAI](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)** Désormais généralement disponible. CompteAI utilise l’intelligence artificielle pour indiquer les comptes que vous devriez cibler dans le cadre de votre stratégie ABM.

<br> 

**_Versions Non Trimestrielles_**

Les fonctionnalités suivantes devraient être publiées tout au long du premier trimestre civil et au début du deuxième trimestre 2019.

## [!DNL Marketo Sky]

* **Fonctionnalité complète du programme de messagerie électronique** : envoyez des e-mails, créez des tests A/B et suivez les résultats dans une expérience conviviale.
* **Fonctionnalité de campagne intelligente** : profitez d’une stabilité améliorée dans une nouvelle interface utilisateur à mesure que la fonctionnalité de campagne intelligente continue de se déployer dans Sky.
* **Gérer Design Studio Assets** : possibilité supplémentaire de gérer les modèles, les images, le Forms, les fragments de code, les fichiers, les e-mails et les pages de destination en bloc à partir des vues de liste de Design Studio.
* **Diffusion dans le tableau de bord du fuseau horaire du destinataire** : comprenez le comportement des clients avec le compte rendu des performances des e-mails envoyés à l’aide de la fonction Diffuser dans le fuseau horaire du destinataire dans Sky.

## Marketo Sales Engage

* **Audit amélioré** : nouvelle visibilité sur toutes les personnes, tous les e-mails et [le contenu](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md) dans une instance avec une possibilité supplémentaire de [mettre fin aux campagnes existantes](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md)créées par d’autres utilisateurs.
* **[Gestion des désabonnements](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md)** : optimisez la délivrabilité et la conformité grâce à la possibilité de [bloquer les domaines d’e-mail](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md) des contacts. Marketo effectue également une référence croisée à la base de données de prospects pour les désabonnements avant d’envoyer un e-mail.

## [!DNL Bizible] par Marketo

* **[!DNL Bizible]Découvrez les améliorations apportées aux fonctionnalités** : les nouvelles fonctionnalités de segmentation des tableaux de bord permettent aux professionnels du marketing de mieux comprendre les performances.
* **Prise en charge multidevise** : basculez entre la devise de votre entreprise et toute devise locale grâce à la nouvelle fonctionnalité de conversion automatique de devise de [!DNL Bizible], reposant sur des tables de devises CRM.
* **Coûts de campagne CRM** : mesurez les dépenses et le retour sur investissement des activités de marketing hors ligne avec la possibilité d’extraire automatiquement les données de coût de l’objet de campagne CRM.

## Juin 2019 {#june}

Les fonctionnalités suivantes sont incluses dans la version du 19 juin. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

**_Versions trimestrielles_**

Les fonctionnalités suivantes ont été publiées le 14 juin 2019.

## Services principaux Marketo {#marketo-core-services}

* **Somme de contrôle d’extraction de fichier en bloc** : vérifiez qu’un fichier complet a été récupéré en comparant votre hachage de fichier à la chaîne de somme de contrôle de vos tâches d’extraction terminées.
* **Migration automatisée de la version Email 1.0 vers la version Email 2.0** : la version Email 2.0 est entièrement compatible avec les e-mails et les modèles Email 1.0. Profitez des nouvelles fonctionnalités, telles que la possibilité de regrouper des éléments de contenu (images, texte, etc.) dans les modules , définissez des variables telles que Chaîne, Couleur, Image, etc. dans les modèles et exploitez les modèles de démarrage entièrement réactifs. Comprend également un sélecteur visuel de modèle d’e-mail.

>[!CAUTION]
>
>Depuis le 18 juin 2019, l’e-mail 1.0 n’est plus disponible. Vous pouvez en savoir plus sur Email 2.0 et l’obsolescence d’Email 1.0 [ici](https://nation.marketo.com/docs/DOC-7038).

## Account-Based Marketing

* **[!DNL LinkedIn]Account Matching (BETA)** : une nouvelle fonctionnalité d’ABM est désormais disponible en version bêta, vous permettant d’envoyer des listes de comptes connus et d’espaces blancs directement de Marketo vers LinkedIn. Cette fonctionnalité est automatiquement incluse pour tous les clients Marketo ABM.

<br> 

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes devraient sortir au cours du deuxième trimestre civil et au début du troisième trimestre de 2019.

## [!DNL Marketo Sky]

* **Limites d’événement** et **Objectifs d’événement** sont généralement disponibles dans [!DNL Marketo Sky] sous le module complémentaire Événements Premium .

   * Limites d’événement : optimisez l’expérience client pour vos événements et webinaires avec des limites d’enregistrement, des redirections de page et une fonctionnalité de liste d’attente.
   * Objectifs de l’événement : définissez des objectifs d’inscription et de participation à l’événement et suivez la progression en temps réel.

* **Liens de navigation complets** : nous avons activé la navigation vers toutes les applications autorisées, telles que Hootsuite, Calendrier, etc.
* **Vues E-mail, Page de destination, Extrait de code, Formulaire, Image et Liste de fichiers** : affichez, recherchez et effectuez des actions en masse sur l’une de vos ressources dans Design Studio.
* **Page d’informations sur l’image, le fichier et le fragment de code** : obtenez des informations rapides sur vos ressources avec des métadonnées telles que _créées à/par_ et des actions telles que _supprimer_ et _approuver_.
* **Widget Publications du blog de la communauté** : accédez aux publications récentes de la communauté dans My Marketo.
* **Widget bientôt expiré** : ajoutez le widget « bientôt expiré » à votre tableau de bord Mon Marketo pour voir quelles campagnes et pages de destination vont bientôt expirer.
* **Plus de cartes de liste dynamique** : segmentez et ciblez de manière appropriée avec des cartes de liste dynamique supplémentaires, y compris l’étape de flux « Créer une tâche », les règles de liste dynamique CRM, etc.
* **Page d’informations sur le champion/challenger d’e-mail** : consultez les données telles que les critères de réussite, les critères créés à l’adresse, etc. issues de vos tests de champion/challenger d’e-mail.

## Marketo [!DNL Sales Connect] {#marketo-sales-connect}

* **Actions en bloc dans la personnalisation [!DNL Salesforce] campagnes** : optimisez la productivité en envoyant des e-mails et en ajoutant des contacts aux campagnes en bloc avec la personnalisation [!DNL Salesforce].
* **Paramètres - Page [!DNL Salesforce] pour les administrateurs et les non-administrateurs** : gérez votre instance [!DNL Sales Connect] avec une vue claire de l’instance [!DNL Salesforce] connectée à [!DNL Sales Connect], ainsi que Mon e-mail pour [!DNL Salesforce] les mises à jour. Les paramètres de synchronisation améliorés pour les administrateurs, les non-administrateurs et la synchronisation à l’échelle de l’équipe seront publiés au cours des prochains mois.
* **Paramètres - Page d’intégration** : guichet unique pour toutes vos intégrations, afin que vous puissiez tirer le meilleur parti de notre écosystème ouvert.
* **Paramètres - Page de profil** : affichez et mettez à jour les détails de votre compte, modifiez votre mot de passe et vérifiez le statut de l’implémentation de votre instance sur cette nouvelle page de profil.

* **Modèles de courrier électronique système** : mise à jour des fonctionnalités de conception, de réactivité et d’internationalisation.

## [!DNL Bizible] par Marketo

* **Prise en charge multidevise pour les[!DNL Dynamics]** : [!DNL Bizible] s’adapte désormais aux tables de devises [!DNL Microsoft Dynamics], afin que vous puissiez facilement basculer entre les devises d’entreprise et locales. (Remarque : la prise en charge de SFDC a été publiée au 1er trimestre 2019.)
* **Intégration de Drift** : découvrez comment les conversations Drift affectent le parcours de votre client. [!DNL Bizible] extraira également les adresses e-mail des conversations pour créer un nouveau prospect ou connecter le point de contact à un prospect existant.
* **Localisation** : [!DNL Bizible] est désormais disponible dans toutes les langues prises en charge par Marketo (anglais, japonais, allemand, espagnol, français et portugais).

_**Webinaire de mise à jour des produits**_ Regardez l’enregistrement de notre webinaire sur les innovations de mise à jour du 19 juin [ici](https://engage.marketo.com/Marketo-June-Product-Release-2019-On-Demand.html).

## Août 2019 {#august}

Les fonctionnalités suivantes sont incluses dans la version du 19 août. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

**_Versions trimestrielles_**

Les fonctionnalités suivantes ont été publiées le 16 août 2019.

## Engagement Marketo de base {#core-marketo-engage}

* **Framework de webinaire extensible** : gagnez du temps avec le nouveau framework de webinaire prêt à l’emploi de Marketo (introduit dans les notes de mise à jour de l’hiver 19) qui transmet en toute transparence les données des fournisseurs de webinaires à Marketo et vice versa. Cvent et Zoom sont désormais disponibles dans ce nouveau framework.
* **Mise à jour de l’API Smart Campaign** : gérez les fonctionnalités de cycle de vie des campagnes intelligentes tout en complétant l’interface CRUD (création, lecture, mise à jour, suppression).
* **Modification de l’API Update Email Headers** : l’API Update Email Header ne nécessite plus qu’un e-mail soit associé à un modèle pour mettre à jour les champs d’en-tête, tels que l’objet.

**** ![(étoile)](assets/yellow-star.png)

* **[!DNL LinkedIn]correspondance de compte** auparavant en version Beta, est désormais disponible pour tous.
* **AccountAI** est officiellement rebaptisé **Profil de compte**.

<br> 

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes sont publiées selon un cycle non trimestriel et seront publiées tout au long du troisième trimestre civil et au début du 4e trimestre 2019.

**[!DNL Marketo Sales Connect]** ![(étoile)](assets/yellow-star.png)

* **Amélioration de la mise en page des personnes :** gérez vos personnes et vos groupes par le biais d’importations de listes et d’actions en bloc dans la nouvelle mise en page des personnes.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile ( ![(étoile)](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo pour en savoir plus.

>[!NOTE]
>
>**Obsolescence de TLS 1.0 et 1.1** : pour nous aligner sur les normes de sécurité internationales d’Adobe, nous allons abandonner la prise en charge de TLS (Transport Layer Security) 1.0 et 1.1 à compter du 13 décembre 2019. Les systèmes s’intégrant à Marketo et non conformes au protocole 1.2 peuvent perdre l’accès aux services Marketo Engage.
>
>**Pour conserver votre accès à Marketo Engage, assurez-vous que tous les systèmes clients sont conformes au protocole TLS 1.2 avant le 13 décembre 2019**. Vous trouverez de plus amples informations [ici](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).

**_Webinaire de mise à jour du produit_** [Rejoignez-nous](https://engage.marketo.com/August_19_Release_Webinar.html) le 28 août à 1:00PM PT / 4:00PM ET pour un webinaire en direct hébergé par notre équipe produit et découvrez en détail les fonctionnalités incluses dans cette version.

