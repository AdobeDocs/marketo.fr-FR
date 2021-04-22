---
description: Configuration d’OAuth 2.0 - Marketo Docs - Documentation du produit
title: Configuration d’OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Configuration d’OAuth 2.0 {#setting-up-oauth-2-0}

Salesforce utilise le protocole OAuth pour permettre aux utilisateurs des applications d’accéder en toute sécurité (d’authentifier l’application à l’aide d’OAuth 2.0) aux données via des appels d’API REST sans avoir à révéler les informations de connexion. Vous trouverez ci-dessous les étapes à suivre pour connecter et synchroniser Marketo en toute sécurité avec Salesforce.

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


1. Dans la section Admin Marketo, cliquez sur **CRM**, puis sur **Synchroniser avec Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. Ajoutez les informations de Consumer key et de Secret du client que vous avez précédemment enregistrées, puis cliquez sur **Enregistrer**.

   ![](assets/setting-up-oauth-2-8.png)

1. Sur la page de synchronisation Marketo Salesforce, cliquez sur le bouton **Connexion avec Salesforce**.

   ![](assets/setting-up-oauth-2-9.png)

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
