---
description: Connexion à l’aide d’OAuth 2.0 - Documents Marketo - Documentation du produit
title: Connexion à l’aide d’OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Connexion à l’aide d’OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce utilise le protocole OAuth pour permettre aux utilisateurs des applications d’accéder en toute sécurité (authentifier l’application à l’aide d’OAuth 2.0) aux données sans avoir à révéler les informations de connexion. Vous trouverez ci-dessous les étapes à suivre pour établir une connexion sécurisée et synchroniser le Marketo Engage avec Salesforce.

>[!IMPORTANT]
>
>Pour connecter Marketo et Salesforce à l’aide d’OAuth, connectez-vous à Marketo par le biais d’un navigateur privé (incognito) afin d’éviter toute connexion à Salesforce avec un nom d’utilisateur incorrect.

## Configuration d’une application connectée {#set-up-connected-app}

1. Dans Salesforce, sous Configuration, dans les outils de plateforme, accédez à Applications, App Manager, puis cliquez sur **[!UICONTROL Nouvelle application connectée]**.

   ![](assets/setting-up-oauth-2-1.png)

1. Renseignez les détails et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/setting-up-oauth-2-2.png)

1. Cochez la case **[!UICONTROL Activer les paramètres OAuth]** . Pour l’URL de callback, saisissez `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Sélectionnez tous les périmètres OAuth disponibles et cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/setting-up-oauth-2-3.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/setting-up-oauth-2-4.png)

1. Cliquez sur **[!UICONTROL Continuer]**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copiez la clé du client et le secret du client (vous en aurez besoin ultérieurement pour l’utiliser dans Marketo Engage).

   ![](assets/setting-up-oauth-2-6.png)

>[!CAUTION]
>
>Pendant que vous êtes toujours sur la page Nouvelle application connectée, faites défiler l’écran vers le bas et assurez-vous que la case &quot;Require BAT Key for Code Exchange (PKCE)&quot; (Exiger la clé de bon à tirer pour l’ du code) est _NOT_ cochée, car cela interférerait avec la configuration.

## Configuration de Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* L’accès à l’API doit être activé pour l’utilisateur de synchronisation Salesforce (si vous êtes un utilisateur de Salesforce Professional Edition, cet accès n’est pas disponible par défaut ; veuillez contacter votre gestionnaire de compte Salesforce).
>* L’utilisateur de synchronisation Marketo doit être créé dans Salesforce.
>* Pour les clients existants, la fonctionnalité &quot;Activer OAuth pour la synchronisation SFDC&quot; est activée sur l’abonnement du client.
>* Les bloqueurs de fenêtres contextuelles sont désactivés.
>* L’application connectée est créée et nous disposons de la clé client et du secret client disponibles.

>[!CAUTION]
>
>Veillez à masquer tous les champs dont vous n’avez pas besoin dans Marketo de l’utilisateur de synchronisation avant de cliquer sur **[!UICONTROL Synchroniser les champs]**. Une fois que vous avez cliqué sur Synchroniser les champs, tous les champs visibles par l’utilisateur dans SFDC sont créés en permanence dans Marketo et ne peuvent pas être supprimés.

1. Dans la section Administration de Marketo, cliquez sur **[!UICONTROL CRM]**, puis sur **[!UICONTROL Synchroniser avec Salesforce]**.

   ![](assets/setting-up-oauth-2-7.png)

1. Ajoutez les informations Consumer Key et Consumer Secret que vous avez précédemment enregistrées, puis cliquez sur et **[!UICONTROL Enregistrer]**.

   ![](assets/setting-up-oauth-2-8.png)

1. Sur la page de synchronisation Marketo Salesforce, cliquez sur le bouton **[!UICONTROL Se connecter avec Salesforce]** .

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Si vous voyez des champs Nom d’utilisateur/Mot de passe/Jeton et non un bouton &quot;Connexion avec Salesforce&quot;, votre abonnement Marketo est activé pour l’authentification de base. Reportez-vous à la section [Configuration de Marketo avec authentification de base](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}. Une fois que la synchronisation commence à utiliser un ensemble d’informations d’identification, il n’y a plus de changement d’informations d’identification ou d’abonnement Salesforce. Si vous souhaitez utiliser Oauth 2.0, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

1. Une fenêtre contextuelle contenant la page de connexion Salesforce s’affiche. Clé dans vos informations d’identification &quot;Utilisateur de synchronisation Marketo&quot; et connectez-vous.

   ![](assets/setting-up-oauth-2-10.png)

1. Saisissez le code de vérification que vous avez reçu par courrier électronique (envoyé par Salesforce) et cliquez sur **[!UICONTROL Vérifier]**.

   ![](assets/setting-up-oauth-2-11.png)

1. Une fois la vérification effectuée, la page d’accès s’affiche pour demander l’accès. Cliquez sur **[!UICONTROL Autoriser]**.

   ![](assets/setting-up-oauth-2-12.png)

1. Dans quelques minutes, une fenêtre contextuelle s’affiche dans Marketo. Cliquez sur **[!UICONTROL Confirmer les informations d’identification]**.

   ![](assets/setting-up-oauth-2-13.png)

1. Une fois la synchronisation des champs terminée, cliquez sur **[!UICONTROL Démarrer la synchronisation Salesforce]**.

   ![](assets/setting-up-oauth-2-14.png)

1. Cliquez sur **[!UICONTROL Démarrer la synchronisation]**.

   ![](assets/setting-up-oauth-2-15.png)

Votre synchronisation entre Marketo et Salesforce est maintenant en cours.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [ Étape 1 sur 3 : Ajout de champs Marketo à Salesforce (Enterprise/Unlimited)&lbrace;1](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [ Étape 2 sur 3 : création d’un utilisateur Salesforce pour Marketo (Enterprise/Unlimited)&lbrace;1](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [Installer le package Marketo Sales Insight dans l&#39;AppExchange Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Configurer Marketo Sales Insight dans Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
