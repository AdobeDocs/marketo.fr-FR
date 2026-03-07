---
description: Questions fréquentes sur Adobe Identity for Marketo Engage, y compris la migration, les URL, la fonction SSO, l’administration du produit par rapport à l’administration de Marketo, et les places sur la liste autorisée.
title: Questions fréquentes sur Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '1591'
ht-degree: 98%

---

# Questions fréquentes sur Adobe Identity Management {#adobe-identity-management-faq}

**Qu’est-ce qu’Adobe Identity ?**

Le système Adobe Identity Management se compose de trois éléments.

* [!DNL Adobe Identity Service] : gère l’authentification et la validation de l’utilisateur final ou de l’utilisatrice finale, y compris la fédération et l’authentification unique (SSO) à l’exécution.

* Adobe Admin Console : Admin Console permet de centraliser la gestion de vos droits Adobe à l’échelle de l’entreprise. Elle permet la gestion des utilisateurs et utilisatrices, du service cloud, des droits de licence pour ordinateurs de bureau, de la configuration des fédérations et fournit des fonctionnalités de sécurité pour la prévention des pertes de données.

* API User Management d’Adobe (UMAPI) : permet aux organisations de gérer les utilisateurs, les utilisatrices et les droits d’entreprise dans Adobe Admin Console au niveau de l’API.

**Quand les abonnements Marketo Engage existants seront-ils intégrés à IMS ?**

Les abonnements Marketo Engage existants sont actuellement migrés vers Adobe IMS lors de tout événement de vente, qui inclut les renouvellements, les événements de réattribution de contrat et/ou les addenda. Les migrations en dehors d’un événement de vente sont prises en charge à compter d’octobre 2024.

**Après la migration, les URL de Marketo Engage resteront-elles les mêmes ?**

