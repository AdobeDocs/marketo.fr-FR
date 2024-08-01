---
description: Configuration d’un environnement de test d’actions Sales Insight - Documents Marketo - Documentation du produit
title: Configuration d’un environnement de test d’actions de statistiques sur les ventes
exl-id: 8bc3a8a6-7fbc-4cbe-99a7-21b066ec4f96
source-git-commit: 1f228323c18204149630a7cb77d6ae0a88b425e3
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Configuration d’un environnement de test d’actions de statistiques sur les ventes {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions est une application web qui s’intègre exclusivement au CRM Salesforce via le [ package Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. On parle parfois de &quot;ventes Marketo&quot; ou simplement de &quot;actions&quot;.

Si vous disposez d’un environnement de test Marketo, vous pouvez activer une instance d’actions à utiliser avec votre environnement de test à des fins de test.

Lors de la configuration d’une instance Actions, vous devez décider si elle sera configurée pour fonctionner avec Salesforce Sandbox ou avec la production Salesforce. Cela est dû au fait que Salesforce utilise différents points de terminaison pour chacun d’eux et que les actions utilisent la connexion à Salesforce pour activer et authentifier les utilisateurs.

Suivez les étapes ci-dessous pour configurer une instance Actions afin qu’elle fonctionne avec votre instance Salesforce Sandbox.

>[!NOTE]
>
>Vous pouvez en savoir plus sur la façon dont les utilisateurs [activeront leur siège Actions](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}. Vous pouvez également en savoir plus sur la façon dont les utilisateurs [s’authentifient avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}. De plus, si vous préférez que les utilisateurs s’authentifient par courrier électronique et mot de passe, vous pouvez en savoir plus à ce sujet dans notre [article sur les paramètres de gestion de connexion](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

## Demande d’une instance d’actions à configurer dans votre environnement de test Marketo {#request=an-actions-instance}

Les actions Sales Insight ne sont pas activées pour les instances Marketo Sandbox, sauf si elles sont demandées. Contactez l’équipe du compte d’Adobe (votre gestionnaire de compte) pour envoyer une demande.

## Configuration de votre compte d’actions pour Marketo Sandbox {#provision-your-actions-account}

Une fois que les actions sont activées pour votre environnement de test Marketo, vous devez suivre les étapes ci-dessous pour activer votre nouvelle instance.

1. Connectez-vous à votre instance Marketo Sandbox.

1. Accédez à **Admin**.

1. Sélectionnez **Sales Insight**.

1. Sélectionnez **Configuration des actions**.

   >[!IMPORTANT]
   >
   >Une adresse électronique ne peut être utilisée que pour une instance Actions sur les instances Sandbox et Production. Si vous êtes un administrateur qui doit accéder à plusieurs instances dans Production et Sandbox, vous devez utiliser une adresse électronique différente pour chacune d’elles.

1. Dans la carte d’attribution des privilèges d’accès, sélectionnez l’utilisateur que vous souhaitez inviter à rejoindre votre instance d’actions Sales Insight.

## Activation de l’instance d’actions {#activate-your-actions-instance}

Votre instance Actions doit être activée avec un compte de production Salesforce. Une fois activé, il peut être basculé vers un compte Sandbox Salesforce.

1. Recherchez l’invitation envoyée.

1. Cliquez sur le lien **Commencer** .

1. Activez avec votre instance de production Salesforce.

1. Suivez les invites pour configurer le compte. Pour une présentation détaillée, consultez notre [article Intégration d’utilisateurs](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}.

## Préparation de l’instance d’actions à la compatibilité avec votre instance Salesforce Sandbox {#prepare-your-actions-instance}

Les actions nécessitent que vous activiez d’abord une nouvelle instance avec un utilisateur de production Salesforce. Une fois activée, vous pouvez suivre les étapes suivantes pour préparer votre instance à la compatibilité Salesforce Sandbox.

1. Mettez à jour les paramètres de connexion sur &quot;Toutes les méthodes de connexion&quot; afin que vous puissiez vous connecter avec un nom d’utilisateur et un mot de passe, si nécessaire. Si vous le souhaitez, vous pouvez revenir à &quot;Salesforce uniquement&quot; une fois que tout est configuré. [Découvrez comment procéder ici](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

1. Déconnectez-vous de Salesforce Production et connectez-vous à votre environnement de test Salesforce. [Découvrez comment vous connecter ici](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}. Pour l’étape 3, sélectionnez &quot;Sandbox&quot; au lieu de &quot;Salesforce&quot;. Si vous êtes déjà connecté, une option de déconnexion doit s’afficher dans l’onglet Connexions et personnalisations Salesforce .

>[!NOTE]
>
>Si vous disposez d’un domaine personnalisé pour votre instance Salesforce, nous vous recommandons d’être connecté à votre instance Salesforce avant de vous connecter à Salesforce ou de vous connecter aux actions.

## Demander que votre instance d’actions soit convertie pour être compatible avec votre environnement de test Salesforce {#request-your-actions-instance-be-converted}

1. Contactez le [support Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} pour demander que votre nouvelle instance d’actions Sales Insight soit configurée pour être compatible avec Salesforce Sandbox.

1. Testez tout ce qui est configuré correctement en essayant de vous connecter à l’aide du bouton &quot;Se connecter avec Salesforce&quot; sur la page toutapp.com/login.

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >Si vous rencontrez des problèmes à ce stade, vous pouvez demander la réinitialisation d’un mot de passe et utiliser un mot de passe pour récupérer l’accès à votre compte.

Votre instance est maintenant prête à être utilisée avec votre instance Salesforce Sandbox. Si vous souhaitez utiliser la [connexion automatique Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"} à partir de Salesforce, vous pouvez revenir à &quot;Salesforce uniquement&quot; dans vos [paramètres de gestion de connexion](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

>[!NOTE]
>
>* [Connecter votre compte d’actions d’aperçu des ventes à Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [ Guide d’intégration des utilisateurs des actions Sales Insight ](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [Connexion automatique à partir de Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [Paramètres de gestion de connexion](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
