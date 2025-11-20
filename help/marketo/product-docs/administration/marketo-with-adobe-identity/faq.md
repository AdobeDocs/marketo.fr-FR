---
description: FAQ sur Adobe Identity Management - Documentation de Marketo - Documentation du produit
title: FAQ sur Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 95ed91736b7276dd7a5b9e09958c1f09832ae719
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 1%

---

# FAQ sur Adobe Identity Management {#adobe-identity-management-faq}

**Qu’est-ce qu’Adobe Identity ?**

Le système Adobe Identity Management se compose de trois composants.

* [!DNL Adobe Identity Service] : gère l’authentification et la validation de l’utilisateur final, y compris la fédération et l’authentification unique (SSO) à l’exécution.

* Adobe Admin Console : Admin Console fournit un emplacement central pour la gestion des droits Adobe dans l’ensemble de votre organisation. Il gère la gestion des utilisateurs, le service cloud, les droits de licence pour ordinateurs de bureau, la configuration des fédérations et fournit des fonctionnalités de sécurité pour la prévention des pertes de données.

* API User Management d’Adobe (UMAPI) : permet aux organisations de gérer les utilisateurs et les droits d’entreprise dans Adobe Admin Console au niveau de l’API.

**Quand les abonnements Marketo Engage existants seront-ils intégrés à IMS ?**

Les abonnements Marketo Engage existants sont actuellement migrés vers l’IMS Adobe lors de tout événement de vente, qui inclut les renouvellements, les événements de réattribution de contrat et/ou les addenda. Les migrations en dehors d’un événement de vente sont prises en charge à compter d’octobre 2024.

**Après la migration, les URL de Marketo Engage resteront-elles les mêmes ?**