Non. Les URL s’affichent au format suivant après la migration : `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (les XXX représentent l’identifiant Munchkin et le @tenantID provient de votre organisation Adobe).

**Devons-nous faire quelque chose pour préparer le changement d’URL ?**

Oui. Après la migration, Marketo Engage ne sera plus diffusé depuis experience.adobe.com, mais depuis Adobe Experience Cloud. Vous devrez travailler avec votre équipe informatique pour placer sur la liste autorisée tous les domaines Adobe répertoriés [au début de cet article](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} afin d’éviter toute interruption de l’accès à Marketo Engage.

Les liens et signets précédents vers les ressources Marketo Engage sur le domaine engage-xx.marketo.com _continueront_ à fonctionner. Cependant, vous devez d’abord vous connecter à l’instance Marketo Engage pour l’URL à laquelle vous accédez. Par exemple, pour accéder à un signet pour une campagne intelligente dans l’instance avec l’identifiant Munchkin 123-ABC-456, vous devez d’abord vous connecter à l’instance Marketo Engage avec l’identifiant Munchkin 123-ABC-456.

Bien que cela ne soit pas prévu, les futurs travaux de développement peuvent perturber cette fonction de redirection. Pour éviter toute interruption inattendue, il est recommandé de mettre à jour les signets dès que possible.

**Cela fonctionne-t-il avec l’authentification unique ?**

Oui. L’intégration à Adobe IMS prend en charge les utilisateurs et utilisatrices d’identifiants universels ainsi que l’authentification unique. L’authentification unique est désormais gérée par Adobe IMS et configurée au niveau de l’organisation dans Adobe Admin Console. Cependant, il existe des différences dans la prise en charge initiée par Marketo Engage IdP par rapport à la prise en charge initiée par le SP d’Adobe ([en savoir plus ici](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}). Si vous avez besoin d’aide concernant les différences d’authentification unique après la migration vers Admin Console, contactez l’[assistance clientèle Adobe](https://helpx.adobe.com/fr/contact.html){target="_blank"}.

**Quelle est la différence entre l’administrateur ou l’administratrice de produit Adobe et l’administrateur ou l’administratrice Marketo Engage ?**

* Administrateur ou administratrice de produit Adobe est un nouveau rôle de la plateforme Marketo.
* Le rôle d’administrateur ou d’administratrice de produit Adobe est accordé aux utilisateurs et utilisatrices en charge de l’administration de produit dans Adobe Admin Console.
* L’administrateur ou l’administratrice de produit Adobe est un rôle en lecture seule et ne peut pas être modifié ni supprimé dans Marketo Engage.
* L’administrateur ou l’administratrice de produit Adobe dispose des mêmes droits et privilèges qu’un administrateur ou une administratrice Marketo standard.
* Le rôle d’administrateur ou d’administratrice Marketo Engage est toujours un rôle d’administration et est accordé à un utilisateur ou une utilisatrice dans Marketo Engage.
* Seules les personnes avec le rôle d’administrateur ou d’administratrice par défaut de Marketo sont affectées en tant qu’administrateur ou administratrice de produit Marketo dans Admin Console.

**La prise en charge du client de l’API User Management a-t-elle changé ?**

Oui. Les personnes qui ont intégré Adobe IMS ne peuvent pas utiliser toutes les API User Management de Marketo existantes. Pour les actions d’invitation, de mise à jour et de suppression des utilisateurs et utilisatrices, vous devez utiliser les [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} d’Adobe. Pour la gestion des rôles, les API User Management de Marketo s’appliquent toujours. En dehors de cela, il n’y a aucune autre modification de la prise en charge du client API REST Marketo.

**Qui contacter pour obtenir de l’aide si nous sommes intégrés à IMS ?**

* Avant la migration de l’utilisateur ou de l’utilisatrice : consignez les tickets d’assistance auprès de la [communauté Marketing Nation](https://nation.marketo.com/t5/support/ct-p/Support) ou envoyez un e-mail à l’adresse `customercare@marketo.com`.

* Après la migration de l’utilisateur ou de l’utilisatrice : consignez les tickets d’assistance auprès de la [communauté Marketing Nation](https://nation.marketo.com/t5/support/ct-p/Support) ou envoyez un e-mail à l’adresse `customercare@marketo.com`.

* Après la fin de la migration : les administrateurs et administratrices de l’assistance produit peuvent consigner des tickets via le portail d’assistance Experience League.

Si vous disposez d’Ultimate Success, vous avez accès au service de migration premium d’Admin Console. Contactez l’équipe Adobe en charge des comptes (votre gestionnaire de compte) pour obtenir de l’aide.

**Si j’utilise Adobe Identity pour accéder à d’autres applications Adobe, puis-je l’utiliser pour accéder à Marketo ?**

Même si vous disposez d’autres produits Adobe, vous ne pouvez pas accéder à Marketo avec Adobe Identity tant que l’abonnement n’a pas été migré vers IMS.

**Les rôles d’utilisateur ou d’utilisatrice de Marketo (dans les espaces de travail) sont-ils gérés dans Adobe Admin Console ?**

Non. La gestion des rôles d’utilisateur ou d’utilisatrice (dans les espaces de travail) s’effectue dans Marketo Engage.

**Je suis en charge de l’administration Marketo dans un abonnement intégré à IMS et je n’ai pas accès à Admin Console. Comment puis-je y accéder ?**

Tous les administrateurs et administratrices système ou produit Adobe ayant accès à l’Admin Console de votre organisation peut vous y accorder l’accès. Si vous ne savez pas qui, dans votre organisation, dispose de privilèges d’administration dans la console, contactez l’[assistance clientèle Adobe](https://helpx.adobe.com/fr/contact.html){target="_blank"}.

**Comment un administrateur ou une administratrice ajoute des utilisateurs et utilisatrices à Marketo[!DNL Sales Connect] ?**

Bien qu’il y ait une carte de produit dans Admin Console pour [!DNL Sales Connect], Admin Console ne doit pas être utilisée pour ajouter/gérer des utilisateurs et utilisatrices. Le lien suivant permet aux administrateurs et administratrices de gérer les utilisateurs et utilisatrices via Marketo [!DNL Sales Connect] : [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Où puis-je en savoir plus sur Adobe Admin Console ?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/fr/enterprise/admin-guide.html){target="_blank"}.

**Dois-je toujours accéder à la section Admin de Marketo pour apporter des modifications au compte d’utilisateur ou d’utilisatrice de mon compte ?**

Non, vous devez accéder à [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Comment cela fonctionne-t-il avec l’identifiant universel Marketo ?**

Les personnes intégrées à Adobe Identity peuvent accéder facilement à tous les abonnements compatibles avec IMS via le sélecteur d’abonnements du produit.

**Cela fonctionne-t-il avec l’authentification unique ?**

Oui. L’intégration de Marketo à Adobe IMS prend en charge les utilisateurs et utilisatrices d’identifiants universels ainsi que l’authentification unique. L’authentification unique est désormais gérée par Adobe IMS et configurée au niveau de l’organisation dans Adobe Admin Console. [En savoir plus ici](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

**J’ai déjà intégré Adobe Identity et je souhaite maintenant implémenter l’authentification unique. Que dois-je faire ?**

Si vous souhaitez implémenter l’authentification unique et que votre abonnement a été intégré à Adobe Identity sans que l’authentification unique ne soit implémentée dans l’organisation Adobe, envoyez un ticket à l’[assistance de Marketo](https://nation.marketo.com/){target="_blank"} et indiquez la rubrique « Marketo sur Admin Console, implémentation de l’authentification unique ».

**Comment fonctionne l’autorisation des appareils ?**

Actuellement, Adobe IMS ne prend en charge aucune fonctionnalité semblable à la fonction d’autorisation des appareils Marketo.

**Est-il toujours possible d’utiliser la fonction « Connexion à la boîte de dialogue d’invitation de l’utilisateur ou de l’utilisatrice » pour rendre la connexion d’un utilisateur ou d’une utilisatrice unique à partir de son e-mail ?**

Non. Le workflow d’invitation d’utilisateur ou d’utilisatrice n’est plus actif lorsqu’un abonnement est activé pour IMS. La fonctionnalité n’est donc plus valide. Adobe Identity nécessite que l’identité d’un utilisateur ou d’une utilisatrice soit liée à son adresse e-mail.

**Pour Adobe IMS, avons-nous la possibilité d’utiliser Adobe ID, Enterprise ID ou Federated ID ?**

Oui, vous déterminez le type d’identité à prendre en charge par votre organisation. Vous trouverez plus d’informations ici : [Vue d’ensemble d’Identity](https://helpx.adobe.com/fr/enterprise/using/identity.html) et ici : [Configurer Identity](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

**Quelles cartes produits sont prises en charge dans Adobe Admin Console ?**

Les cartes de produits prises en charge sont les suivantes : Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect et Marketo Sales Insight Actions.

**Que se passe-t-il si ma connexion d’utilisateur ou d’utilisatrice ne correspond pas à mon adresse e-mail lors de ma migration vers Adobe Identity ?**

Les utilisateurs et utilisatrices Marketo Engage actuels dont les comptes sont différents de leur adresse e-mail ne se connecteront plus avec ces informations d’identification une fois la migration vers Adobe Identity effectuée. Les identités Adobe s’authentifient toujours à l’adresse e-mail d’un utilisateur ou d’une utilisatrice. Vous pouvez mettre à jour une adresse e-mail d’identité Adobe à l’adresse [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Que se passe-t-il après la migration d’Adobe Identity si mon abonnement utilise des paramètres de restriction d’adresses IP ?**

Vos restrictions d’adresses IP actuelles resteront actives durant le premier trimestre 2026 (cela s’applique aux abonnements pour lesquels elles étaient activées avant la migration). Ces restrictions s’appliqueront également aux utilisateurs et utilisatrices d’Adobe ID. Vos contrôles d’accès continueront donc à fonctionner comme prévu.

À compter du premier trimestre 2026, les restrictions d’adresses IP héritées seront supprimées. À partir de là, l’accès basé sur les adresses IP sera géré exclusivement dans Adobe Admin Console (AAC). Pour maintenir un accès sécurisé, vous devez configurer les restrictions IP dans AAC. Pour plus d’informations, consultez cet [article de blog de Marketing Nation](https://nation.marketo.com/t5/product-blogs/updated-important-update-ip-restrictions-feature-transition/ba-p/358420){target="_blank"}.

**Que se passe-t-il après la migration d’Adobe Identity si j’ai des utilisateurs et utilisatrices dont le rôle offre la possibilité de « Contourner l’authentification unique » ?**

Adobe Admin Console s’accompagne d’un répertoire d’identifiants d’entreprise par défaut. Les utilisateurs et utilisatrices en dehors des domaines déclarés dans les répertoires Federated ID d’une organisation Adobe seront affectés à ce répertoire avec un type d’identité Adobe ID. Ces utilisateurs et utilisatrices pourront accéder à Marketo Engage sans passer par l’authentification unique (SSO) et l’entreprise conservera la propriété de la licence, et non les personnes.

**Je dispose de plusieurs abonnements, mais l’authentification unique n’est pas activée pour tous. Que se passe-t-il après la migration d’Adobe Identity ?**

Lorsque les abonnements sont intégrés à Adobe Identity, l’authentification unique (SSO) est configurée au niveau de l’organisation Adobe. Cela signifie que l’authentification unique s’applique à toutes les instances de produit dans l’organisation Adobe. Lorsque l’authentification unique est configurée, elle s’applique à toutes les instances Marketo de cette organisation Adobe. Auparavant, Marketo prenait en charge ce paramètre au niveau de l’instance. Cela n’est pas pris en charge par le système Adobe Identity Management.

**Des modifications doivent-elles être apportées aux CNAME, SPF ou DKIM que nous utilisons actuellement pour Marketo Engage après la migration d’Adobe Identity ?**

Non, cela n’a aucun impact sur ces configurations.

**Comment empêcher les sessions d’expirer ?**

Dans [Paramètres avancés](https://helpx.adobe.com/fr/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}, vous pouvez personnaliser la durée de vie maximale de la session souhaitée (autorisations d’administration système requises). Il est recommandé d’établir ce paramètre après la migration du produit, mais avant la migration des utilisateurs et utilisatrices.

**Je dois maintenant naviguer jusqu’à Experience Cloud pour accéder à Marketo Engage. Existe-t-il un moyen de rationaliser ce flux ?**

Oui. Vous pouvez créer un signet de navigateur du lien qui se lance après avoir cliqué sur le bouton **Démarrer** sur la page d’entrée de l’instance Marketo Engage afin de contourner cette page à l’avenir.

![](assets/faq-1.png)
