---
description: Présentation de l’abonnement Marketo et de la migration des utilisateurs vers Adobe Admin Console - Documents Marketo - Documentation du produit
title: Présentation de l’abonnement Marketo et de la migration des utilisateurs vers Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 404d2720dec6b4932c99a1f390a88dc0835c7491
workflow-type: tm+mt
source-wordcount: '1301'
ht-degree: 0%

---

# Présentation de l’abonnement Marketo et de la migration des utilisateurs vers Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe améliore la gestion de vos abonnements et de vos utilisateurs Adobe Marketo Engage, en augmentant votre productivité pour vous et votre entreprise. Dans le cadre de cette modification, Adobe migre vos abonnements et utilisateurs de Marketo Engage vers Adobe Admin Console. Il s’agit d’une migration nécessaire qui n’affectera aucun workflow, contenu, intégration ou actif marketing.

Découvrez comment utiliser Adobe Admin Console pour gérer vos droits d’Adobe dans l’ensemble de votre organisation avec l’ [Guide d’administration pour les entreprises et les équipes](https://helpx.adobe.com/fr/enterprise/admin-guide.html){target="_blank"}.

## Qu’est-ce qui change ? {#what-is-changing}

Dans le cadre de la migration, votre gestion des abonnements et des utilisateurs passera de l’application Marketo à Adobe Admin Console.

* **Les administrateurs système gèrent les abonnements sur Adobe Admin Console.**. Consultez tous vos produits Adobe dans une seule console.

* **Les administrateurs de produit gèrent les utilisateurs et leur accès sur Adobe Admin Console**. Ajoutez et supprimez des utilisateurs pour tous vos abonnements Adobe.

* **Les utilisateurs se connecteront avec l’identité de l’Adobe**. Adobe migre les utilisateurs existants vers Adobe Admin Console. Les utilisateurs se connectent à leurs abonnements Marketo à l’aide de leur nouvelle identité d’Adobe : Adobe ID ou Adobe Federated ID (SSO).

* **La façon dont vous gérez toutes les autres fonctionnalités n’a pas changé** dans l’application Marketo Engage elle-même, notamment la gestion des fonctionnalités, des rôles utilisateur, des espaces de travail, des fonctionnalités et du comportement.

## Chronologie du Parcours de migration {#migration-journey-timeline}

Adobe migre d’abord vos abonnements de Marketo Engage vers Adobe Admin Console, puis migre tous les utilisateurs existants avec des adresses électroniques vérifiées. Si vous êtes administrateur système ou administrateur de produit Marketo, vous recevrez des e-mails vous guidant tout au long du parcours de migration. Voici une chronologie de ce à quoi vous pouvez vous attendre :

### Migration des abonnements terminée {#subscription-migration-complete}

Les administrateurs système recevront un e-mail une fois la migration de l’abonnement vers Adobe Admin Console terminée.

Les administrateurs système peuvent avoir besoin de suivre certaines étapes nécessaires avant que la migration des utilisateurs ne commence à minimiser l’impact pour les utilisateurs de Marketo :

* Si vos utilisateurs Marketo se connectent actuellement avec SSO, vous devrez configurer SSO sur Adobe Admin Console afin que vos utilisateurs puissent continuer à se connecter avec SSO. Si vos utilisateurs Marketo n’utilisent pas actuellement la fonction SSO, mais que vous souhaitez la configurer sur Adobe Admin Console, vous pouvez le faire à ce stade du parcours de migration.

* Si vous gérez déjà d’autres produits Adobe dans votre Adobe Admin Console, Adobe peut demander votre consentement pour migrer automatiquement les utilisateurs vers votre console existante. Cliquez sur le bouton &quot;Commencer&quot; dans le courrier électronique pour accéder à la page de consentement.

Pour l’instant, la gestion des utilisateurs n’a pas été modifiée. Bien que les produits Marketo apparaissent dans le Admin Console, les administrateurs Marketo continueront à gérer les utilisateurs dans la zone d’administration de Marketo, et les utilisateurs continueront à se connecter à l’aide de leur identité Marketo jusqu’à ce que leur migration des utilisateurs soit terminée. Pendant ce temps, les produits Marketo ne peuvent pas être administrés dans Admin Console tant que la migration des utilisateurs n’a pas commencé. Cela inclut l’instance de Dynamic Chat associée à l’abonnement.

>[!NOTE]
>
>Si vous n’utilisez pas actuellement SSO mais envisagez de l’implémenter, nous vous conseillons de le faire avant la migration des utilisateurs. Si vous souhaitez mettre en oeuvre l’authentification unique et que votre abonnement a été intégré à Adobe Identity sans que l’authentification unique soit mise en oeuvre dans l’organisation Adobe, envoyez un ticket à [Prise en charge de Marketo](https://nation.marketo.com/){target="_blank"} et spécifiez la rubrique &quot;Marketo on Admin Console, implémentation de l’authentification unique&quot;.

### Planification de la migration des utilisateurs {#schedule-user-migration}

Une fois que votre administrateur système a rempli les conditions préalables décrites dans la section précédente, Adobe programmera automatiquement la migration de vos utilisateurs 30 jours à l’avance et communiquera avec les administrateurs produit Marketo pour gérer la migration des utilisateurs.

Les administrateurs de produit Marketo :

* Recevez un courrier électronique avec la date de début de la migration des utilisateurs prévue 30 jours à l’avance.

* Accédez à la console de migration Marketo, située dans la zone d’administration de Marketo, où ils ont la possibilité de modifier la date de migration d’un abonnement.

>[!NOTE]
>
>En raison de la complexité de la migration, les modifications de date ne sont limitées qu’à 30 jours au maximum au-delà de la date planifiée. Envoi d’un courrier électronique à `marketocares@marketo.com` si vous avez besoin d’une date ultérieure.

* Dans My Marketo, une bannière s’affiche avec un compte à rebours jusqu’à la date de début de la migration des utilisateurs.

* Recevez un email de rappel le jour précédant la date de début de la migration de l’utilisateur.

### Préparation des utilisateurs pour le jour de migration {#prepare-users-for-migration-day}

En tant qu’administrateur de produit Marketo, vous êtes invité à vous assurer que tous les utilisateurs sont prêts pour le jour de migration.

* Vérifier [vérification par email](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} pour tous les utilisateurs de la zone d’administration de Marketo. Encourager les utilisateurs qui n’ont pas vérifié leur adresse électronique à le faire, et aider les utilisateurs à résoudre les problèmes liés à l’achèvement du processus de vérification.

* Préparez tous les utilisateurs à la migration à venir vers Adobe Identity.

>[!NOTE]
>
>À mesure que les utilisateurs migrent, ils reçoivent un courrier électronique de l’Adobe les informant de la modification de leur manière de se connecter à Marketo. Les utilisateurs seront invités à accepter une invitation à se connecter à l’aide d’Adobe Identity pour la première fois, soit en se connectant à l’aide d’une Adobe ID existante, soit en en configurant une nouvelle à l’aide de la même adresse électronique.

>[!IMPORTANT]
>
>Si un utilisateur Marketo Engage ne vérifie pas son adresse électronique, il ne sera pas migré vers un Adobe ID et n’aura plus accès à l’abonnement Marketo une fois la migration pour l’abonnement terminée. Pour récupérer l’accès, un administrateur de produit Marketo doit les ajouter en tant que nouvel utilisateur.

### À quoi vous attendre le jour de la migration {#what-to-expect-on-migration-day}

Tous les abonnements Marketo avec un fuseau horaire des États-Unis seront migrés à partir de minuit, heure du Pacifique, à partir de la date de début de la migration. La migration des utilisateurs pour tous les autres abonnements commencera à minuit du fuseau horaire spécifié de l’abonnement.

**Adobe migrera automatiquement d’abord les administrateurs Marketo**. Lorsque les administrateurs Marketo sont migrés vers Adobe Identity, ils se voient attribuer le rôle d’ administrateur de produit Adobe dans l’application Marketo avec tous les autres rôles qu’ils avaient auparavant.

**Si votre abonnement Marketo comporte moins de 75 utilisateurs**, Adobe migre automatiquement le reste de vos utilisateurs. Ce workflow vise à offrir le niveau d’automatisation le plus élevé afin de réduire la surcharge pour les utilisateurs d’Adobe Marketo. Aucune action de votre part n’est requise pour exécuter la migration.

**Si votre abonnement Marketo comporte plus de 75 utilisateurs**, les administrateurs de produit Marketo auront accès à la zone Migration des utilisateurs en libre-service de Marketo Migration Console, située dans la zone d’administration de Marketo. Pour ceux qui ont besoin d’un meilleur contrôle pendant le processus de migration des utilisateurs, les administrateurs de produits Marketo pourront commencer à sélectionner des utilisateurs pour effectuer la migration par lots, ou tous à la fois. Une fois les utilisateurs sélectionnés, les administrateurs ont la possibilité de &quot;migrer maintenant&quot; ou de &quot;planifier la migration&quot; à une date ultérieure, ce qui leur offre la flexibilité et le contrôle suffisants sur les utilisateurs migrés lors de cette migration.

>[!NOTE]
>
>L’accès au produit ne sera pas perdu lors de la migration des utilisateurs. Si un utilisateur est connecté au moment de la migration de son utilisateur, il sera déconnecté et invité à se reconnecter dans les minutes qui suivent la fin de la migration à l’aide de l’option Adobe Identity.

Lorsque les utilisateurs sont migrés, ils reçoivent un courrier électronique de l’Adobe les informant de la modification de leur manière de se connecter à Marketo. Les utilisateurs seront invités à accepter une invitation à se connecter à l’aide d’Adobe Identity pour la première fois, soit en se connectant à un Adobe ID existant, soit en configurant une nouvelle Adobe ID à l’aide de la même adresse électronique.

Vous trouverez plus d’informations dans la section [Migration vers Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [User Sign-in with Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}, and [Adobe Identity Management FAQ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Migration des utilisateurs terminée {#user-migration-complete}

Adobe avertira tous les administrateurs système et les administrateurs de produit par courrier électronique une fois que tous les administrateurs et utilisateurs seront migrés. À l’heure actuelle, tous les utilisateurs de Marketo pour cet abonnement se connectent à Marketo à l’aide d’Adobe Identity et les administrateurs de produit gèrent les utilisateurs uniquement sur Adobe Admin Console.

## Obtenir une assistance {#get-support}

Pour une prise en charge supplémentaire concernant votre inscription ou la migration des utilisateurs, envoyez un email à `marketocares@marketo.com`.

>[!MORELIKETHIS]
>
>* [Migration vers Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Connexion de l’utilisateur avec Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [FAQ sur Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
