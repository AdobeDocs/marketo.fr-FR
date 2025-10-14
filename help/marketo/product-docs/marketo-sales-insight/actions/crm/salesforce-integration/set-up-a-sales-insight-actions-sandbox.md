---
description: Configuration d’un sandbox d’actions Sales Insight - Documents Marketo - Documentation du produit
title: Configurer un sandbox d’Actions des informations sur les ventes
exl-id: 8bc3a8a6-7fbc-4cbe-99a7-21b066ec4f96
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 2%

---

# Configurer un sandbox d’Actions des informations sur les ventes {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions est une application web qui s’intègre exclusivement au CRM Salesforce via le package [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. Il est parfois appelé « Ventes Marketo » ou simplement « Actions ».

Si vous disposez d’un sandbox Marketo, vous pouvez permettre l’utilisation d’une instance Actions avec votre sandbox à des fins de test.

Lors de la configuration d’une instance Actions, vous devez décider si elle sera configurée pour fonctionner avec le sandbox Salesforce ou la production Salesforce. En effet, Salesforce utilise différents points d’entrée pour chacun et Actions utilise la connexion à Salesforce pour activer et authentifier les utilisateurs.

Suivez les étapes ci-dessous pour configurer une instance Actions afin qu’elle fonctionne avec votre instance Salesforce Sandbox.

>[!NOTE]
>
>Vous pouvez en savoir plus sur la manière dont les utilisateurs [activent leur siège Actions](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}. Vous pouvez également en savoir plus sur la manière dont les utilisateurs s’authentifieront [avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}. De plus, si vous préférez que les utilisateurs s’authentifient par e-mail et par mot de passe, vous pouvez en savoir plus à ce sujet dans notre article [Paramètres de gestion des connexions](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

## Demandez qu’une instance Actions soit configurée sur votre sandbox Marketo {#request=an-actions-instance}

Les actions Sales Insight ne sont pas activées pour les instances Marketo Sandbox, sauf demande contraire. Contactez l’équipe du compte Adobe (votre gestionnaire de compte) pour soumettre une demande.

## Configuration de votre compte d’actions pour Marketo Sandbox {#provision-your-actions-account}

Une fois que les actions sont activées pour votre sandbox Marketo, vous devez suivre les étapes ci-dessous pour activer votre nouvelle instance.

1. Connectez-vous à votre instance Marketo Sandbox.

1. Accédez à **Admin**.

1. Sélectionnez **Ventes Insight**.

1. Sélectionnez **Configuration des actions**.

   >[!IMPORTANT]
   >
   >Une adresse e-mail ne peut être utilisée que pour une seule instance Actions à la fois sur les instances Sandbox et de Production. Si vous êtes un administrateur qui devra accéder à plusieurs instances dans Production et Sandbox, vous devez utiliser une adresse e-mail différente pour chacune d’elles.

1. Dans la carte de mise en service, sélectionnez l’utilisateur que vous souhaitez inviter à rejoindre votre instance Sales Insight Actions.

## Activation De Votre Instance Actions {#activate-your-actions-instance}

Votre instance Actions devra être activée avec un compte de production Salesforce. Une fois activé, il peut être basculé vers un compte Sandbox Salesforce.

1. Localisez l’invitation envoyée.

1. Cliquez sur le lien **Commencer**.

1. Activez-le avec votre instance de production Salesforce.

1. Suivez les invites pour configurer le compte. Pour une présentation détaillée, consultez notre article [&#x200B; Intégration des utilisateurs &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}.

## Préparez votre instance Actions pour qu’elle soit compatible avec votre instance Salesforce Sandbox {#prepare-your-actions-instance}

Les actions nécessitent que vous activiez d’abord une nouvelle instance avec un utilisateur de production Salesforce. Une fois cette option activée, vous pouvez suivre les étapes ci-après pour préparer votre instance à la compatibilité avec Salesforce Sandbox.

1. Mettez à jour les paramètres de connexion sur « Toutes les méthodes de connexion » afin que vous puissiez vous connecter avec un nom d’utilisateur et un mot de passe si nécessaire. Si vous le souhaitez, vous pouvez revenir à « Salesforce uniquement » une fois que tout est configuré. [Voir comment faire ici](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

1. Déconnectez-vous de la production Salesforce et connectez-vous à votre sandbox Salesforce. [Voir comment se connecter ici](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}. Pour l’étape 3, sélectionnez « Sandbox » au lieu de « Salesforce ». Si vous êtes déjà connecté, vous devriez voir une option de déconnexion dans l’onglet Connexions et personnalisations de Salesforce .

>[!NOTE]
>
>Si vous disposez d’un domaine personnalisé pour votre instance Salesforce, nous vous recommandons de vous connecter à votre instance Salesforce avant de vous connecter à Salesforce ou à Actions.

## Demandez la conversion de votre instance Actions pour qu’elle soit compatible avec votre sandbox Salesforce {#request-your-actions-instance-be-converted}

1. Contactez l’assistance Marketo Engage [&#128279;](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} pour demander que votre nouvelle instance d’actions Sales Insight soit configurée de manière à être compatible avec Salesforce Sandbox.

1. Testez tout est configuré correctement en essayant de vous connecter à l’aide du bouton « Se connecter avec Salesforce » sur la page toutapp.com/login.

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >Si vous rencontrez des problèmes à ce stade, vous pouvez demander une réinitialisation du mot de passe et utiliser un mot de passe pour récupérer l’accès à votre compte.

Votre instance est maintenant prête à être utilisée avec votre instance Salesforce Sandbox. Si vous souhaitez utiliser la connexion automatique [Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"} depuis Salesforce, vous pouvez revenir à « Salesforce uniquement » dans vos [paramètres de gestion des connexions](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

>[!NOTE]
>
>* [Connexion de votre compte d’actions Sales Insight à Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [Guide d’intégration des utilisateurs des actions de vente Insight](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [&#x200B; Connexion automatique à partir de Salesforce &#x200B;](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [Paramètres de gestion des connexions](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
