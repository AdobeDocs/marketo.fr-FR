---
description: FAQ sur Adobe Identity Management - Documentation de Marketo - Documentation du produit
title: FAQ sur Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 0%

---

# FAQ sur Adobe Identity Management {#adobe-identity-management-faq}

**Qu’est-ce que l’identité d’Adobe ?**

Le système Adobe Identity Management se compose de trois composants.

* [!DNL Adobe Identity Service] : gère l’authentification et la validation de l’utilisateur final, y compris la fédération et l’authentification unique (SSO) à l’exécution.

* Adobe Admin Console : l’Admin Console fournit un emplacement central pour la gestion des droits à l’Adobe dans l’ensemble de votre organisation. Il gère la gestion des utilisateurs, le service cloud, les droits de licence pour ordinateurs de bureau, la configuration des fédérations et fournit des fonctionnalités de sécurité pour la prévention des pertes de données.

* API User Management d’Adobe (UMAPI) : permet aux organisations de gérer les utilisateurs et les droits d’entreprise dans Adobe Admin Console au niveau de l’API.

**Quand les abonnements de Marketo Engage existants seront-ils intégrés à IMS ?**

Les abonnements de Marketo Engage existants sont actuellement migrés vers Adobe IMS lors de tout événement de vente, qui inclut les renouvellements, les événements de réattribution de contrat et/ou les addenda. Les migrations en dehors d’un événement de vente sont désormais prises en charge à compter d’octobre 2024.

**Après la migration, les URL du Marketo Engage resteront-elles les mêmes ?**

Non. Les URL auront un aspect différent après la migration.

**Devons-nous faire quelque chose pour préparer le changement d’URL ?**

Oui. Après la migration, Marketo Engage ne sera plus diffusée depuis experience.adobe.com vers Adobe Experience Cloud. Vous devrez travailler avec votre équipe informatique pour placer sur la liste autorisée tous les domaines Adobes répertoriés [au début de cet article](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} afin d’éviter toute interruption de l’accès au Marketo Engage.

Les liens et signets précédents vers les ressources du Marketo Engage sur le domaine engage-xx.marketo.com _continueront_ à fonctionner. Cependant, vous devez d’abord vous connecter à l’instance du Marketo Engage pour l’URL à laquelle vous accédez. Par exemple, pour accéder à un signet pour une campagne dynamique dans une instance avec l’ID de Munchkin 123-ABC-456, vous devez d’abord vous connecter à l’instance de Marketo Engage avec l’ID de Munchkin 123-ABC-456.

**Quelle est la différence entre un administrateur de produit Adobe et un administrateur de Marketo Engage ?**

* Adobe Product Admin est un nouveau rôle de la plateforme Marketo.
* Le rôle d’administrateur de produit Adobe est accordé aux utilisateurs ajoutés en tant qu’administrateur de produit dans Adobe Admin Console
* Adobe Product Admin est un rôle en lecture seule qui ne peut pas être modifié ni supprimé du Marketo Engage.
* Adobe Product Admin dispose des mêmes droits et privilèges qu’un administrateur Marketo standard.
* Le rôle d’administrateur de Marketo Engage reste un rôle d’administrateur. Il est attribué à un utilisateur dans Marketo Engage.

**La prise en charge du client de l’API User Management a-t-elle changé ?**

Oui. Ceux qui ont intégré Adobe IMS ne peuvent pas utiliser toutes les API User Management de Marketo existantes. Pour les actions d’invitation, de mise à jour et de suppression des utilisateurs, l’Adobe [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} doit être utilisé. Pour la gestion des rôles, les API User Management de Marketo s’appliquent toujours. En dehors de cela, il n’y a aucune autre modification de la prise en charge du client API REST Marketo.

**Qui contacter pour obtenir de l’aide si nous sommes intégrés à IMS ?**