Non. Les URL s’affichent au format suivant après la migration : `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (les XXX représentent l’identifiant Munchkin et @tenantID provient de votre organisation Adobe).

**Devons-nous faire quelque chose pour préparer le changement d’URL ?**

Oui. Après la migration, Marketo Engage ne sera plus diffusée depuis experience.adobe.com vers Adobe Experience Cloud. Vous devrez travailler avec votre équipe informatique pour placer sur la liste autorisée tous les domaines Adobe répertoriés [au début de cet article](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} afin d’éviter toute interruption de l’accès à Marketo Engage.

Les liens et signets précédents vers les ressources Marketo Engage sur le domaine engage-xx.marketo.com _continueront_ à fonctionner. Cependant, vous devez d’abord vous connecter à l’instance Marketo Engage pour l’URL à laquelle vous accédez. Par exemple, pour accéder à un signet pour une campagne dynamique dans l’instance avec l’identifiant Munchkin 123-ABC-456, vous devez d’abord vous connecter à l’instance Marketo Engage avec l’identifiant Munchkin 123-ABC-456.

Bien que cela ne soit pas prévu, les travaux de développement futurs peuvent rompre cette fonction de redirection. Pour éviter toute interruption inattendue, il est recommandé de mettre à jour les signets dès que possible.

**Cela fonctionne-t-il avec l’authentification unique ?**

Oui. L’intégration à Adobe IMS prend en charge les utilisateurs d’Universal ID et la connexion unique. La connexion unique est désormais gérée par Adobe IMS et configurée au niveau de l’organisation dans Adobe Admin Console. Cependant, il existe des différences dans la prise en charge initiée par Marketo Engage IdP par rapport à la prise en charge initiée par Adobe SP ([en savoir plus ici](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}). Si vous avez besoin d’aide concernant les différences d’authentification unique après la migration vers Admin Console, contactez l’[Assistance clientèle Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**Quelle est la différence entre un administrateur de produit Adobe et un administrateur Marketo Engage ?**

* Adobe Product Admin est un nouveau rôle de la plateforme Marketo.
* Le rôle d’administrateur de produit Adobe est accordé aux utilisateurs ajoutés en tant qu’administrateur de produit dans Adobe Admin Console
* L’administrateur de produit Adobe est un rôle en lecture seule et ne peut pas être modifié ni supprimé de Marketo Engage.
* L’administrateur de produit Adobe dispose des mêmes droits et privilèges qu’un administrateur Marketo standard.
* Le rôle d’administrateur Marketo Engage est toujours un rôle d’administrateur et est accordé à un utilisateur dans Marketo Engage.
* Seuls les utilisateurs avec le rôle d’administrateur par défaut de Marketo sont affectés en tant qu’administrateur de produit Marketo dans Admin Console.

**La prise en charge du client de l’API User Management a-t-elle changé ?**

Oui. Ceux qui ont intégré Adobe IMS ne peuvent pas utiliser toutes les API User Management de Marketo existantes. Pour les actions d’invitation, de mise à jour et de suppression des utilisateurs, les [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} d’Adobe doivent être utilisées. Pour la gestion des rôles, les API User Management de Marketo s’appliquent toujours. En dehors de cela, il n’y a aucune autre modification de la prise en charge du client API REST Marketo.

**Qui contacter pour obtenir de l’aide si nous sommes intégrés à IMS ?**

* Migration des pré-utilisateurs : déposer les cas d’assistance dans la [Communauté de la nation marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou `customercare@marketo.com` par e-mail.

* Migration après l’utilisateur ou l’utilisatrice : consignez les cas d’assistance dans la [Communauté de la nation marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou `customercare@marketo.com` par e-mail.

* Fin de la migration après assistance : les administrateurs de l’assistance produit peuvent déposer des cas via le portail d’assistance Experience League.

Si vous disposez d’Ultimate Success, vous avez accès au service de gant blanc de migration d’Admin Console. Contactez l’équipe du compte Adobe (votre gestionnaire de compte) pour obtenir de l’aide.

**Si j’utilise une Adobe Identity pour accéder à d’autres applications Adobe, puis-je l’utiliser pour accéder à Marketo ?**

Même si vous disposez d’autres produits Adobe, vous ne pouvez pas accéder à Marketo avec Adobe Identity tant que l’abonnement n’a pas été migré vers IMS.

**Les rôles utilisateur de Marketo (dans les espaces de travail) sont-ils gérés dans Adobe Admin Console ?**

Non. La gestion des rôles utilisateur (dans les espaces de travail) s’est terminée dans Marketo Engage.

**Je suis un administrateur Marketo dans un abonnement intégré à IMS et je n’ai pas accès à Admin Console. Comment puis-je y accéder ?**

Tout administrateur système ou produit Adobe ayant accès à l’Admin Console de votre organisation peut vous y accorder l’accès. Si vous ne savez pas qui, dans votre organisation, dispose de privilèges d’administrateur dans la console, contactez l’[Assistance clientèle Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**Comment un administrateur ajouterait-il des utilisateurs aux [!DNL Sales Connect] Marketo ?**

Bien qu’il y ait une carte de produit dans Admin Console pour [!DNL Sales Connect], Admin Console ne doit pas être utilisé pour ajouter/gérer des utilisateurs. Le lien suivant permet aux administrateurs de gérer les utilisateurs via Marketo [!DNL Sales Connect] : [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Où puis-je en savoir plus sur le Adobe Admin Console ?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/fr/enterprise/admin-guide.html){target="_blank"}.

**Dois-je toujours accéder à la section Admin de Marketo pour apporter des modifications au compte utilisateur de mon compte ?**

Non, vous devez accéder à [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Comment cela fonctionne-t-il avec l’identifiant universel Marketo ?**

Les personnes intégrées à l’identité Adobe peuvent accéder facilement à tous les abonnements compatibles IMS via le sélecteur d’abonnements du produit.

**Cela fonctionne-t-il avec l’authentification unique ?**

Oui. L’intégration de Marketo à Adobe IMS prend en charge les utilisateurs d’Universal ID et la connexion unique. La connexion unique est désormais gérée par Adobe IMS et configurée au niveau de l’organisation dans Adobe Admin Console. [En savoir plus ici](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

**J’ai déjà intégré Adobe Identity et je souhaite maintenant implémenter SSO. Qu&#39;est-ce que je fais ?**

Si vous souhaitez implémenter l’authentification unique et que votre abonnement a été intégré à Adobe Identity sans que la connexion unique ne soit implémentée dans l’organisation Adobe, envoyez un ticket à l’assistance de [Marketo](https://nation.marketo.com/){target="_blank"} et indiquez la rubrique « Marketo sur Admin Console, implémentation de l’authentification unique ».

**Comment fonctionne l’autorisation des appareils ?**

Actuellement, Adobe IMS ne prend en charge aucune fonctionnalité telle que la fonction d’autorisation des appareils Marketo.

**Est-il toujours possible d’utiliser la fonction « Connexion à la boîte de dialogue d’invitation de l’utilisateur » pour rendre la connexion d’un utilisateur unique à partir de son e-mail ?**

Non. Le workflow d’invitation d’utilisateurs n’est plus actif lorsqu’un abonnement est activé pour IMS. La fonctionnalité n’est donc plus valide. L’identité Adobe nécessite que l’identité d’un utilisateur soit pilotée par son adresse e-mail.

**Pour Adobe IMS, avons-nous la possibilité d’utiliser Adobe ID, Enterprise ID ou Federated ID ?**

Oui, vous déterminez le type d’identité à prendre en charge par votre organisation. Vous trouverez plus d’informations ici : [Présentation des identités](https://helpx.adobe.com/fr/enterprise/using/identity.html) et ici : [Configurer les identités](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

**Quelles cartes produits sont prises en charge dans Adobe Admin Console ?**

Les cartes de produits prises en charge sont les suivantes : Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect et Marketo Sales Insight Actions.

**Que se passe-t-il si ma connexion utilisateur ne correspond pas à mon adresse e-mail lorsque je suis migré vers une identité Adobe ?**

Les utilisateurs Marketo Engage actuels dont les comptes sont différents de leur adresse e-mail ne se connecteront plus avec ces informations d’identification une fois la migration vers une identité Adobe effectuée. Les identités Adobe s’authentifient toujours à l’adresse e-mail d’un utilisateur. Vous pouvez mettre à jour une adresse e-mail d’identité Adobe à l’adresse [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Que se passe-t-il après la migration d’Adobe Identity si mon abonnement utilise des paramètres de restriction IP ?**

Vos restrictions d’adresses IP actuelles resteront actives jusqu’au premier trimestre 2026 (cela s’applique aux abonnements pour lesquels elles étaient activées avant la migration). Ces restrictions s’appliqueront également aux utilisateurs d’Adobe ID. Vos contrôles d’accès continueront donc à fonctionner comme prévu.

À compter du 1er trimestre 2026, les restrictions IP héritées seront supprimées. À partir de là, l’accès basé sur les adresses IP sera géré exclusivement dans le Adobe Admin Console (AAC). Pour maintenir un accès sécurisé, vous devez configurer les restrictions IP dans AAC. Pour plus d&#39;informations, consultez cet article de blog [ Marketing Nation ](https://nation.marketo.com/t5/product-blogs/updated-important-update-ip-restrictions-feature-transition/ba-p/358420){target="_blank"}.

**Que se passe-t-il après la migration de l’identité Adobe si j’ai des utilisateurs dont le rôle offre la possibilité de « Contourner l’authentification SSO » ?**

Adobe Admin Console s’accompagne d’un répertoire Business ID par défaut. Les utilisateurs situés en dehors des domaines déclarés dans les répertoires Federated ID d’une organisation Adobe seront affectés à ce répertoire avec un type d’identité Adobe ID. Ces utilisateurs pourront accéder à Marketo Engage sans passer par l’authentification unique (SSO) et la propriété de la licence restera la société, et non les individus.

**Je dispose de plusieurs abonnements, mais l’authentification SSO n’est pas activée pour tous. Que se passe-t-il après la migration d’Adobe Identity ?**

Lorsque les abonnements sont intégrés à Adobe Identity, l’authentification unique (SSO) est configurée au niveau de l’organisation Adobe. Cela signifie que la connexion unique s’applique à toutes les instances de produit dans l’organisation Adobe. Lorsque la connexion unique est configurée, elle s’applique à toutes les instances Marketo de cette organisation Adobe. Auparavant, Marketo prenait en charge ce paramètre au niveau de l’instance. Ce n’est pas pris en charge par le système Adobe Identity Management.

**Des modifications doivent-elles être apportées aux CNAME, SPF ou DKIM que nous utilisons actuellement pour Marketo Engage après la migration d’Adobe Identity ?**

Non, ces configurations n’ont aucun impact.

**Comment empêcher les sessions d’expirer ?**

Dans [Paramètres avancés](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}, vous pouvez personnaliser la durée de vie maximale de la session souhaitée (autorisations d’administrateur système requises). Il est recommandé d’établir ce paramètre après la migration du produit, mais avant la migration des utilisateurs et utilisatrices.

**Je dois maintenant accéder à Experience Cloud pour accéder à Marketo Engage. Existe-t-il un moyen de rationaliser ce flux ?**

Oui. Vous pouvez créer un signet de navigateur du lien qui se lance après avoir cliqué sur le bouton **Lancer** sur la page d’entrée de l’instance Marketo Engage afin de contourner cette page à l’avenir.

![](assets/faq-1.png)
