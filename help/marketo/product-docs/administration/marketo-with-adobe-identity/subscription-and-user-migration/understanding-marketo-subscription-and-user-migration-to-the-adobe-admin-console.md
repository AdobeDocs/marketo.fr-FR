---
description: Présentation de l’abonnement à Marketo et de la migration des utilisateurs vers Adobe Admin Console - Documentation de Marketo - Documentation du produit
title: Présentation de l’abonnement à Marketo et de la migration des utilisateurs vers Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 8b44c3b2ccabeb796a3a8f7775848a5063279076
workflow-type: tm+mt
source-wordcount: '1571'
ht-degree: 0%

---

# Présentation de l’abonnement à Marketo et de la migration des utilisateurs vers Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe améliore la gestion de vos abonnements et de vos utilisateurs Adobe Marketo Engage, ce qui accroît votre productivité et celle de votre entreprise. Dans le cadre de cette modification, Adobe effectue une migration de vos abonnements et de vos utilisateurs Marketo Engage vers Adobe Admin Console. Il s’agit d’une migration nécessaire qui n’affectera aucun workflow marketing, contenu, intégrations ou ressources.

>[!TIP]
>
>Découvrez comment utiliser Adobe Admin Console pour gérer vos droits Adobe dans l’ensemble de votre organisation à l’aide du [ Guide d’administration pour les entreprises et les équipes ](https://helpx.adobe.com/fr/enterprise/admin-guide.html){target="_blank"}.

## Qu’est-ce qui change ? {#what-is-changing}

Dans le cadre de la migration, votre abonnement et la gestion des utilisateurs seront transférés de l’application Marketo vers Adobe Admin Console.

* **Les administrateurs système géreront les abonnements sur Adobe Admin Console**. Voir tous vos produits Adobe dans une seule console.

* **Les administrateurs de produit géreront les utilisateurs et leur accès sur Adobe Admin Console**. Ajoutez et supprimez des utilisateurs pour tous vos abonnements Adobe. Le Adobe Admin Console ne prend pas en charge l’expiration d’accès utilisateur. Les utilisateurs et utilisatrices disposant d’un accès à Marketo Engage programmé pour expirer après la migration continueront à migrer et se verront accorder un accès sans expiration. Après la migration, ils doivent être supprimés manuellement au plus tard à la date d’expiration souhaitée.

* **Les utilisateurs se connecteront avec Adobe Identity**. Adobe effectuera la migration des utilisateurs existants vers Adobe Admin Console. Les utilisateurs se connecteront à leurs abonnements Marketo à l’aide de leur nouvelle identité Adobe, soit une Adobe ID, soit une Federated ID Adobe (SSO).

* **Les URL auront un aspect différent après la migration**. Marketo Engage sera diffusée de experience.adobe.com à Adobe Experience Cloud, et les URL seront au format suivant : `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (les XXX représentent l’ID Munchkin, et l’@tenantID provient de votre organisation Adobe). Vous devrez travailler avec votre équipe informatique pour placer sur la liste autorisée tous les domaines Adobe répertoriés [au début de cet article](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} afin d’éviter toute interruption de l’accès à Marketo Engage.

Les numéros d’ID de vos ressources restent les mêmes. Les liens et signets précédents vers les ressources Marketo Engage sur le domaine engage-xx.marketo.com _continueront_ à fonctionner. Cependant, vous devez d’abord vous connecter à l’instance Marketo Engage pour l’URL à laquelle vous accédez. Par exemple, pour accéder à un signet pour une campagne dynamique dans l’instance avec l’identifiant Munchkin 123-ABC-456, vous devez d’abord vous connecter à l’instance Marketo Engage avec l’identifiant Munchkin 123-ABC-456.

Bien que cela ne soit pas prévu, les travaux de développement futurs peuvent rompre cette fonction de redirection. Pour éviter toute interruption inattendue, il est recommandé de mettre à jour les signets dès que possible.

## Qu’est-ce qui ne change pas ? {#what-is-not-changing}

* **La façon dont vous gérez toutes les autres fonctionnalités** y compris la gestion des fonctionnalités, des rôles utilisateur, des espaces de travail, des fonctionnalités et du comportement de l’application Marketo Engage elle-même, reste inchangée. La gestion des utilisateurs locaux (API uniquement) reste dans l’onglet _Utilisateurs et rôles_ de la zone d’administration de Marketo.

## Calendrier du Parcours de migration {#migration-journey-timeline}

Adobe commencera par migrer votre ou vos abonnements Marketo Engage vers Adobe Admin Console, puis tous les utilisateurs dont les adresses e-mail sont vérifiées. Si vous êtes un administrateur système ou un administrateur de produit Marketo, vous recevrez des e-mails vous guidant tout au long du parcours de migration. Voici un calendrier de ce à quoi vous pouvez vous attendre :

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### Migration de l’abonnement terminée {#subscription-migration-complete}

Les administrateurs système recevront un e-mail une fois la migration d’abonnement vers Adobe Admin Console terminée.

Les administrateurs système peuvent devoir effectuer certaines étapes requises avant que la migration des utilisateurs ne commence afin de minimiser l’impact sur les utilisateurs de Marketo :

* Si vos utilisateurs Marketo se connectent actuellement avec l’authentification unique, vous devrez configurer l’authentification unique sur le Adobe Admin Console afin que vos utilisateurs puissent continuer à se connecter avec l’authentification unique. Si vos utilisateurs Marketo n’utilisent pas actuellement la connexion unique, mais que vous souhaitez la configurer sur Adobe Admin Console, vous pouvez le faire à ce stade du parcours de migration.

* Si vous gérez déjà d’autres produits Adobe dans votre Adobe Admin Console, Adobe peut demander votre consentement pour migrer automatiquement les utilisateurs vers votre console existante. Cliquez sur le bouton « Commencer » dans l’e-mail pour accéder à la page de consentement.

La gestion des utilisateurs n’a pas changé pour le moment. Bien que les produits Marketo apparaissent dans Admin Console, les administrateurs Marketo continueront à gérer les utilisateurs dans la zone d’administration Marketo et les utilisateurs continueront à se connecter avec leur identité Marketo jusqu’à ce que leur migration d’utilisateur soit terminée. Pendant ce temps, les produits Marketo ne peuvent pas être administrés dans Admin Console tant que la migration des utilisateurs n’a pas commencé. Cela inclut l’instance Dynamic Chat associée à l’abonnement.

>[!NOTE]
>
>Si vous n’utilisez pas actuellement la connexion unique, mais envisagez de l’implémenter, nous vous suggérons de le faire avant que la migration des utilisateurs ne se produise. Si vous souhaitez implémenter l’authentification unique et que votre abonnement a été intégré à Adobe Identity sans que la connexion unique ne soit implémentée dans l’organisation Adobe, envoyez un ticket à l’assistance de [Marketo](https://nation.marketo.com/){target="_blank"} et indiquez la rubrique « Marketo sur Admin Console, implémentation de l’authentification unique ».

### Planifier la migration des utilisateurs {#schedule-user-migration}

Une fois que l’administrateur système a rempli les conditions préalables décrites dans la section précédente, Adobe planifie automatiquement la migration de vos utilisateurs 30 jours à l’avance et communique avec les administrateurs de produit Marketo pour gérer la migration des utilisateurs.

Les administrateurs de produit Marketo :

* Recevez un e-mail avec leur Date de début de migration des utilisateurs planifiée 30 jours à l’avance.

* Accédez à la console Migration de Marketo, située dans la zone d’administration de Marketo, où ils ont la possibilité de modifier la date de migration d’un abonnement.

>[!NOTE]
>
>En raison de la complexité de la migration, les changements de date sont limités à 30 jours au maximum au-delà de la date planifiée. Envoyez un e-mail à `marketocares@marketo.com` si vous avez besoin d’une date ultérieure.

* Une bannière dans Mon Marketo affiche un compte à rebours vers la date de début de la migration des utilisateurs.

* Recevez un e-mail de rappel la veille de la date de début de la migration des utilisateurs.

### Préparer les utilisateurs à la journée de migration {#prepare-users-for-migration-day}

En tant qu’administrateur de produit Marketo, nous vous recommandons de vous assurer que tous les utilisateurs sont prêts pour la journée de migration.

* Vérifiez [vérification par e-mail](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} le statut pour tous les utilisateurs dans la zone d’administration de Marketo. Encouragez les utilisateurs et utilisatrices qui n’ont pas vérifié leur adresse e-mail à le faire et aidez-les à résoudre tous les problèmes liés au processus de vérification.

* Recherchez des notifications d’utilisateur « verrouillées » dans votre boîte de réception. Conseillez aux utilisateurs verrouillés de réinitialiser leur mot de passe afin de rétablir l’accès à Marketo Engage avant la journée de migration.

* Préparez tous les utilisateurs à la migration à venir vers Adobe Identity.

>[!IMPORTANT]
>
>Si un utilisateur Marketo Engage ne vérifie pas son adresse e-mail ou est verrouillé au moment de la migration de l’utilisateur, il n’est pas migré vers une Adobe ID et perd l’accès à l’abonnement Marketo une fois la migration de l’abonnement terminée. Pour récupérer l’accès, un administrateur de produit Marketo doit les ajouter en tant que nouvel utilisateur.

### À quoi s’attendre le jour de la migration {#what-to-expect-on-migration-day}

Tous les abonnements Marketo avec fuseau horaire des États-Unis seront migrés à partir de minuit, heure standard du Pacifique, de la date de début de la migration. La migration des utilisateurs pour tous les autres abonnements commencera à minuit dans le fuseau horaire spécifié par l&#39;abonnement.

**Adobe migre automatiquement les administrateurs Marketo (avec un rôle d’administrateur standard) en premier**. Lorsque les administrateurs Marketo sont migrés vers Adobe Identity avec un rôle d’administrateur de produit Admin Console, ils se voient attribuer le rôle d’administrateur de produit Adobe dans l’application Marketo avec tous les autres rôles qu’ils occupaient auparavant.

**Si votre abonnement Marketo ne dispose pas de l’authentification unique dans Marketo et/ou votre organisation Adobe**, Adobe migre automatiquement le reste de vos utilisateurs. Ce workflow vise à fournir le niveau d’automatisation le plus élevé possible afin de minimiser les frais généraux pour les utilisateurs d’Adobe Marketo. Aucune action de votre part n’est requise pour exécuter la migration.

**Si votre abonnement Marketo dispose d’une authentification unique dans Marketo et/ou votre organisation Adobe**, les administrateurs Marketo auront accès à la zone Migration des utilisateurs en libre-service de la console de migration de Marketo, située dans la zone Administration de Marketo. Pour ceux qui ont besoin d’un meilleur contrôle pendant le processus de migration des utilisateurs, les administrateurs Marketo pourront commencer à sélectionner les utilisateurs à migrer par lots ou tous en même temps. Une fois les utilisateurs sélectionnés, les administrateurs ont la possibilité de « Migrer maintenant » ou de « Planifier la migration » pour une date ultérieure, ce qui leur offre une flexibilité et un contrôle optimaux quant aux utilisateurs qui feront l’objet d’une migration.

>[!NOTE]
>
>Il n’y aura aucune perte d’accès au produit pendant la migration des utilisateurs. Si un utilisateur est connecté au cours de la migration, il se déconnecte et est invité à se reconnecter dans les minutes qui suivent à l’aide d’Adobe Identity une fois la migration terminée. L’utilisateur doit accepter l’invitation en cliquant sur le lien contenu dans l’e-mail de droits envoyé à la fin d’une migration d’utilisateur réussie.

Lorsque les utilisateurs seront migrés, ils recevront un e-mail d’Adobe les informant du changement de leur méthode de connexion à Marketo. Les utilisateurs **doivent** acceptent une invitation à se connecter pour la première fois à l’aide d’Adobe Identity, soit en se connectant avec un Adobe ID existant, soit en configurant un nouvel Adobe ID à l’aide de la même adresse e-mail.

Vous trouverez plus d’informations dans les sections [Migration vers Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [Connexion utilisateur avec Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} et [FAQ sur Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Migration des utilisateurs terminée {#user-migration-complete}

Adobe avertira tous les administrateurs système et les administrateurs de produit par e-mail une fois que tous les administrateurs et utilisateurs auront été migrés. À ce stade, tous les utilisateurs de Marketo pour cet abonnement se connecteront à Marketo à l’aide d’Adobe Identity, et les administrateurs de produit géreront les utilisateurs uniquement sur Adobe Admin Console.

## Obtenir de l’aide {#get-support}

Pour obtenir une assistance supplémentaire concernant votre abonnement ou la migration des utilisateurs, envoyez un e-mail à `marketocares@marketo.com`.

>[!MORELIKETHIS]
>
>* [Migration vers Adobe Identity Overview](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Connexion utilisateur avec Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [FAQ Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [Tutoriel sur la migration vers Adobe Identity Management](https://experienceleague.adobe.com/fr/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}
