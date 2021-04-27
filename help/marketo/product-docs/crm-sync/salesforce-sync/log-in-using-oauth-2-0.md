---
description: Connexion à l’aide d’OAuth 2.0 - Marketo Docs - Documentation du produit
title: Connexion à l’aide d’OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Connectez-vous à l’aide d’OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce utilise le protocole OAuth pour permettre aux utilisateurs d&#39;applications d&#39;accéder en toute sécurité (authentifier l&#39;application à l&#39;aide des données OAuth 2.0) sans avoir à révéler les informations de connexion. Vous trouverez ci-dessous les étapes à suivre pour connecter et synchroniser Marketo en toute sécurité avec Salesforce.

## Configurer une application connectée {#set-up-connected-app}

1. Dans Salesforce, sous Configuration, dans les outils de plate-forme, accédez à Applications, App Manager, puis cliquez sur **Nouvelle application connectée**.

   ![](assets/setting-up-oauth-2-1.png)

1. Renseignez les détails et cliquez sur **Enregistrer**.

   ![](assets/setting-up-oauth-2-2.png)

1. Cochez la case **Activer les paramètres OAuth**. Pour l’URL de rappel, saisissez `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Sélectionnez toutes les étendues OAuth disponibles et cliquez sur **Ajouter**.

   ![](assets/setting-up-oauth-2-3.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/setting-up-oauth-2-4.png)

1. Cliquez sur **Continuer**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copiez le Consumer key et le Secret du client.

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>Enregistrez les informations sur le Consumer key et le Secret du client pour les utiliser ultérieurement dans Marketo.

## Configurer Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* L&#39;accès à l&#39;API doit être activé pour l&#39;utilisateur de synchronisation Salesforce (si vous utilisez Salesforce Professional Edition, cet accès n&#39;est pas disponible par défaut ; veuillez contacter votre responsable de compte Salesforce).
>* L&#39;utilisateur Marketo Sync doit être créé dans Salesforce.
>* Pour les clients existants, l’option &quot;Activer OAuth pour la synchronisation SFDC&quot; est activée sur l’abonnement du client.
>* Les bloqueurs de fenêtres contextuelles sont désactivés.
>* L’application connectée est créée et le Consumer key et le Secret du client sont disponibles.


>[!CAUTION]
>
>Veillez à masquer tous les champs dont vous n’avez pas besoin dans Marketo de l’utilisateur de synchronisation avant de cliquer sur **Synchroniser les champs**. Une fois que vous avez cliqué sur Synchroniser les champs, tous les champs visibles par l’utilisateur dans SFDC sont créés définitivement dans Marketo et ne peuvent pas être supprimés.

1. Dans la section Admin Marketo, cliquez sur **CRM**, puis sur **Synchroniser avec Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. Ajoutez les informations de Consumer key et de Secret du client que vous avez précédemment enregistrées, puis cliquez sur **Enregistrer**.

   ![](assets/setting-up-oauth-2-8.png)

1. Sur la page de synchronisation Marketo Salesforce, cliquez sur le bouton **Connexion avec Salesforce**.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Si vous voyez des champs Nom d’utilisateur/Mot de passe/Jeton et non un bouton &quot;Connexion avec Salesforce&quot;, votre Abonnement Marketo est activé pour l’authentification de base. Reportez-vous à [Configuration de Marketo avec l&#39;authentification de base](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). Une fois que la synchronisation commence à l&#39;aide d&#39;un jeu d&#39;informations d&#39;identification, il n&#39;y a pas de changement d&#39;informations d&#39;identification ou d&#39;abonnement Salesforce. Si vous souhaitez utiliser Oracle 2.0, contactez votre responsable de succès client.

1. Une fenêtre contextuelle contenant la page de connexion de la force de vente s&#39;affiche. Clic dans vos informations d’identification &quot;Marketo Sync User&quot; et connectez-vous.

   ![](assets/setting-up-oauth-2-10.png)

1. Entrez le code de vérification que vous avez reçu par courrier électronique (envoyé par Salesforce) et cliquez sur **Vérifier**.

   ![](assets/setting-up-oauth-2-11.png)

1. Une fois la vérification terminée, la page d’accès s’affiche pour demander l’accès. Cliquez sur **Autoriser**.

   ![](assets/setting-up-oauth-2-12.png)

1. Dans quelques minutes, une fenêtre contextuelle s’affiche à Marketo. Cliquez sur **Confirmer les informations d’identification**.

   ![](assets/setting-up-oauth-2-13.png)

1. Une fois la synchronisation des champs terminée, cliquez sur **Début Salesforce Sync**.

   ![](assets/setting-up-oauth-2-14.png)

1. Cliquez sur **Début Sync**.

   ![](assets/setting-up-oauth-2-15.png)

Votre synchronisation entre Marketo et Salesforce est en cours.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Étape 1 sur 3 : Ajouter les champs Marketo à Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Étape 2 sur 3 : Créer un utilisateur Salesforce pour Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installer le module Marketo Sales Insight dans l&#39;AppExchange Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurer Marketo Sales Insight dans Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

