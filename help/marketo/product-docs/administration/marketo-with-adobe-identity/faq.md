---
description: FAQ sur Adobe Identity Management - Documentation Marketo - Documentation du produit
title: FAQ sur Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 525417cc289d918f6ff8038c1c293f5c4aca0f9c
workflow-type: tm+mt
source-wordcount: '1484'
ht-degree: 0%

---

# FAQ sur Adobe Identity Management {#adobe-identity-management-faq}

**Qu’est-ce que l’identité de l’Adobe ?**

Adobe Identity Management System se compose de trois composants.

* [!DNL Adobe Identity Service] : gère l’authentification et la validation de l’utilisateur final, y compris la fédération et l’authentification unique (SSO) au moment de l’exécution.

* Adobe Admin Console : l’Admin Console fournit un emplacement central pour la gestion des droits d’Adobe dans l’ensemble de votre organisation. Il gère la gestion des utilisateurs, le service cloud, les droits de licence de bureau, la configuration de fédération et fournit des fonctionnalités de sécurité de prévention des pertes de données.

* API Adobe User Management (UMAPI) : permet aux entreprises de gérer les utilisateurs et les droits des entreprises dans Adobe Admin Console au niveau de l’API.

**Quand les abonnements de Marketo Engage existants seront-ils intégrés à IMS ?**

Les abonnements de Marketo Engage existants sont actuellement migrés vers Adobe IMS lors de tout événement de vente, qui comprend les renouvellements, les événements de réattribution et/ou les addendums. Les migrations en dehors d’un événement commercial sont désormais prises en charge à compter d’octobre 2024.

**Après la migration, les URL de Marketo Engage resteront-elles identiques ?**

Non. Les URL auront un aspect différent après la migration.

**Y a-t-il quelque chose que nous devons faire pour préparer le changement d’URL ?**

Oui. Après la migration, le Marketo Engage passe de experience.adobe.com à Adobe Experience Cloud. Vous devrez travailler avec votre équipe informatique pour placer sur la liste autorisée tous les domaines d’Adobe répertoriés [ en haut de cet article ](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} afin d’éviter toute interruption de l’accès des Marketo Engage.

Les liens et signets précédents vers les ressources de Marketo Engage sur le domaine engage-xx.marketo.com _continueront à fonctionner._ Cependant, vous devez d’abord vous connecter à l’instance de Marketo Engage pour l’URL à laquelle vous accédez. Par exemple, pour accéder à un signet pour une campagne dynamique avec l’ID Munchkin 123-ABC-456, vous devez d’abord vous connecter à l’instance de Marketo Engage avec l’ID Munchkin 123-ABC-456.

**Quelle est la différence entre un administrateur de produit Adobe et un administrateur de Marketo Engage ?**

* L’administrateur de produit Adobe est un nouveau rôle dans la plateforme Marketo.
* Le rôle Administrateur de produit Adobe est attribué aux utilisateurs ajoutés en tant qu’administrateur de produit dans Adobe Admin Console
* L’administrateur de produit Adobe est un rôle en lecture seule qui ne peut pas être modifié ni supprimé de Marketo Engage.
* L’administrateur de produit Adobe dispose des mêmes droits et privilèges qu’un administrateur Marketo standard.
* Le rôle d’administrateur du Marketo Engage est toujours un administrateur et est attribué à un utilisateur en Marketo Engage.

**La prise en charge du client de l’API de gestion des utilisateurs a-t-elle changé ?**

Oui. Ceux qui ont été intégrés à Adobe IMS ne peuvent pas utiliser toutes les API de gestion des utilisateurs Marketo existantes. Pour les actions d’invitation, de mise à jour et de suppression de l’utilisateur, l’Adobe [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} doit être utilisé. Pour la gestion des rôles, les API de gestion des utilisateurs de Marketo s’appliquent toujours. En outre, aucune autre modification n’est apportée à la prise en charge des clients de l’API REST Marketo.

**Qui contactez l’assistance si nous sommes intégrés à IMS ?**

