---
description: Ce qui change lorsque les abonnements et les utilisateurs migrent vers Adobe Admin Console, notamment les rôles d’administrateur système et d’administrateur de produit, la connexion à l’aide d’Adobe Identity, les URL et le calendrier de migration.
title: Présentation de l’abonnement à Marketo et de la migration des utilisateurs et utilisatrices vers Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '1584'
ht-degree: 98%

---

# Présentation de l’abonnement à Marketo et de la migration des utilisateurs et utilisatrices vers Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe améliore la gestion de vos abonnements et de vos utilisateurs et utilisatrices Adobe Marketo Engage, ce qui accroît votre productivité et celle de votre entreprise. Dans le cadre de cette modification, Adobe effectue une migration de vos abonnements et de vos utilisateurs et utilisatrices Marketo Engage vers Adobe Admin Console. Il s’agit d’une migration nécessaire qui n’affectera aucun workflow marketing, contenu, ni aucune intégration ou ressource.

>[!TIP]
>
>Découvrez comment utiliser Adobe Admin Console pour gérer vos droits Adobe dans l’ensemble de votre organisation à l’aide du [Guide d’administration pour les entreprises et les équipes](https://helpx.adobe.com/fr/enterprise/admin-guide.html){target="_blank"}.

## Qu’est-ce qui change ? {#what-is-changing}

Dans le cadre de la migration, votre abonnement et la gestion des utilisateurs et utilisatrices seront transférés de l’application Marketo vers Adobe Admin Console.

* **Les administrateurs et administratrices système géreront les abonnements sur Adobe Admin Console**. Consultez tous vos produits Adobe dans une seule console.

* **Les administrateurs et administratrices de produit géreront les utilisateurs et utilisatrices ainsi que leur accès sur Adobe Admin Console**. Ajoutez et supprimez des utilisateurs et utilisatrices pour tous vos abonnements Adobe. Adobe Admin Console ne prend pas en charge l’expiration d’accès des utilisateurs et utilisatrices. Les utilisateurs et utilisatrices disposant d’un accès à Marketo Engage programmé pour expirer après la migration continueront à migrer et se verront accorder un accès sans expiration. Après la migration, ils doivent être supprimés manuellement au plus tard à la date d’expiration souhaitée.

* **Les utilisateurs et utilisatrices se connecteront avec Adobe Identity**. Adobe effectuera la migration des utilisateurs et utilisatrices existants vers Adobe Admin Console. Les utilisateurs et utilisatrices se connecteront à leurs abonnements Marketo à l’aide de leur nouvelle identité Adobe, soit un Adobe ID, soit un Adobe Federated ID (SSO).

* **Les URL auront un aspect différent après la migration**. Le service de Marketo Engage passera d’experience.adobe.com à Adobe Experience Cloud, et les URL seront au format suivant : `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (les XXX représentent l’ID Munchkin, et le @tenantID provient de votre organisation Adobe). Vous devrez travailler avec votre équipe informatique pour placer sur la liste autorisée tous les domaines Adobe répertoriés [au début de cet article](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} afin d’éviter toute interruption de l’accès à Marketo Engage.

Les numéros d’ID de vos ressources restent les mêmes. Les liens et signets précédents vers les ressources Marketo Engage sur le domaine engage-xx.marketo.com _continueront_ à fonctionner. Cependant, vous devez d’abord vous connecter à l’instance Marketo Engage pour l’URL à laquelle vous accédez. Par exemple, pour accéder à un signet pour une campagne intelligente dans l’instance avec l’identifiant Munchkin 123-ABC-456, vous devez d’abord vous connecter à l’instance Marketo Engage avec l’identifiant Munchkin 123-ABC-456.

Bien que cela ne soit pas prévu, les futurs travaux de développement peuvent perturber cette fonction de redirection. Pour éviter toute interruption inattendue, il est recommandé de mettre à jour les signets dès que possible.

## Qu’est-ce qui ne change pas ? {#what-is-not-changing}

* **La façon dont vous gérez toutes les autres fonctionnalités**, y compris la gestion des fonctionnalités, des rôles d’utilisateurs et d’utilisatrices, des espaces de travail et du comportement de l’application Marketo Engage elle-même, reste inchangée. La gestion des utilisateurs et utilisatrices locaux (API uniquement) reste dans l’onglet _Utilisateurs et utilisatrices et rôles_ de la zone d’administration de Marketo.

## Chronologie du parcours de migration {#migration-journey-timeline}

Adobe commencera par migrer votre ou vos abonnements Marketo Engage vers Adobe Admin Console, puis tous les utilisateurs et utilisatrices dont les adresses e-mail sont vérifiées. Si vous êtes administrateur ou administratrice système ou administrateur ou administratrice de produit Marketo, vous recevrez des e-mails vous guidant tout au long du parcours de migration. Voici une chronologie de ce à quoi vous pouvez vous attendre :

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### Migration complète de l’abonnement {#subscription-migration-complete}

Les administrateurs et administratrices système recevront un e-mail une fois la migration d’abonnement vers Adobe Admin Console terminée.

Les administrateurs et administratrices système peuvent devoir effectuer certaines étapes requises avant que la migration des utilisateurs et utilisatrices ne commence afin de minimiser l’impact sur les utilisateurs et utilisatrices de Marketo :

* Si vos utilisateurs et utilisatrices Marketo se connectent actuellement avec l’authentification unique, vous devrez configurer l’authentification unique sur Adobe Admin Console afin que vos utilisateurs et utilisatrices puissent continuer à se connecter avec l’authentification unique. Si vos utilisateurs et utilisatrices Marketo n’utilisent actuellement pas l’authentification unique, mais que vous souhaitez la configurer sur Adobe Admin Console, vous pouvez le faire à ce stade du parcours de migration.

* Si vous gérez déjà d’autres produits Adobe dans votre Adobe Admin Console, Adobe peut demander votre consentement pour migrer automatiquement les utilisateurs et utilisatrices vers votre console existante. Cliquez sur le bouton « Commencer » dans l’e-mail pour accéder à la page de consentement.

La gestion des utilisateurs et utilisatrices n’a pas changé pour le moment. Bien que les produits Marketo apparaissent dans Admin Console, les administrateurs et administratrices Marketo continueront à gérer les utilisateurs et utilisatrices dans la zone d’administration Marketo et ces derniers continueront à se connecter avec leur identité Marketo jusqu’à ce que leur migration d’utilisateur ou d’utilisatrice soit terminée. Pendant ce temps, les produits Marketo ne peuvent pas être administrés dans Admin Console tant que la migration des utilisateurs et utilisatrices n’a pas commencé. Cela inclut l’instance Dynamic Chat associée à l’abonnement.

>[!NOTE]
>
>Si vous n’utilisez actuellement pas l’authentification unique mais que vous envisagez de l’implémenter, nous vous suggérons de le faire avant que la migration des utilisateurs et utilisatrices ne se produise. Si vous souhaitez implémenter l’authentification unique et que votre abonnement a été intégré à Adobe Identity sans que l’authentification unique ne soit implémentée dans l’organisation Adobe, envoyez un ticket à l’[assistance de Marketo](https://nation.marketo.com/){target="_blank"} et indiquez la rubrique « Marketo sur Admin Console, implémentation de l’authentification unique ».

### Planifier la migration des utilisateurs et utilisatrices {#schedule-user-migration}

Une fois que l’administrateur ou l’administratrice système a rempli les conditions préalables décrites dans la section précédente, Adobe planifie automatiquement la migration de vos utilisateurs et utilisatrices 30 jours à l’avance et communique avec les administrateurs et administratrices de produit Marketo pour gérer la migration des utilisateurs et utilisatrices.

Les administrateurs et administratrices de produit Marketo :

* Reçoivent un e-mail avec leur date de début de migration des utilisateurs et utilisatrices planifiée 30 jours à l’avance.

* Obtiennent l’accès à la console de migration de Marketo, située dans la zone d’administration de Marketo, où il leur est possible de modifier la date de migration d’un abonnement.

>[!NOTE]
>
>En raison de la complexité de la migration, les changements de date sont limités à 30 jours au maximum au-delà de la date planifiée. Envoyez un e-mail à `marketocares@marketo.com` si vous avez besoin d’une date ultérieure.

* Voient une bannière dans Mon Marketo qui affiche un compte à rebours de la date de début de la migration des utilisateurs et utilisatrices.

* Reçoivent un e-mail de rappel la veille de la date de début de la migration des utilisateurs et utilisatrices.

### Préparer les utilisateurs et utilisatrices au jour de la migration {#prepare-users-for-migration-day}

En tant qu’administrateur ou administratrice de produit Marketo, nous vous recommandons de vous assurer que l’ensemble des personnes sont prêtes pour le jour de la migration.

* Vérifiez le statut de [vérification d’e-mail](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} de l’ensemble des utilisateurs et utilisatrices dans la zone d’administration de Marketo. Encouragez les utilisateurs et utilisatrices qui n’ont pas vérifié leur adresse e-mail à le faire et aidez-les à résoudre tous les problèmes liés au processus de vérification.

* Recherchez les notifications concernant les personnes « verrouillées » dans votre boîte de réception. Conseillez aux personnes verrouillées de réinitialiser leur mot de passe afin de rétablir l’accès à Marketo Engage avant le jour de la migration.

* Préparez l’ensemble des utilisateurs et utilisatrices à la migration à venir vers Adobe Identity.

>[!IMPORTANT]
>
>Si un utilisateur ou une utilisatrice Marketo Engage ne vérifie pas son adresse e-mail ou que la personne est verrouillée au moment de la migration des utilisateurs et utilisatrices, la personne n’est pas migrée vers un Adobe ID et perd l’accès à l’abonnement Marketo une fois la migration de l’abonnement terminée. Pour récupérer l’accès, un administrateur ou une administratrice de produit Marketo doit l’ajouter en tant que nouvel utilisateur ou nouvelle utilisatrice.

### À quoi s’attendre le jour de la migration {#what-to-expect-on-migration-day}

Tous les abonnements Marketo avec un fuseau horaire des États-Unis seront migrés à partir de minuit, heure standard du Pacifique, à la date de début de la migration. La migration des utilisateurs et utilisatrices pour tous les autres abonnements commencera à minuit dans le fuseau horaire spécifié par l’abonnement.

**Adobe migre automatiquement les administrateurs et administratrices Marketo (avec un rôle d’administration standard) en premier**. Lorsque les administrateurs et administratrices Marketo sont migrés vers Adobe Identity avec un rôle d’administration de produit Admin Console, ils se voient attribuer le rôle d’administration de produit Adobe dans l’application Marketo avec tous les autres rôles qu’ils occupaient auparavant.

**Si votre abonnement Marketo ne dispose pas de l’authentification unique dans Marketo et/ou votre organisation Adobe**, Adobe migre automatiquement le reste de vos utilisateurs et utilisatrices. Ce workflow vise à fournir le niveau d’automatisation le plus élevé possible afin de minimiser les frais généraux pour les utilisateurs et utilisatrices d’Adobe Marketo. Aucune action de votre part n’est requise pour exécuter la migration.

**Si votre abonnement Marketo dispose d’une authentification unique dans Marketo et/ou votre organisation Adobe**, les administrateurs et administratrices Marketo auront accès à la zone Migration des utilisateurs et utilisatrices en libre-service de la console de migration de Marketo, située dans la zone Administration de Marketo. Pour les personnes qui ont besoin d’un meilleur contrôle pendant le processus de migration des utilisateurs et utilisatrices, les administrateurs et administratrices Marketo pourront sélectionner les utilisateurs et utilisatrices à migrer par lots ou tout le monde en même temps. Une fois les personnes sélectionnées, les administrateurs et administratrices ont la possibilité de « Migrer maintenant » ou de « Planifier la migration » pour une date ultérieure, ce qui leur offre une flexibilité et un contrôle optimaux quant aux utilisateurs et utilisatrices qui feront l’objet d’une migration.

>[!NOTE]
>
>Il n’y aura aucune perte d’accès au produit pendant la migration des utilisateurs et utilisatrices. Si une personne est connectée pendant sa migration, elle est déconnectée et invitée à se reconnecter dans les minutes qui suivent à l’aide d’Adobe Identity une fois la migration terminée. L’utilisateur ou l’utilisatrice doit accepter l’invitation en cliquant sur le lien contenu dans l’e-mail de droits envoyé à la fin d’une migration réussie.

Lorsque les personnes seront migrées, elles recevront un e-mail d’Adobe les informant du changement de leur méthode de connexion à Marketo. Les utilisateurs et utilisatrices **doivent** accepter une invitation à se connecter pour la première fois à l’aide d’Adobe Identity, soit en se connectant avec un Adobe ID existant, soit en configurant un nouvel Adobe ID à l’aide de la même adresse e-mail.

Vous trouverez plus d’informations dans les sections [Migration vers Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [Connexion d’utilisateur ou d’utilisatrice à Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} et [Questions fréquentes sur Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Migration des utilisateurs et utilisatrices terminée {#user-migration-complete}

Adobe avertira l’ensemble des administrateurs et administratrices système et de produit par e-mail une fois la migration des administrateurs et administratrices et des utilisateurs et utilisatrices terminée. À ce stade, l’ensemble des utilisateurs et utilisatrices de Marketo pour cet abonnement se connecteront à Marketo à l’aide d’Adobe Identity, et les administrateurs et administratrices de produit géreront les utilisateurs et utilisatrices uniquement sur Adobe Admin Console.

## Obtenir de l’aide {#get-support}

Pour obtenir davantage d’aide concernant votre abonnement ou la migration des utilisateurs et utilisatrices, envoyez un e-mail à `marketocares@marketo.com`.

>[!MORELIKETHIS]
>
>* [Vue d’ensemble de la migration vers Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Connexion d’utilisateur ou d’utilisatrice à Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Questions fréquentes sur Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [Tutoriel sur la migration vers Adobe Identity Management](https://experienceleague.adobe.com/fr/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}
