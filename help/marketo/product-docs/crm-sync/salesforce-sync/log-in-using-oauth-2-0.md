---
description: Connexion à l’aide d’OAuth 2.0 - Documents Marketo - Documentation du produit
title: Se connecter à l’aide d’OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Se connecter à l’aide d’OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce utilise le protocole OAuth pour permettre aux utilisateurs des applications d’accéder en toute sécurité aux données (d’authentifier l’application à l’aide d’OAuth 2.0) sans avoir à révéler leurs informations de connexion. Vous trouverez ci-dessous les étapes à effectuer pour connecter et synchroniser Marketo Engage avec Salesforce en toute sécurité.

>[!IMPORTANT]
>
>Pour connecter Marketo et [!DNL Salesforce] à l’aide d’OAuth, connectez-vous à Marketo via un navigateur privé (incognito) afin d’éviter de vous connecter à [!DNL Salesforce] avec un nom d’utilisateur incorrect.

## Configurer l’application connectée {#set-up-connected-app}

1. Dans Salesforce, sous Configuration, dans les outils de Platform, accédez à Applications, App Manager, puis cliquez sur **[!UICONTROL Nouvelle application connectée]**.

   ![](assets/setting-up-oauth-2-1.png)

1. Renseignez les détails et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/setting-up-oauth-2-2.png)

1. Cochez la case **[!UICONTROL Activer les paramètres OAuth]**. Pour l’URL de rappel, saisissez `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Sélectionnez toutes les portées OAuth disponibles et cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/setting-up-oauth-2-3.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/setting-up-oauth-2-4.png)

1. Cliquez sur **[!UICONTROL Continuer]**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copiez la clé du client et le secret du client (vous en aurez besoin ultérieurement pour les utiliser dans Marketo Engage).

   ![](assets/setting-up-oauth-2-6.png)

>[!CAUTION]
>
>Toujours sur la page Nouvelle application connectée , faites défiler la page vers le bas et assurez-vous que la case à cocher « Exiger la clé de vérification pour l’échange de code (PKCE) » est _NON_ cochée, car elle interfère avec la configuration.

## Configuration de Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* L’accès à l’API doit être activé pour l’utilisateur de la synchronisation Salesforce (si vous êtes un utilisateur de Salesforce Professional Edition, cet accès n’est pas disponible par défaut ; contactez votre chargé de compte Salesforce).
>* L’utilisateur de la synchronisation Marketo doit être créé dans Salesforce.
>* Pour les clients existants, la fonction « Activer OAuth pour la synchronisation SFDC » est activée sur l’abonnement du client.
>* Les bloqueurs de fenêtres contextuelles sont désactivés.
>* L’application connectée est créée et nous disposons des clés [!UICONTROL Consumer Key] et [!UICONTROL Consumer Secret] disponibles.

>[!CAUTION]
>
>Veillez à masquer tous les champs dont vous n’avez pas besoin dans Marketo à l’utilisateur de la synchronisation avant de cliquer sur **[!UICONTROL Synchroniser les champs]**. Une fois que vous avez cliqué sur Synchroniser les champs , tous les champs que l’utilisateur peut voir dans SFDC sont créés de manière permanente dans Marketo et ne peuvent pas être supprimés.

1. Dans la section Marketo Admin , cliquez sur **[!UICONTROL CRM]**, puis **[!UICONTROL Synchroniser avec Salesforce]**.

   ![](assets/setting-up-oauth-2-7.png)

1. Ajoutez les informations Clé du client et Secret du client que vous avez précédemment enregistrées et cliquez sur et **[!UICONTROL Enregistrer]**.

   ![](assets/setting-up-oauth-2-8.png)

1. Sur la page de synchronisation de Marketo Salesforce, cliquez sur le bouton **[!UICONTROL Se connecter avec Salesforce]**.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Si les champs Nom d’utilisateur/Mot de passe/Jeton s’affichent et non un bouton « Se connecter avec Salesforce », votre abonnement Marketo est activé pour l’authentification de base. Reportez-vous à la section [Configuration de Marketo avec une authentification de base](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}. Une fois que la synchronisation commence à utiliser un ensemble d’informations d’identification, il n’est plus possible de basculer sur les informations d’identification ou l’abonnement Salesforce. Si vous souhaitez utiliser Oauth 2.0, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

1. Un pop-up s’affiche avec la page de connexion à Salesforce. Saisissez vos informations d’identification « Utilisateur de synchronisation Marketo » et connectez-vous.

   ![](assets/setting-up-oauth-2-10.png)

1. Saisissez le code de vérification que vous avez reçu par e-mail (envoyé par Salesforce) et cliquez sur **[!UICONTROL Vérifier]**.

   ![](assets/setting-up-oauth-2-11.png)

1. Une fois la vérification effectuée, la page d’accès s’affiche pour demander l’accès. Cliquez sur **[!UICONTROL Autoriser]**.

   ![](assets/setting-up-oauth-2-12.png)

1. Dans quelques minutes, un pop-up apparaîtra dans Marketo. Cliquez sur **[!UICONTROL Confirmer les informations d’identification]**.

   ![](assets/setting-up-oauth-2-13.png)

1. Une fois la synchronisation des champs terminée, cliquez sur **[!UICONTROL Démarrer la synchronisation Salesforce]**.

   ![](assets/setting-up-oauth-2-14.png)

1. Cliquez sur **[!UICONTROL Démarrer la synchronisation]**.

   ![](assets/setting-up-oauth-2-15.png)

Votre synchronisation entre Marketo et [!DNL Salesforce] est en cours.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Étape 1 sur 3 : Ajouter des champs Marketo à Salesforce (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [Étape 2 sur 3 : création d’un utilisateur Salesforce pour Marketo (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [Installer le package Marketo Sales Insight dans Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