* Migration des pré-utilisateurs : cas de prise en charge des fichiers dans la [communauté Marketing Nation](https://nation.marketo.com/t5/support/ct-p/Support) ou l’e-mail `customercare@marketo.com`.

* Migration des post-utilisateurs : cas de prise en charge des fichiers dans la [communauté Marketing Nation](https://nation.marketo.com/t5/support/ct-p/Support) ou l’e-mail `customercare@marketo.com`.

* Fin de la migration après la prise en charge : les administrateurs du support produit peuvent archiver des dossiers via le portail du support Experience League.

Si vous obtenez une réussite finale, vous avez accès au service Gant blanc de migration Admin Console. Contactez l’équipe Compte d’Adobe (votre gestionnaire de compte) pour obtenir de l’aide.

**Si j’utilise une identité d’Adobe pour accéder à d’autres applications d’Adobe, puis-je l’utiliser pour accéder à Marketo ?**

Même si vous disposez d’autres produits Adobe, vous ne pouvez pas accéder à Marketo avec l’Adobe Identity tant que l’abonnement n’est pas migré vers IMS.

**Les rôles utilisateur Marketo (dans les espaces de travail) sont-ils gérés dans Adobe Admin Console ?**

Non. La gestion des rôles utilisateur (dans les espaces de travail) est effectuée dans Marketo Engage.

**Je suis administrateur Marketo dans un abonnement intégré IMS et n’ai pas accès à l’Admin Console. Comment puis-je y accéder ?**

Tout administrateur système d’Adobe ou de produit ayant accès à l’Admin Console de votre entreprise peut vous donner accès. Si vous ne savez pas qui dans votre organisation dispose des privilèges d’administrateur dans la console, contactez l’ [assistance clientèle d’Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**Comment un administrateur ajouterait-il des utilisateurs à Marketo [!DNL Sales Connect] ?**

Bien qu’il y ait une carte de produit dans Admin Console pour [!DNL Sales Connect], Admin Console ne doit pas être utilisé pour ajouter/gérer des utilisateurs. Le lien suivant permettra aux administrateurs de gérer les utilisateurs via Marketo [!DNL Sales Connect] : [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Où puis-je en apprendre davantage sur Adobe Admin Console ?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/fr/enterprise/admin-guide.html){target="_blank"}.

**Puis-je toujours accéder à la section Admin de Marketo pour apporter des modifications au compte utilisateur de mon compte ?**

Non, vous devez accéder à [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Comment cela fonctionne-t-il avec Marketo Universal ID ?**

Les personnes intégrées à l’identité Adobe peuvent accéder facilement à tous les abonnements activés pour IMS via le sélecteur d’abonnements du produit.

**Cela fonctionne-t-il avec SSO ?**

Oui. L’intégration de Marketo avec Adobe IMS prend en charge les utilisateurs d’ID universels et l’authentification unique. L’authentification unique est désormais pilotée par Adobe IMS et configurée au niveau de l’organisation dans Adobe Admin Console. [En savoir plus ici](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

**J’ai déjà été intégré à Adobe Identity et je souhaite maintenant mettre en oeuvre la connexion unique. Que faire ?**

Si vous souhaitez mettre en oeuvre l’authentification unique et que votre abonnement a été intégré à Adobe Identity sans que l’authentification unique soit mise en oeuvre dans l’organisation d’Adobe, envoyez un ticket à l’[Assistance Marketo](https://nation.marketo.com/){target="_blank"} et spécifiez la rubrique &quot;Marketo on Admin Console, implémentation de l’authentification unique&quot;.

**Comment fonctionne l’autorisation de périphérique ?**

Adobe IMS ne prend actuellement en charge rien de tel que la fonctionnalité d’autorisation des périphériques de Marketo.

**Est-il toujours possible d&#39;utiliser la fonction &quot;Boîte de dialogue d&#39;invitation de connexion&quot; pour rendre la connexion d&#39;un utilisateur unique à partir de son email ?**

Non. Le workflow d’invitation d’utilisateur n’est plus actif lorsqu’un abonnement est activé sur IMS. La fonctionnalité n’est donc plus valide. L’identité de l’Adobe nécessite que l’identité d’un utilisateur soit déterminée par son email.

**Pour Adobe IMS, avons-nous la possibilité d’utiliser Adobe ID, Enterprise ID ou Federated ID ?**

Oui, vous déterminez le type d’identité à prendre en charge par votre organisation. Vous trouverez plus d’informations ici : [Présentation des identités](https://helpx.adobe.com/fr/enterprise/using/identity.html) et ici : [Configuration de l’identité](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

**Quelles cartes de produits sont prises en charge dans Adobe Admin Console ?**

Les cartes de produits prises en charge sont les suivantes : Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect et Marketo Sales Insight Actions.

**Que se passe-t-il si ma connexion utilisateur ne correspond pas à mon adresse électronique lorsque je suis migrée vers une identité d’Adobe ?**

Les utilisateurs Marketo Engage actuels disposant de comptes différents de leur adresse électronique ne se connectent plus avec ces informations d’identification une fois migrées vers une identité d’Adobe. Les identités d’Adobe s’authentifient toujours avec l’adresse électronique d’un utilisateur. Vous pouvez mettre à jour une adresse électronique d’identité d’Adobe à l’adresse [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Que se passe-t-il après la migration des identités d’Adobe si mon abonnement utilise les paramètres de restriction d’IP ?**

Lorsque les abonnements sont intégrés à Adobe Identity, les paramètres de restriction d’IP ne sont pas migrés vers Adobe Admin Console. Les paramètres de restriction d’IP de Marketo incluent l’autorisation d’accès uniquement à partir d’adresses IP spécifiques et le blocage d’accès à des adresses IP spécifiques. Actuellement, Adobe Identity Management System ne prend pas en charge les fonctionnalités de restriction d’IP.

À compter du début de 2025, Adobe Identity Management System va sortir une fonctionnalité qui prendra en charge uniquement les adresses IP spécifiques, en prenant en charge une transition pour les utilisateurs Marketo qui utilisent cette fonctionnalité. Les utilisateurs qui utilisent actuellement cette fonctionnalité ne feront pas l’objet d’une migration de l’utilisateur tant qu’elle n’aura pas été publiée. Une fois la fonctionnalité fournie, les utilisateurs sont avertis de la planification de leur migration. Des informations supplémentaires sur la fonctionnalité seront fournies le cas échéant.

Les utilisateurs qui utilisent actuellement la restriction d’IP, empêchant l’accès à des adresses spécifiques, ne pourront plus utiliser cette fonctionnalité après avoir été migrés vers Adobe Identity, car elle n’est pas prise en charge par Adobe Identity Management System.

**Que se passe-t-il après la migration des identités d’Adobe si j’ai des utilisateurs avec un rôle qui a l’option &quot;Contourner l’authentification unique&quot; ?**

Lorsque les abonnements sont intégrés à Adobe Identity, l’authentification unique (SSO) est configurée au niveau de l’organisation Adobe pour tous les utilisateurs. Lorsque l’authentification unique est configurée, elle est appliquée à tous les utilisateurs Marketo/toutes les instances Marketo de cette organisation d’Adobe. Auparavant, Marketo prenait en charge l’autorisation de configurer un rôle utilisateur afin qu’il ait la possibilité de &quot;Contourner l’authentification unique&quot;. Ceci n’est pas pris en charge par Adobe Identity Management System.

**J’ai plusieurs abonnements, mais tous n’ont pas l’authentification unique activée. Que se passe-t-il après la migration des identités des Adobes ?**

Lorsque les abonnements sont intégrés à Adobe Identity, l’authentification unique (SSO) est configurée au niveau de l’organisation Adobe. Cela signifie que l’authentification unique s’applique à toutes les instances de produit dans l’organisation Adobe. Lorsque l’authentification unique est configurée, elle s’applique à toutes les instances Marketo de cette organisation d’Adobe. Auparavant, Marketo prenait en charge ce paramètre au niveau de l’instance. Cela n’est pas pris en charge par Adobe Identity Management System.

**Des modifications sont-elles nécessaires pour les CNAME, SPF ou DKIM que nous utilisons actuellement pour le Marketo Engage après la migration des identités d’Adobe ?**

Non, ces configurations n’ont aucun impact.

**Je dois maintenant accéder à Experience Cloud pour accéder à Marketo Engage. Y a-t-il un moyen de rationaliser ce flux ?**

Oui. Vous pouvez créer un signet de navigateur du lien qui se lance après avoir cliqué sur le bouton **Launch** sur la page d’entrée de l’instance de Marketo Engage pour contourner cette page.

![](assets/faq-1.png)