* Migration des pré-utilisateurs : déposer les cas d’assistance dans la [Communauté de la nation marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou `customercare@marketo.com` par e-mail.

* Migration après l’utilisateur ou l’utilisatrice : consignez les cas d’assistance dans la [Communauté de la nation marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou `customercare@marketo.com` par e-mail.

* Fin de la migration après assistance : les administrateurs de l’assistance produit peuvent déposer des cas via le portail d’assistance Experience League.

Si vous disposez d’Ultimate Success, vous avez accès au service de gants blancs Migration Admin Console . Contactez l’équipe du compte d’Adobe (votre gestionnaire de compte) pour obtenir de l’aide.

**Si j’utilise une identité d’Adobe pour accéder à d’autres applications d’Adobe, puis-je l’utiliser pour accéder à Marketo ?**

Même si vous disposez d’autres produits Adobes, vous ne pouvez pas accéder à Marketo avec une identité Adobe tant que l’abonnement n’a pas été migré vers IMS.

**Les rôles utilisateur de Marketo (dans les espaces de travail) sont-ils gérés dans Adobe Admin Console ?**

Non. La gestion des rôles utilisateur (dans les espaces de travail) s’est terminée dans Marketo Engage.

**Je suis un administrateur Marketo dans un abonnement intégré IMS et je n’ai pas accès à l’Admin Console. Comment puis-je y accéder ?**

Tout administrateur système ou produit d’Adobe ayant accès à l’Admin Console de votre organisation peut vous y accorder l’accès. Si vous ne savez pas qui, dans votre organisation, dispose de privilèges d’administrateur dans la console, contactez l’Assistance clientèle d’Adobe [](https://helpx.adobe.com/contact.html){target="_blank"}.

**Comment un administrateur ajouterait-il des utilisateurs aux [!DNL Sales Connect] Marketo ?**

Bien qu’il y ait une fiche produit dans Admin Console pour [!DNL Sales Connect], Admin Console ne doit pas être utilisé pour ajouter/gérer des utilisateurs. Le lien suivant permet aux administrateurs de gérer les utilisateurs via Marketo [!DNL Sales Connect] : [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Où puis-je en savoir plus sur le Adobe Admin Console ?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/fr/enterprise/admin-guide.html){target="_blank"}.

**Dois-je toujours accéder à la section Admin de Marketo pour apporter des modifications au compte utilisateur de mon compte ?**

Non, vous devez accéder à [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Comment cela fonctionne-t-il avec l’identifiant universel Marketo ?**

Les personnes intégrées à l’identité d’Adobe peuvent accéder facilement à tous les abonnements compatibles IMS via le sélecteur d’abonnements du produit.

**Cela fonctionne-t-il avec l’authentification unique ?**

Oui. L’intégration de Marketo à Adobe IMS prend en charge les utilisateurs d’Universal ID et la connexion unique. La connexion unique est désormais gérée par Adobe IMS et configurée au niveau de l’organisation dans Adobe Admin Console. [En savoir plus ici](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

**J’ai déjà été intégré à Adobe Identity et je veux maintenant implémenter SSO. Qu&#39;est-ce que je fais ?**

Si vous souhaitez implémenter l’authentification unique et que votre abonnement a été intégré à l’identité d’Adobe sans que la connexion unique soit implémentée dans l’organisation d’Adobe, envoyez un ticket à l’assistance de [Marketo](https://nation.marketo.com/){target="_blank"} et indiquez la rubrique « Marketo sur Admin Console, implémentation de l’authentification unique ».

**Comment fonctionne l’autorisation des appareils ?**

Actuellement, Adobe IMS ne prend en charge aucune fonctionnalité telle que la fonction d’autorisation des appareils Marketo.

**Est-il toujours possible d’utiliser la fonction « Connexion à la boîte de dialogue d’invitation de l’utilisateur » pour rendre la connexion d’un utilisateur unique à partir de son e-mail ?**

Non. Le workflow d’invitation d’utilisateurs n’est plus actif lorsqu’un abonnement est activé pour IMS. La fonctionnalité n’est donc plus valide. L’identité d’Adobe nécessite que l’identité d’un utilisateur soit pilotée par son adresse e-mail.

**Pour Adobe IMS, avons-nous la possibilité d’utiliser Adobe ID, Enterprise ID ou Federated ID ?**

Oui, vous déterminez le type d’identité à prendre en charge par votre organisation. Vous trouverez plus d’informations ici : [Présentation des identités](https://helpx.adobe.com/fr/enterprise/using/identity.html) et ici : [Configurer les identités](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

**Quelles cartes produits sont prises en charge dans Adobe Admin Console ?**

Les cartes de produits prises en charge sont les suivantes : Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect et Marketo Sales Insight Actions.

**Que se passe-t-il si ma connexion utilisateur ne correspond pas à mon adresse e-mail lorsque je suis migré vers une identité Adobe ?**

Les utilisateurs actuels du Marketo Engage dont les comptes sont différents de leur adresse e-mail ne se connectent plus avec ces informations d’identification une fois migrés vers une identité d’Adobe. Les identités d’Adobe s’authentifient toujours à l’adresse e-mail d’un utilisateur. Vous pouvez mettre à jour une adresse e-mail d’identité Adobe à l’adresse [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Que se passe-t-il après la migration d’identité d’Adobe si mon abonnement utilise des paramètres de restriction IP ?**

Lorsque les abonnements sont intégrés à Adobe Identity, les paramètres de restriction d’adresses IP ne sont pas migrés vers Adobe Admin Console. Les paramètres de restriction IP de Marketo incluent l’autorisation d’accès à partir d’adresses IP spécifiques uniquement et le blocage de l’accès à partir d’adresses IP spécifiques. Actuellement, le système Identity Management d’Adobe ne prend pas en charge les fonctionnalités de restriction d’adresses IP.

Début 2025, Adobe Identity Management System proposera une fonctionnalité permettant de n’autoriser que des adresses IP spécifiques, prenant ainsi en charge une transition pour les utilisateurs de Marketo qui utilisent actuellement cette fonctionnalité. Les utilisateurs et utilisatrices qui utilisent actuellement cette fonctionnalité ne seront pas soumis à la migration des utilisateurs et utilisatrices tant que la fonctionnalité ne sera pas publiée. Une fois la fonctionnalité diffusée, les utilisateurs sont avertis de la planification de leur migration. Des informations supplémentaires sur la fonctionnalité seront fournies lorsqu’elles seront disponibles.

Les utilisateurs qui utilisent actuellement la restriction d’adresse IP, bloquant l’accès à des adresses spécifiques, ne pourront plus utiliser cette fonctionnalité après avoir migré vers l’identité d’Adobe, car elle n’est pas prise en charge par le système Identity Management d’Adobe.

**Que se passe-t-il après la migration d’identité d’Adobe si j’ai des utilisateurs dont le rôle offre la possibilité de « Contourner l’authentification SSO » ?**

Lorsque les abonnements sont intégrés à l’identité Adobe, l’authentification unique (SSO) est configurée au niveau de l’organisation Adobe pour tous les utilisateurs. Lorsque la connexion unique est configurée, elle est appliquée à tous les utilisateurs Marketo/toutes les instances Marketo de cette organisation d’Adobe. Auparavant, Marketo prenait en charge la possibilité de configurer un rôle d’utilisateur pour avoir la possibilité de « Contourner l’authentification SSO ». Ce n’est pas pris en charge par le système Identity Management d’Adobe.

**Je dispose de plusieurs abonnements, mais l’authentification SSO n’est pas activée pour tous. Que se passe-t-il après la migration d’identité d’Adobe ?**

Lorsque les abonnements sont intégrés à l’identité Adobe, l’authentification unique (SSO) est configurée au niveau de l’organisation Adobe. Cela signifie que la connexion unique s’applique à toutes les instances de produit dans l’organisation d’Adobe. Lorsque la connexion unique est configurée, elle s’applique à toutes les instances Marketo de cette organisation d’Adobe. Auparavant, Marketo prenait en charge ce paramètre au niveau de l’instance. Ce n’est pas pris en charge par le système Identity Management d’Adobe.

**Des modifications doivent-elles être apportées aux CNAME, SPF ou DKIM que nous utilisons actuellement pour Marketo Engage après la migration d’identité d’Adobe ?**

Non, ces configurations n’ont aucun impact.

**Comment empêcher les sessions d’expirer ?**

Dans [Paramètres avancés](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}, vous pouvez personnaliser la durée de vie maximale de la session souhaitée (autorisations d’administrateur système requises). Il est recommandé d’établir ce paramètre après la migration du produit, mais avant la migration des utilisateurs et utilisatrices.

**Je dois maintenant accéder à Experience Cloud pour accéder à Marketo Engage. Existe-t-il un moyen de rationaliser ce flux ?**

Oui. Vous pouvez créer un signet de navigateur du lien qui se lance après avoir cliqué sur le bouton **Lancer** sur la page d’entrée de l’instance de Marketo Engage afin de contourner cette page à l’avenir.

![](assets/faq-1.png)
